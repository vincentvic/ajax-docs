---
title: OnClientMouseOver
page_title: OnClientMouseOver | RadToolBar for ASP.NET AJAX Documentation
description: OnClientMouseOver
slug: toolbar/client-side-programming/onclientmouseover
tags: onclientmouseover
published: True
position: 19
---

# OnClientMouseOver

## 

The **OnClientMouseOver** client-side event occurs when the mouse moves over an item in the toolbar.

The event handler receives two parameters:

1. The instance of the toolbar firing the event.

1. An eventArgs parameter containing the following methods:

* **get_item** returns a reference to the item under the mouse.

* **get_domEvent** returns the DOM event object for the mouse movement.

You can use this event to respond when the mouse is over an item:

````ASPNET	
<script type="text/javascript">
    function ShowItem(toolbar, args) 
    {
        var label = document.getElementById("Label1");
        label.innerText = args.get_item().get_text();
    }
</script>

<telerik:radtoolbar id="RadToolBar1" runat="server" onclientmouseover="ShowItem">  
    <Items>    
    <telerik:RadToolBarButton Text="Button1" />     
    <telerik:RadToolBarButton Text="Button2" />    
    <telerik:RadToolBarButton Text="Button3" /> 
    </Items>
</telerik:radtoolbar>
<br />
<br />
<asp:Label ID="Label1" runat="server" Text=""></asp:Label>
````


