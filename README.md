### MTS SRE Course

namespace: **sre-cource-student-80**  
hub: **48bc7dbc-665e-4bfc-8518-baa92b5f2c62**

Для запуска плейбука необходимо заполнить инвентарь корректными хостами, указазть ansible_host, разложить ключи по управляемым хостам. Выполненена базовая конфигрурация в ansible.cfg (remote_user и inventory).  
В плейбуке несколько play с целевыми группами хостов.  
  
Пример запуска плейбука:  
```console
ansible-playbook install_cluster.yaml
```
