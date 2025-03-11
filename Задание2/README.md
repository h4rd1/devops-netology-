
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



