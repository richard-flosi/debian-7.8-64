Creates a [debian-7.8-64](https://atlas.hashicorp.com/puppetlabs/boxes/debian-7.8-64-puppet) [vagrant](https://vagrantup.com) box with [example.com](https://github.com/richard-flosi/example.com) website [provisioned with chef-solo](http://docs.vagrantup.com/v2/provisioning/chef_solo.html).

# Getting Started

Install [Vagrant](http://docs.vagrantup.com/v2/installation/) and [Virtual Box](https://www.virtualbox.org/wiki/Downloads).

Install the [Vagrant Berkshelf Plugin](http://berkshelf.com/):
`vagrant plugin install vagrant-berkshelf`

Clone this repository:
`git clone git@github.com:richard-flosi/debian-7.8-64.git`

Change into the cloned directory:
`cd debian-7.8-64`

And start the vagrant box:
`vagrant up`

Once this completes you will have a debian server running openresty with example.com host on it. On your local machine you can access the website at: http://192.168.33.10

Update the `/etc/hosts` file on your local machine to include:
`192.168.33.10	vagrant.example.com`

Now you can access the website at: http://vagrant.example.com/
