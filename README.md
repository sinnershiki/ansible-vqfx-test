vqfx-vagrantを使って、juniper検証
--

# 概要
juniperには、qfxのvirtual環境が公式によってあがっているので、それを使ってjunosにAnsibleを流し込む検証をします

https://github.com/Juniper/vqfx10k-vagrant

# how to use

```
% cd /path/to/full-2qfx/
% vagrant ssh-config >> ssh_config
% /path/to/another_dir
% git clone https://github.com/sinnershiki/ansible-vqfx-test
% cd ansible-vqfx-test
% cp /path/to/full-2qfx/ssh_config .
% ansible-playbook -i hosts show_config.yml
```
