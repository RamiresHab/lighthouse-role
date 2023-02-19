Role Name
=========

Эта роль поднимает статику lighthouse для просмотра логов из Clickhouse.

Requirements
------------
Для работы этой роли требуется ansible версии 2.10 или выше.

Role Variables
--------------

У роли нет определяемых переменных. Роль использует template lighthouse.j2 для конфигурации nginx, сервер поднимается на 81 порту по http.

Dependencies
------------

Для работы этой роли необходимо предварительно поднять сервер с Clickhouse и сервер с Vector. Эту роль можно применить на сервер с ОС Ubutu 22.04 и выше.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - lighthouse-role

License
-------

MIT

Author Information
------------------

Roman Khabibullin
