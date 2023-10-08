### MTS SRE Course

namespace: **sre-cource-student-80**  
hub: **48bc7dbc-665e-4bfc-8518-baa92b5f2c62**

MVP. Плейбук для настройки HA Cluster Postgresql.  

Для запуска плейбука необходимо заполнить инвентарь корректными хостами, указазть ansible_host, разместить ssh ключи по управляемым хостам. Плейбук необходимо запускать с jump хоста (haproxy). Выполненена базовая конфигрурация в ansible.cfg (remote_user и inventory).  
В плейбуке несколько play с целевыми группами хостов.  
  
Пример запуска плейбука:  
```console
ansible-playbook install_cluster.yaml
```

helm чарт запускается из дирректории helm, следующей командой:  
```console
helm install sre-coourse-api sre-coourse-api --kubeconfig=/home/vagrant/kubeconfig
or
helm upgrade sre-coourse-api sre-coourse-api --kubeconfig=/home/vagrant/kubeconfig
```
