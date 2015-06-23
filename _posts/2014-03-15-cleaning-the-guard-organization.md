---
layout: post
title:  "Cleaning the Guard organization"
date:   2014-03-15 13:13:22
categories: guard, english
author: rymai
---

It is often misleading for Guard users to go to https://github.com/guard/guard-xxx and realize that it is an unmaintained fork of the plugin’s creator repo. For instance, this is the case for [guard/guard-teaspoon](https://github.com/guard/guard-teaspoon) which is a fork of [modeset/guard-teaspoon](https://github.com/modeset/guard-teaspoon).

Another issue is when both the [original plugin's repo](https://github.com/oliamb/guard-compass/issues) and the [forked repo](https://github.com/guard/guard-compass/issues) activate their issue tracker. This often leads to issues not reported at the right place.

Ideally, all the Guard plugins under the Guard organization should be up-to-date, maintained and with the issue tracker active. No forked plugins should be present under the organization.

My plan to realize that is as follow:

- ask each plugin’s creator/owner if they would be ok to transfer the plugin's origin to the Guard organization;  if they refuse, we will simply not fork the repo under the organization (or remove the already forked repo)
- as a side effect, we will always require the [MIT license](http://choosealicense.com/licenses/mit/) for all the Guard plugins under the Guard organization

Here are a few benefits to this strategy:

- Guard users will find all the “officials and maintained” repos [under the Guard organization](https://github.com/guard)
- when you’re a member of an organization on GitHub, you have access to an [agregated view of all the organization’s issues](https://github.com/organizations/guard/dashboard/issues/repos) and that’s awesome! For instance it could bring more awareness to Guard plugins that are not well-known and which struggles with unresolved issues
- when a maintainer do not want to maintain a plugin anymore, she can look for someone to maintain it and since the repo belongs to the organization, it is simply a matter of giving the rights to the new maintainer: no need to transfer the repo between users and so on

_Please keep in mind that ownership will be kept through the LICENSE file present for each plugin._

That's it, tell me what you think! ;)
