INFO FOR SKINNERS - How to use this addon in your skin:


RunScript(script.image.resource.select,type=Foo)

If you run the script like this, it will open a select dialog with all installed image resource addons of the given type.
The first item in the list (none) can be used to remove the current mapping.
The last item in the list (get more..) will allow users to install additional image resource addons.

After selecting one, the script will set the following skin string: Foo

You can now use $INFO[Skin.String(Foo)] to access the images inside the image resource addon.


example usage:
- RunScript(script.image.resource.select,type=resource.images.studios)
- $INFO[Skin.String(resource.images.studios)]
