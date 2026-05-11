# Дипломный практикум в Yandex.Cloud

Данный репозиторий содержит Kubespray с настройками для развертывания Kubernetes кластера

Ansible Inventory с IP адресами виртуальных машин кластера хранится по пути `inventory/mycluster/hosts.yml`

Запуск Kubespray производится из директории `kubespray` при помощи команды: `ansible-playbook -i inventory/mycluster/hosts.yml cluster.yml`

Созданная инфраструктура при помощи Kubespray:

![Ответ на задание 1](https://github.com/Francotirado/diploma-ansible/blob/main/img/1.jpg)

![Ответ на задание 1](https://github.com/Francotirado/diploma-ansible/blob/main/img/4.jpg)

Содержимое файла `~/.kube/config` в мастер ноде кластера (далее потребуется для репозитория diploma-k8s для автоматизированного развертывания пайплайна для секрета **KUBE_CONFIG**):

![Ответ на задание 1](https://github.com/Francotirado/diploma-ansible/blob/main/img/2.jpg)

Выполнение команды `kubectl get pods --all-namespaces`

![Ответ на задание 1](https://github.com/Francotirado/diploma-ansible/blob/main/img/3.jpg)
