# Changelog Jeedom V4.1

## 4.1.0

### Prerequisites

- Debian 10 Buster

### News / Improvements

- **Synthesis** : New page **Home → Synthesis** offering a global visual summary of the parts, with quick access to summaries.
- **Research** : Add of a search engine in **Tools → Search**.
- **Dashboard** : Edit mode now inserting the moved tile.
- **Dashboard** : Edit mode: the equipment refresh icons are replaced by an icon allowing access to their configuration, thanks to a new simplified modal.
- **Dashboard** : We can now click on the *time* time actions widgets to open the history window of the linked info command.
- **Dashboard** : The size of a new equipment&#39;s tile adapts to its content.
- **Dashboard** : Add (back!) A button to filter the displayed items by category.
- **Dashboard** : Ctrl Click on an info opens the history window with all the historicized commands of the equipment visible on the tile. Ctrl Click on a legend to display only this one, Alt Click to display them all.
- **Dashboard** : Redesign of the display of the object tree (arrow to the left of the search).
- **Dashboard** : Ability to blur background images (Configuration -> Interface).
- **Tools / Widgets** : Function *Apply on* shows the linked commands checked, unchecking one will apply the default core widget to this command.
- **Widget** : Adding a core widget *sliderVertical*.
- **Widget** : Adding a core widget *binarySwitch*.
- **Update Center** : Updates are checked automatically when opening this page and update check is older than 120mins.
- **Update Center** : The progress bar is now on the tab *Core and plugins*, and the log open by default on the tab *Information*.
- **Update Center** : If you open another browser during an update, the progress bar and the log indicate it.
- **Update Center** : If the update finishes correctly, display of a window asking to reload the page.
- **Core updates** : Implementation of a system for cleaning up old unused Core files.
- **Scenario** : Adding a search engine (to the left of the Run button).
- **Scenario** : Addition of the age function (gives the age of the value of the order).
- **Scenario** : *stateChanges()* now accept the period *Today* (midnight to now), *yesterday* and *day* (for 1 day).
- **Scenario** : Functions *statistics (), average (), max (), min (), trend (), duration()* : Bugfix over the period *yesterday*, and accept now *day* (for 1 day).
- **Scenario** : Possibility to deactivate the automatic quote system (Settings → System → Configuration : Commandes).
- **Scenario** : Viewing a *Warning* if no trigger is configured.
- **Scenario** : Bugfix of *select* on block copy / paste.
- **Scenario** : Copy / paste of block between different scenarios.
- **Scenario** : The undo / redo functions are now available as buttons (next to the block creation button).
- **Scenario** :  addition of "Historical export" (exportHistory)
- **Scenario variables window** : Alphabetical sort at opening.
- **Scenario variables window** : The scenarios used by the variables are now clickable, with opening of the search on the variable.
- **Analysis / History** : Ctrl Click on a legend to display only this history, Alt Click to display them all.
- **Analysis / History** : The options *grouping, type, variation, staircase* are active only with a single displayed curve.
- **Analysis / History** : We can now use the option *Area* with the option *Steps*.
- **Analysis / Logs** : New monospace type font for logs.
- **View** : Possibility to put scenarios.
- **View** : Edit mode now inserting the moved tile.
- **View** : Edit mode: the equipment refresh icons are replaced by an icon allowing access to their configuration, thanks to a new simplified modal.
- **View** : The display order is now independent of that on the Dashboard.
- **Timeline** : Separation of History and Timeline pages.
- **Timeline** : Integration of the Timeline in DB for reliability reasons.
- **Timeline** : Management of multiple timelines.
- **Timeline** : Complete graphic redesign of the timeline (Desktop / Mobile).
- **Global Summary** : Summary view, support for summaries from a different object or with an empty root object (Desktop and WebApp).
- **Tools / Objects** : New tab *Summary by equipment*.
- **Domotic overview** : Plugin equipments deactivated and their controls no longer have the icons on the right (equipment configuration and advanced configuration).
- **Domotic overview** : Ability to search on equipment categories.
- **Domotic overview** : Possibility to move several pieces of equipment from one object to another.
- **Domotic overview** : Possibility to select all the equipment of an object.
- **Task engine** : On the tab *Daemon*, disabled plugins no longer appear.
- **Report** : The use of *chromium* if available.
- **Report** : Possibility to export timelines.
- **Configuration** : The tab *Information* is now in the tab *Main*.
- **Configuration** : The tab *Commands* is now in the tab *Equipments*.
- **Advanced equipment configuration window** : Dynamic change of table configuration.
- **Equipments** : New Category *Opening*.
- **Equipments** : Possibility of inverting cursor type commands (info and action)
- **Equipments** : Possibility to add class css to a tile (see widget documentation).
- **About window** : Addition of links to Changelog and FAQ.
- Widgets / Objects / Scenarios / Interactions / Plugins Pages :
	- Ctrl Clic / Clic Center on a Widget, Object, Scenarios, Interaction, plugin equipment : Opens in a new tab.
	- Ctrl Clic / Clic Center also available in their context menus (on the tabs).
- New ModalDisplay page :
	- Analysis menu : Ctrl Click / Click Center on *Real time* : Open the window in a new tab, in full screen.
	- Tools menu : Ctrl Click / Click Center on *Notes*, *Expression tester*, *Variables*, *Research* : Open the window in a new tab, in full screen.
- Code Block, File Editor, Advanced Customization : Dark theme adaptation.

### WebApp
- Integration of the new Synthesis page.
- Scenarios page, a click on the scenario title displays its log.
- We can now select / copy part of a log.
- On the search in a log, addition of an x button to cancel the search.
- Persistence of the theme toggle (8h).
- On a design, a click with three fingers returns to the home page.
- Display of scenarios by group.
- New monospace type font for logs.
- Many bug-fix (UI, portrait / landscape iOS, etc.).

### Autres
- **Documentation** : Adaptations in line with v4 and v4.1.
- **Documentation** : New page *Keyboard / mouse shortcuts* including a summary of all shortcuts in Jeedom. Accessible from the Dashboard doc or the FAQ.
- **Lib** : Update HighStock v7.1.2 to v8.2.0.
- **Lib** : Update jQuery v3.4.1 to v3.5.1.
- **Lib** : Update Font Awesome 5.9.0 to 5.13.1.
- **API** :  addition of an option to prohibit an api key of a plugin from executing core methods (general)
- Securing Ajax requests.
- Securing API calls.
- Bug fixes.
- Numerous desktop / mobile performance optimizations.

### Changements
- Function **scenario-> getHumanName()** of the php scenario class no longer returns *[object] [group] [name]* But *[group] [object] [name]*.
- Function **scenario-> byString()** must now be called with the structure *[group] [object] [name]*.
- Functions **network-> getInterfaceIp () network-> getInterfaceMac () network-> getInterfaces()** have been replaced by **network-> getInterfacesInfo()**


# Changelog Jeedom V4.0

## 4.0.61

- Fixed a problem when applying a scenario template
- Addition of an option to disable SSL verification during communication with the market (not recommended but useful in certain specific network configuration)
- Fixed an issue with archiving history if the smoothing mode was forever
- Bug fixes
- Correction of the trigger () command in scenarios so that it returns the name of the trigger (without the #) instead of the value, for the value you must use triggerValue()

## 4.0.60

- Removal of the new DNS system in eu.jeedom.link following too many operators who prohibit permanent http2 flows

## 4.0.59

- Fixed bugs on time widgets
- Increase in the number of bad passwords before banishment (avoids problems with the webapp when rotating API keys)

## 4.0.57

- Reinforcement of cookie security
- Using chromium (if installed) for reports
- Fixed a problem with calculating state time on widgets if the jeedom time zone is not the same as that of the browser
- Bugfix

## 4.0.55

- The new dns (\*. Eu.jeedom.link) becomes the primary DNS (the old DNS still works)

## 4.0.54

- Start of the update to the new documentation site

## 4.0.53

- Bug fix.

## 4.0.52

- Bug correction (update to do absolutely if you are in 4.0.51).

## 4.0.51

- Bugfix.
- Optimization of the future DNS system.

## 4.0.49

- Possibility of choosing the Jeedom TTS engine and possibility of having plugins that offers a new TTS engine.
- Improved webview support in the mobile application.
- Bugfix.
- Updating the doc.

## 4.0.47

- Improved expression tester.
- Updating the repository on smart.
- Bugfix.

## 4.0.44

- Improved translations.
- Bugfix.
- Improved cloud backup restore.
- Cloud restoration now only retrieves the local backup, leaving the choice to download or restore it.

## 4.0.43

- Improved translations.
- Fixed bugs on scenario templates.

## 4.0.0
- Complete theme redesign (Core 2019 Light / Dark / Legacy).
- Possibility to change the theme automatically depending on the time.
- In mobile, the theme may change depending on the brightness (Requires to activate *generic extra sensor* in chrome, chrome page://flags).<br/><br/>
- Improvement and reorganization of the main menu.
- Plugins menu : The list of categories and plugins is now sorted alphabetically.
- Tools menu : Add a button to access the expression tester.
- Tools menu : Adding a button to access the variables.<br/><br/>
- Search fields now support accents.
- The search fields (Dashboard, scenarios, objects, widgets, interactions, plugins) are now active when the page is opened, allowing you to type a search directly.
- Added an X button on the search fields to cancel the search.
- During a search, the key *escape* cancel search.
- Dashboard : In edit mode, the search control and its buttons are disabled and become fixed.
- Dashboard : In edit mode, a click of a button *expand* to the right of objects resizes the tiles of the object to the height of the highest. Ctrl + click reduces them to the height of the lowest.
- Dashboard : Command execution on a tile is now signaled by the button *Refresh*. If there is none on the tile, it will appear during execution.
- Dashboard : The tiles indicate an info command (historized, which will open the History window) or action on hover.
- Dashboard : The history window now allows you to open this history in Analysis / History.
- Dashboard : The history window keeps its position / dimensions when reopening another history.
- Command Configuration window: Ctrl + click on "Save" closes the window after.
- Equipment Configuration window: Ctrl + click on "Save" closes the window after.
- Add usage information when deleting a device.
- Objects : Added option to use custom colors.
- Objects : Addition of a contextual menu on the tabs (quick object change).
- Interactions : Addition of a contextual menu on the tabs (quick change of interaction).
- Plugins : Addition of a contextual menu on the tabs (quick change of equipment).
- Plugins : On the Plugins management page, an orange point indicates the plugins in non-stable version.
- Table improvements with filter and sort option.
- Possibility to assign an icon to an interaction.
- Each Jeedom page now has a title in the interface language (browser tab).
- Prevention of auto-filling on 'Access code' fields'.
- Function management *Previous page / Next page* from the browser.<br/><br/>
- Widget : Redesign of the widget system (Tools / Widgets menu).
- Widget : Possibility to replace a widget by another on all the commands using it.
- Widget : Possibility of assigning a widgets to several commands.
- Widget : Adding a horizontal numeric info widget.
- Widget : Adding a vertical numeric info widget.
- Widget : Addition of a numeric compass / wind info widget (thanks @thanaus).
- Widget : Added a numeric rain info widget (thanks @thanaus)
- Widget : Display of the info / action shutter widget proportional to the value.<br/><br/>
- Configuration : Improvement and reorganization of tabs.
- Configuration : Addition of many *tooltips* (aide).
- Configuration : Adding a search engine.
- Configuration : Added a button to empty the cache of widgets (Cache tab).
- Configuration : Added an option to disable the cache of widgets (Cache tab).
- Configuration : Possibility of vertically centering the content of the tiles (Interface tab).
- Configuration : Added a parameter for the global purge of logs (Orders tab).
- Configuration : Change of #message# At #subject# in Configuration / Logs / Messages to avoid duplicating the message.
- Configuration : Possibility in the summaries to add an exclusion of orders that have not been updated for more than XX minutes (example for the calculation of temperature averages if a sensor has not reported anything for more than 30min it will be excluded from the calculation)<br/><br/>
- Scenario : The colorization of blocks is no longer random, but by block type.
- Scenario : Possibility by doing a Ctrl + click on the button *execution* save it, launch it, and display the log (if the log level is not on *None*).
- Scenario : Confirmation of block deletion. Ctrl + click to avoid confirmation.
- Scenario : Addition of a search function in Code blocks. Search : Ctrl + F then Enter, Next result : Ctrl + G, Previous result : Ctrl + Shift + G
- Scenario : Possibility of condensing the blocks.
- Scenario : The 'Add block' action switches to the Scenario tab if necessary.
- Scenario : New block copy / paste functions. Ctrl + click to cut / replace.
- Scenario : A new block is no longer added at the end of the scenario, but after the block where you were before clicking, determined by the last field you clicked.
- Scenario : Setting up an Undo / Redo system (Ctrl + Shift + Z / Ctrl + Shift + Y).
- Scenario : Remove scenario sharing.
- Scenario : Improvement of the scenario template management window.<br/><br/>
- Analysis / Equipment : Addition of a search engine (Batteries tab, search on names and parents).
- Analysis / Equipment : The calendar / equipment day zone can now be clicked to directly access the battery change (s).
- Analysis / Equipment : Adding a search field.<br/><br/>
- Update Center : Warning on the 'Core and plugins' and / or 'Others' tab if an update is available. Switch to 'Others' if necessary.
- Update Center : differentiation by version (stable, beta, ...).
- Update Center : addition of a progress bar during the update.<br/><br/>
- Domotic overview : The history of deletions is now available in a tab (Summary - History).
- Domotic overview : Complete redesign, possibility of ordering objects, equipment, orders.
- Domotic overview : Adding equipment and order IDs, to display and search.
- Domotic overview : CSV export of parent object, id, equipment and their id, command.
- Domotic overview : Possibility of making visible or not one or more commands.<br/><br/>
- Design : Possibility to specify the order (position) of the *Designs* and *3D designs* (Edit, Configure Design).
- Design : Addition of a custom CSS field on the elements of the *Design*.
- Design : Moved the display options in Design of the advanced configuration, in the display parameters from the *Design*. This in order to simplify the interface, and to allow to have different parameters by *Design*.
- Design : Moving and resizing components on *Design* takes their size into account, with or without magnetization.<br/><br/>
- General lightening (css / inline styles, refactoring, etc.) and performance improvements.
- Remove Font Awesome 4 to keep only Font Awesome 5.
- Libs update : jquery 3.4.1, CodeMiror 5.46.0, tablesorter 2.31.1.
- Numerous bug fixes.
- Addition of a mass configuration system (used on the Equipment page to configure Communications Alerts on them)
- Addition of global compatibility of Jeedom DNS with a 4G internet connection.
- Security fix

>**Important**
>
>If after the update you have an error on the Dashboard, try to restart your box so that it takes the new additions of components into account.

>**Important**
>
>The widget plugin is not compatible with this version of Jeedom and will no longer be supported (because the features have been taken internally on the core). More information [here](https://www.Jeedom.com/blog/4368-les-widgets-en-v4).


