# Ansible Role for configure a kvm vm.

**summary**
This role is for configuring a kvm vm inclusive cloudinit config. 
Look in the tasks directory for each configuration.
All configurations are held atomically via their own files. 

## Variables that have to be defined

| variable | description |
| -------- | ----------- |
| cloudinit_fqdn | fqdn |
| kvm_image_size | resitze image to ... |
| kvm_download_url | download url |
| kvm_dist_release_date | release date of the image|
| kvm_distname | distribution name |
| kvm_image_name | name of the image |
| kvm_cloudimage_kvm_url | download uri part to combine with kvm_download_url |
| kvm_cloudimage_kvm_checksum | sha265sum |
| kvm_image_path | path to store the kvm-image |
| cloudinit_rendering | container or virt, for a kvm image choose virt |