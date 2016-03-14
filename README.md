# docker-machine-driver-veertu
Like xhyve, Veertu takes advantage of the Hypervisor.framework that was introduced in OS X 10.10, which brings Type 1 hypervisor technology (direct, host-level access to hardware) to OS X.

Why Veertu?. You can install it in the [AppStore]

There is no current docker-machine-driver for veertu. So I'll investigate the posibility to code one myself.

Who am I? No one, just some random Software Dev/Architect with ~10 years of experience out in the wild.

This branch was born by accident because of [twitter], veertu's quick responses and my couriosity.

Please join the [discussion] if you feel the need for this, have ideas, etc.

* [Docker Machine Driver Plugins] some documentation about how driver-plugins work.
* The idea behind this branch is to have the best, easiest and FREE way to get docker started in OSX with no hassle.
  * Install Veertu in the [AppStore]. (keep it updated from there)
  * Install docker toolbox if you don't already have it along with this plugin.
  * Run `docker-machine create --driver veertu ...`
  * And there you have it!

# Roadmap
* Create a basic hackish implementation until veertu has an API to talk to.
* Once Veertu has it's api implement all the driver functions with it.
* Add a good folder-sharing strategy. NFS, RSYNC or something like that by default.

## Some disclaimers:
* I don't have a lot of spare time in my life, but will do the best effort to make this work.
* If I can't make it work I will probably delegate this branch to someone with more time.
* Veertu doesn't have any API/CLI client as of today, so don't expect this branch having anything non-experimental soon.
* I'm not related to `Veertu Labs Ltd` in any way.


[//]: #Links
[AppStore]: https://itunes.apple.com/ar/app/veertu-native-virtualization/id1024069033?mt=12
[Docker Machine Driver Plugins]: https://github.com/docker/machine/pull/1902
[discussion]: https://forums.docker.com/t/veertu-driver-implementation
[twitter]: https://twitter.com/Qcho86/status/709191539784880128
