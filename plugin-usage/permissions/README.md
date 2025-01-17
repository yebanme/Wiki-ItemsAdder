# 👌🏻Permissions

* Users

  * /ia
    * `ia.user.ia`
  * /iarecipe
    * `ia.user.iarecipe`
  * /iatexture \(to force apply the pack to yourself\)
    * `ia.user.iatexture`
  * /iatexture all \(to force apply the pack to everyone\)
    * `ia.user.iatexture.all`
  * crafting
    * `ia.user.craft.PERMISSION` \(or to give all crafting permissions just use ia.user.craft.\*\)
    * for more info about item permissions please[ read this](../adding-content/advanced/item-properties/basic/item-permission.md)
  * see item in /ia menu
    * `ia.user.ia.PERMISSION` \(or to give all /ia permissions just use ia.user.ia.\*\)
    * for more info about item permissions please[ read this](../adding-content/advanced/item-properties/basic/item-permission.md)
    * `ia.user.iasearchgui` for the search GUI in /ia menu
    * You can also set a permission per category, please check [/ia GUI ](../ia.md)page
  * emoji \(font images\)
    * **/iaimage /emoji, /iaemoji, /e** book GUI \(shows a book with the list of emojis/font images\)
      * `ia.user.image.gui`
    * **/iaimage** **/emoji &lt;text&gt;, /iaemoji &lt;text&gt;, /e &lt;text&gt;** \(shows a tab list with emojis based on searched term\)
      * `ia.user.image.hints`
    * Use emojis in chat
      * `ia.user.image.chat`
    * Use emojis in commands
      * `ia.user.image.command`
    * Use emojis in signs
      * `ia.user.image.sign`
    * Use emojis in books
      * `ia.user.image.book`
    * Use emojis in anvil rename field
      * `ia.user.image.anvil`
    * Permission to use an emoji
      * `ia.user.image.use.<font image name>`
      * Example: `ia.user.image.use.heart`

  ​

* Admin
  * /iaget
    * `ia.admin.iaget`
  * /iagive
    * `ia.admin.iagive`
  * /iadrop
    * `ia.admin.iadrop`
  * /iaremove
    * `ia.admin.iaremove`
  * /iatag
    * `ia.admin.iatag`
  * /iareload
    * `ia.admin.iareload`
  * /iazip
    * `ia.admin.iazip`
  * /iablock _\(get info about block you're looking at\)_
    * `ia.admin.iablock`
  * /ialiquid _\(get info about custom liquid you're looking at\)_
    * `ia.admin.ialiquid`
  * /iadurability
    * ia.admin.iadurability
  * Edit permission \(edit button in /ia\)
    * `ia.admin.edit`
  * /iaplayerstat write _\(write a player custom stat\)_
    * `ia.admin.iaplayerstat.write`
  * /iaplayerstat read _\(read a player custom stat\)_
    * `ia.admin.iaplayerstat.read`
  * /iainfo \(get info about the plugin\)
    * `ia.admin.iainfo`
  * /iakill &lt;mob\|all&gt; \(kill custom mobs\)
    * `ia.admin.iakill`
  * /iasummon &lt;mob&gt; \[amount\]
    * `ia.admin.iasummon`
  * /iaexport &lt;namespace&gt;
    * `ia.admin.iaexport`
  * /iaspawntree &lt;tree&gt;
    * `ia.admin.iaspawntree`
  * /iaplaytotemanimation &lt;totem&gt; &lt;player&gt;
    * `ia.admin.iatotemanimation`
  * /iaplaysound &lt;sound&gt; &lt;player&gt;
    * `ia.admin.iaplaysound`
  * /iacleancache
    * `ia.admin.iacleancache`
* Other:
  * Bypass kick on refuse resourcepack
    * `ia.resourcepack.bypasskick`
  * Bypass player placed blocks can't drop loot
    * `ia.admin.bypassblockplaceloot`

