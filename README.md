# Postgresql database server whenever you need one

## Dependencies

You'll need to have the following tools installed for this to work

* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* [Vagrant](http://vagrantup.com/)

## Instructions

This repo contains everything necessary to stand up a local instance of an
ubuntu 12.04 server running postgresql and phppgadmin.

To get the server going execute the following in the directory:

    vagrant up

To shutdown the database server do the following:

    vagrant halt

To destroy the database server do the following (this will remove all data):

    vagrant destroy

Postgres Admin: postgres, Password: password

DB for tests: postgres://postgres:password@localhost:5432/testdb

## Troubleshooting

This vagrant box takes ports 5432 and 11211 so if you have processes listening
on those ports then things might not work.

