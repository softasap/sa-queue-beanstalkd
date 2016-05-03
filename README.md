sa-queue-beanstalkd
===================

[![Build Status](https://travis-ci.org/softasap/sa-queue-beanstalkd.svg?branch=master)](https://travis-ci.org/softasap/sa-queue-beanstalkd)

beanstalkd_properties: list of regexes in form (regexp, line) to adjust /etc/default/beanstalkd with necessary changes



Example of usage (all parameters are optional)

Simple

  roles:
    - {
        role: "sa-queue-beanstalkd"
      }


Advanced:


  roles:
    - {
        role: "sa-queue-beanstalkd",
        beanstalkd_properties:
          - {regexp: "^#START=.*", line: "START=yes"}
      }



