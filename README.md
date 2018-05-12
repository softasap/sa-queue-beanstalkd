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




Usage with ansible galaxy workflow
----------------------------------

If you installed the `sa-queue-beanstalkd` role using the command


`
   ansible-galaxy install softasap.sa-queue-beanstalkd
`

the role will be available in the folder `library/softasap.sa-queue-beanstalkd`
Please adjust the path accordingly.

```YAML

     - {
         role: "softasap.sa-queue-beanstalkd"
       }

```


Copyright and license
---------------------

Code is dual licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) and the [MIT License] (http://opensource.org/licenses/MIT). Choose the one that suits you best.

Reach us:

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)

Join gitter discussion channel at [Gitter](https://gitter.im/softasap)

Discover other roles at  http://www.softasap.com/roles/registry_generated.html

visit our blog at http://www.softasap.com/blog/archive.html

