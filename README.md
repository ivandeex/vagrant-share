# Role ivansible.vagrant-share

Creates a CIFS mount of temporary developer directory from vagrant host.


## Requirements

You must share your directory on the vagrant host

### Enable sharing on the virtualbox host network

![1-1.network-adapter-list](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/1-1.network-adapter-list.png)

![1-2.network-adapter-props](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/1-2.network-adapter-props.png)

### Share your folder

![3-1.explorer.folder](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/3-1.explorer.folder.png)

![3-2.explorer.props-sharing](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/3-2.explorer.props-sharing.png)

![3-3.explorer.new-sharing](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/3-3.explorer.new-sharing.png)

![3-4.explorer.set-name](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/3-4.explorer.set-name.png)

![3-5.explorer.open-perms](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/3-5.explorer.open-perms.png)

![3-6.explorer.change-perms](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/3-6.explorer.change-perms.png)

### Verify your share is on the list of computer shares

![2-1.cman-admin-tools](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/2-1.cman-admin-tools.png)

![2-2.cman-comp-mgmt](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/2-2.cman-comp-mgmt.png)

![2-3.cman-shares](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/2-3.cman-shares.png)

![2-4.cman-share-props](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/2-4.cman-share-props.png)

![2-5.cman-perms](https://raw.githubusercontent.com/ivansible/vagrant-share/master/help/images/2-5.cman-perms.png)


## Variables

    vg_share_host: 192.168.1.1
    vg_share_name: ''
    vg_share_user: {{ansible_user_id}}
    vg_share_pass: secret_pass
    vg_share_mount: ~/shares/host"

...


## Tags

None


## Dependencies

None


## Running

    ./scripts/run-role vagrant-share dock1

## License

MIT


## Author

Created in 2018 by [IvanSible](https://github.com/ivansible)
