# Preamble #

First and main rule of this application is

#### "It's not to search content, but to download" ####

This means you're using an app to download content only from known resources. And in this way this means if you getting errors or nothing from resources you're DO NOT know - it's your own problem, not app's.

Resources are too different from each other, and there is no way to make only ONE way to download from all of them a the same time. They're have different search rules, keywords, storing methods and other. So, you must to know, how to work with resource you're using.

# Contents #
  * [First screen](#First_screen.md)
  * [New list screen](#New_list_screen.md)
  * [Downloading](#Downloading.md)
  * [Filter features](#Filter_features.md)
  * [Settings](#Settings.md)
    * [Interface](#Interface.md)
    * [Threads](#Threads.md)
    * [Proxy](#Proxy.md)
    * [Doubles](#Doubles.md)
  * [Name formatting](#Name_formatting.md)
    * [string-number format](#string-number_format.md)
    * [datetime format](#datetime_format.md)

# First screen #

By default, after launch the application automatically checks for updates. If updates will be found, a window pops up and suggest to update the application. You can disable autochek in settings.


### Buttons ###
  * **New list** - create a new list;
  * **Load list** - don't work right now;
  * **Settings** - well, app settings;
  * **Exit** - Exit.

# New list screen #

Appears after clicking "New List".

On the right side located a list of resources that you can add. On the left side - list of added items.
To add item you need to click a button with arrow, also you can remove items from the current list.

To the next step of list making you need to click a "Continue" button. For return click a "Change list" button.

After clicking "Continue" button a resource settings panel will appear. "General" item in the list is global for all list's items, if you're don't want to inherit settings from it you need to uncheck "Inherit configuration" flag for other resources in list.

To finish list click "Finish".

After you made your first list, next time the constructor will skip the first (select resource) part and will suggest to use last time used set again. To change it just click "change list" button.

# Downloading #

List gathering will start just after list creation. You can interrupt list gathering by clicking a "Stop getting list" button on the main menu.

After finished gathering you can start download pictures. For it you need to click "Start download pictures" button. To interrupt it click a "stop pictures downloading". Will be downloaded only marked by checkbox pictures.

"Fields" menu allows you to add or remove picture's attributes to the table.

"Filter" execute filter's settings.

"Check" and "Uncheck" allows to execute massive marking of pictures. You can select "all","selected" or "filtered", also you can "invert" marking.

To add new tab (and to start new list) you need to click "new list" from main menu.

On the bottom of table you can see supporting information:
  * **ON AIR** - work in progress;
  * **TTL** - total amount of items;
  * **IGN** - ignored duplicates;
  * **TBL** - time sued to add item to the table (ms);
  * **DBL** - time used to add item to the massive (including duplicate search, ms).

# Filter features #

All fields that can be filtered have their own data types.<br />
In this way, for number-fields you can chose "less" or "more" conditions, but for string-fields you can only chose "equal" or "contains". For "contains" condition you must use rules like in SQL:
  * symbol "%" means it doesn't matter which text instead of this symbol, ex.: "%sup" - will be searched all words ending with "sup"; "f%k" - starting with "f" and ending with "k";
  * symbol "`_`" means skipping an one symbol. ex.: pic00`_` - there will be searched all pictures, where only last symbol can by any.

When downloading in progress, "Downloaded", "Size" and "Progress" fields will appear. If you will filter field "Downloaded" by content (i.e. = not empty), you can watch all downloading pictures by this moment.

# Settings #

### Interface ###
  * **Language** - interface language;
  * **Check updates on application started** - automatically check for updates when application started;
  * **Check updates now** - well, click it to check for updates now;
  * **Appearance** - list of build-in skins. Not really big list;
  * **Use "Look-n-feel" style** - application will try to inherit style from your OS;
  * **Show menu items captions** - enable or disable captions for menu items on grid screen;
  * **Show tips** - only one tip existing is where "download" button is located. Uncheck to disable;
  * **Log mode** - save some special data to log file (rootdir\log).

### Threads ###

  * **List threads count** - thread count for gathering a pictures from pages;
  * **Threads per resource** (checkbox) - limit number of threads for each separate resource;
  * **Threads per resource**  - maximum thread count for each resource (if checkbox is marked);
  * **Pictures thread count** - thread count for picture downloading;
  * **Retries count** - how much time thread will try to download picture again after error;
  * **Speed** - maximum download speed (for whole application);
  * **Use load distribution by resources** - threads will by distributed between all resources in list (kinda queue), it will help to distribute pressure on resources. If disabled - pictures will be downloaded in order of adding to list;

### Proxy ###
Proxy settings.

### Doubles ###
Rules to filter doubles of pictures from list. Every rule working independently (like "OR" condition), and to count picture as a double must be fulfilled at last one of them. But every rule have it's own list of conditions. Conditions designer avalable to edit existing rule or create new. In it you need to point, what added picture fields (left side) should compare with gathered pictures fields (right side). Condition "url = url OR url = source" will look like this:

| url | url |
|:----|:----|
|     | source |

ie to get condition "OR" you need to leave first field empty. To get condition "url = url AND url = source) you need to put field name again instead of empty one:

| url | url |
|:----|:----|
| url | source |

For any API-based boards (like danbooru or gelbooru) is enough to create md5=md5 rule. For all other is much harder. Any way, if picture haven't a field, what should be compared, then rule will be ignored.

**resources** - there you can preset typical settings for each resource (or for all using inheriting from "general).

# Name formatting #

Using variables is not required, but it can help to name a file or distribute files by directories more clearly. In common situation is enough to chose directory to save, then by default will be used format $fname$<($fn$)>.$ext$. Default format will be used every time if after generating name is empty.


| **variable** | **description** | **example** |
|:-------------|:----------------|:------------|
| **$ext$**    | file extension  | jpeg, gif   |
| **$fname$**  | default file name (from url), without extension | b6b3a54dc0c3984e75cc1134dbc844bd5b45d145 |
| **$fn$**     | sequence number in situation, when name is already exists. Zero (0) if do not use isolation <> | name, name1, name2 |
| **$fnn`[`(N)`]`$** | sequence number inside of directory. You can dublicate number N time in a row (helpful to create branched structure) | $fnn$`_`$fname$: 1`_`name.jpg, 2`_`anothername.png<br />$fnn(2)$\$fnn$): 1\1.jpg, 1\2.jpg, 2\1.jpg |
| **$nn$**     | sequence number in list |
| **$rname$**  | resource name   | safebooru.org |
| **$rootdir$** | application root directory, without ending path delimiter "\" |             |
| **$short$**  | short resource name | sfbr, glbr, imto |
| **$tag$**    | keywords posted in "tags" field |             |
| **$tags`[`(N)`]`$** | picture's tags. N - tags count, all by default. |             |
| **%{picture's attribute}%** | attribute, obtained during the gathering | id, source, width, rating |

If variable or attribute name do not exist, then it will remain in file name.
| **example** | **result** |
|:------------|:-----------|
| c:\$bname$\$short$ %author% %id% | c:\$bname$\sfbr %author% 123456789<br />c:\$bname$\imto Gidrant 987654321 |

To avoid unwanted keywords you can isolate it using triangular brackets:

| **example** | **result** |
|:------------|:-----------|
| c:\<$bname$\>$short$< %author%> %id% | c:\sfbr 123456789<br />c:\imto Gidrant 987654321 |

Also isolation affects all symbols inside, ie you can make construction like %id%< page%page%>.$ext$.
You can isolate few names, in this case text remain if one of it can be inserted. Those, that can't be inserted, will be deleted.

Also now is possible to use display format for keys. If is a date, then will be used datetime format, for all other will be used string-number format. It sets using a colon after key name.

| **example** | **source** | **result** |
|:------------|:-----------|:-----------|
| $nn:.2x$    | 15         | 0F         |
| %posted:yyyy-mm-dd% | 31.12.2012 | 2011-12-31 |
| %width:.6d% | 1024       | 001024     |

How do you know what you need to use to achieve the desired result:
### string-number format ###
**`[`-`]``[`Width`]``[`.Precision`]`Type**
  * **Width** - minimal length of string (filled with spaces).
  * **Precision** - leading zeros for decimal (ex. 000123), back zeros for fractional numbers (ex. 1.2300), maximum length for strings.
  * **Type** - value type.
| **type** | **description** | **example** | **type** | **description** | **example** |
|:---------|:----------------|:------------|:---------|:----------------|:------------|
| **d**    | Decimal         | -123        | **e**    | Exponent        | 1.23456780000000E+004 |
| **f**    | Fixed           | 12345.68    | **g**    | General         | 12345.678   |
| **n**    | Number          | 12,345,68   | **m**    | Money           | $12,345.68 (12 345,68р.) |
| **p**    | Pointer         | 0069FC90    | **s**    | String          | Hello       |
| **u**    | Unsigned decimal | 123         | **x**    | Hexadecimal     | 8C          |

### datetime format ###
| **key** | **description** | **key** | **description** |
|:--------|:----------------|:--------|:----------------|
| **y**   | Year last 2 digits (without leading zero) | **m**   | Month number (without leading zero) |
| **yy**  | Year last 2 digits (with leading zero) | **mm**  |Month number as 2 digits |
| **yyyy** |  Year as 4 digits | **mmm** | Month using **`ShortMonthNames`** |
| **d**   | Day (without leading zero) | **mmmm** | Month using **`LongMonthNames`** |
| **dd**  | Day (with leading zero) | **h**   | Hour (without leading zero) |
| **ddd** | Month using **`ShortDayNames`** | **hh**  | Hour (with leading zero) |
| **dddd** | Month using **`LongDayNames`** | **n**   | Minutes (without leading zero) |
| **ddddd** | Day using **`ShortDateFormat`** | **nn**  | Minutes (with leading zero) |
| **dddddd** | Day using **`LongDateFormat`** | **s**   | Seconds (without leading zero) |
| **t**   | Time using **`ShortTimeFormat`** | **ss**  | Seconds (with leading zero) |
| **tt**  | Time using **`LongTimeFormat`** | **c**   | **`ShortDateFormat`** + **`LongTimeFormat`** |
| **am/pm** | Use after h : gives 12 hours + am/pm | **/**   | Substituted by **`DateSeparator`** value |
| **a/p** | Use after h : gives 12 hours + a/p | **:**   |  Substituted by **`TimeSeparator`** value |
| **ampm** | As a/p but using **`TimeAMString`**,**`TimePMString`** |         |                 |


In addition to this formatting, different from the above options are affected by the following variables with their default value (default is determined by the OS):

| **name** | **example** | **name** | **example** |
|:---------|:------------|:---------|:------------|
| **`DateSeparator`** | .           | **`TimeSeparator`** | :           |
| **`ShortDateFormat`** | dd/mm/yyyy  | **`LongDateFormat`** | dd mmm yyyy |
| **`TimeAMString`** | AM          | **`TimePMString`** | PM          |
| **`ShortTimeFormat`** | hh:nn       | **`LongTimeFormat`** | hh:nn:ss    |
| **`ShortMonthNames`** | Jan Feb ... | **`LongMonthNames`** | January, February ... |
| **`ShortDayNames`** | Sun, Mon ... | **`LongDayNames`** | Sunday, Monday ... |