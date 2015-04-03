---
title: PersistenceFramework Overview
page_title: Overview | UI for ASP.NET AJAX Documentation
description: Overview
slug: persistenceframework/overview
tags: overview
published: True
position: 0
---

# PersistenceFramework Overview



Telerik’s Persistence Framework provides the ability to preserve and restore the state of Telerik UI for ASP.NET AJAX, which gives your end users the freedom to arrange and use your app in a way most convenient to them. The framework mainly saves and loads settings of the Telerik controls which are UI configurable, e.g. RadTreeView’s expanded, checked and selected state.You can see this in action in our [online demos](http://demos.telerik.com/aspnet-ajax/persistence-framework/examples/overview/defaultcs.aspx).

The core functionality is presented by RadPersisterManager and RadPersisterManagerProxy – there should be only one instance of the RadPersistenceManager and the proxies are defined on the content pages or user controls to persists the state of the controls on them. RadPersistenceManager allows you to save and load custom key-value settings.

Key features of the framework are:

* Long-term persistence of Telerik controls' UI-modifiable state

* Persistence of custom key-value settings

* Ability to implement own storage and serialization providers