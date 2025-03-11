
Задача 1

Установите на личный Linux-компьютер или учебную локальную ВМ с Linux следующие сервисы(желательно ОС ubuntu 20.04):

    VirtualBox,
    Vagrant, рекомендуем версию 2.3.4
    Packer версии 1.9.х + плагин от Яндекс Облако по инструкции
    уandex cloud cli Так же инициализируйте профиль с помощью yc init .

Примечание: Облачная ВМ с Linux в данной задаче не подойдёт из-за ограничений облачного провайдера. У вас просто не установится virtualbox.

Не использую vbox, hyper-v/docker_desktop

    PS C:\WINDOWS\system32> Get-VM | Format-List Name,Generation


    Name       : DockerDesktopVM
    Generation : 2

    Name       : Ubuntu 20.04 LTS
    Generation : 2

    Name       : VMBitrix9.0-0-CentOSStream9-HyperV
    Generation : 1

Vagrant 

    h4rd@vm1:~$ vagrant -v
    Vagrant 2.2.6

Ansible 

    h4rd@vm1:~$ ansible --version
    ansible 2.9.6
      config file = /etc/ansible/ansible.cfg
      configured module search path = ['/home/h4rd/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
      ansible python module location = /usr/lib/python3/dist-packages/ansible
      executable location = /bin/ansible
      python version = 3.8.10 (default, Mar 15 2022, 12:22:08) [GCC 9.4.0]

Packer

    h4rd@vm1:~$ packer --version
    Packer v1.11.2


Yandex cloud 

    h4rd@vm1:~$ yc init
    Welcome! This command will take you through the configuration process.

Задача 2




