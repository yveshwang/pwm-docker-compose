Title: PWM in 3 steps
Author: Yves Hwang
Date: September 26, 2017

PWM in 3 steps
==============
A simple demo PWM setup to get started. Emphasis here is to illustrate fit, and this is by no means a production ready setup.

Links
=====

* [PWM-Documentation][https://github.com/pwm-project/pwm/wiki/PWM-Documentation]
* [PWM Project][https://github.com/pwm-project/pwm]
* [osixia/openldap][https://github.com/osixia/docker-openldap]
* [osixia/docker-phpLDAPadmin][https://github.com/osixia/docker-phpLDAPadmin]
* [fjudith/pwm][https://github.com/fjudith/docker-pwm]

Getting started
===============
As mentioned, this should be as easy and as painless to get going as possible.

1. `docker-compose up`

2. configure LDAP a little by going to [https://localhost:6443/][https://localhost:6443/], use the default `cn=admin,dc=example,dc=org` with password as `admin` 

3. configure PWM by going to [http://localhost:8080/][http://localhost:8080/]

Only 3 steps?
=============
This is a little misleading of course as the configuration of PWM can be rather tricky. But this should be an adequate springboard for someobody with PWM know-how.

PWM Setup
=========
Note that TLS is disabled for this setup for simplicity. Note that PWM defaults to `636` for accessing openldap. This is the TLS port, so be sure to change that to `389`. Also note that one can use `openldap` can be used as hostname also in PWM. 
