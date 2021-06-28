# evok2mqtt-ansible

Ansible setup to provision an unipi neuron unit with [`evok2mqtt`].

For my home automation setup, I use a hardware platform called [unipi], which runs the [`evok`] software to interface with.
[`evok2mqtt`] is my own custom software that bridges between `evok` and an MQTT broker.

For more details, checkout out my [blog] and my [home automation series] in particular!

## Quick start

Install all galaxy requirements:

    ansible-galaxy install -r requirements.yaml

Run the playbook

    ansible-playbook site.yaml -i hosts.yaml

## Password

I manage my passwords using [`pass`].
The ansible community provides a [pass plugin] that integrates with this tool.

[`evok2mqtt`]: https://github.com/mhemeryck/evok2mqtt
[unipi]: https://www.unipi.technology/
[`evok`]: https://github.com/UniPiTechnology/evok
[blog]: https://blog.mhemeryck.com
[home automation series]: https://blog.mhemeryck.com/2021-06-15/home_automation_why
[`pass`]: https://www.passwordstore.org/
[pass plugin]: https://docs.ansible.com/ansible/latest/collections/community/general/passwordstore_lookup.html
