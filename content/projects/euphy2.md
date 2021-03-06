+++
title = "Euphy2 Tutorial"
date = 2021-02-18T21:19:15.788Z
description = "Tutorial on Euphy2 usage"
tags = ["euphy2"]
showToc = false
+++
<!--more-->
# Table of Contents {#top}

0. [Foreword: Style and arguments][1]

1. [Modifying user information][2]
    - [Setting names: `names`][3]
    - [Setting pronouns: `pronouns`][4]
    - [Deleting info: `delete`][5]
2. [Accessing the pronoun database][6]
    - [Contributing new pronoun sets: `contribute`][7]
    - [Querying database][8]
3. [Trying names and pronouns: `try`][9]
    - [Specifying names and pronouns manually][10]
4. [Miscellaneous][11]

[1]:{{<relref "#foreword">}}
[2]:{{<relref "#usersettings">}}
[3]:{{<relref "#setnames">}}
[4]:{{<relref "#setpronouns">}}
[5]:{{<relref "#deletesettings">}}
[6]:{{<relref "#pronoundb">}}
[7]:{{<relref "#contribute">}}
[8]:{{<relref "#query">}}
[9]:{{<relref "#trynamespronouns">}}
[10]:{{<relref "#specifynamespronouns">}}
[11]:{{<relref "#miscellaneous">}}



> ### Note
> 
> Any text that has a dotted line under it like {{<infobox "Hey there!">}}this{{</infobox>}} can be hovered over for further explanation. This is useful for technical terms that would be familiar to people from a technology background, but would require too much explanation in the text to be smooth for new readers. Keep an eye out for any unfamiliar language!


## {{< totop >}} 0. Foreword: Style and arguments {{</ totop >}} {#foreword}

In the following tutorial, it is assumed that every command is prefixed by `e$`. For example, if a section below were to read:
> Users may use `names` to modify their stored names.

It should be assumed that the actual bot will be used by typing `e$names`. This is done for ease of reading in the tutorial.

Commands that take {{<infobox "Information passed to a command">}}arguments{{</infobox>}} will be notated in the following way:
```
e$command-name required-argument [optional-argument] option-1|option-2
```
Required arguments must be included in the command to run successfully, and optional arguments don't have to be included for the bot to handle the command properly, or they may only be required under certain circumstances. The vertical bar (|) indicates choice from a set of options.

For example, `try` takes two sets of arguments, and would be notated in the following way:
```
e$try [pronoun-1/pronoun-2/.../pronoun-m] [name-1, name-2,..., name-n]
```
This indicates that both the pronoun and name arguments are optional (with [some caveats]({{< relref "#try" >}})). Further, an indefinite amount of arguments may be specified for each, indicated by the {{<infobox "...">}}ellipsis{{</infobox>}}.

## {{< totop >}} 1. Modifying user information {{</ totop >}} {#usersettings}

Euphy2 has three different commands that can be used to control the information Euphy2 has on a user. These are `names`, `pronouns`, and `delete`.

### {{% totop %}} Setting names: `names` {{%/ totop %}} {#setnames}

`names` has the following syntax:
```
e$names [name-1, name-2, ...]
```
When called with no arguments, Euphy2 will send a list of any names you have set for yourself before:

![e$names with no arguments](/img/euphy2/names_no_args.png)

When called with a comma-separated list (like `name 1, name 2, name 3`), the bot will set the names it has stored for you to all of the names you input:

![e$names with arguments](/img/euphy2/names_with_args.png)

The names you set will be selected from randomly [when using `try`][9].

### {{% totop %}} Setting pronouns: `pronouns` {{%/ totop %}} {#setpronouns}

`pronouns` works almost identically to `names`:
```
e$pronouns [pronoun-1/pronoun-2/pronoun-3/...]
```
the only differences being that slashes delineate pronouns (as is common, especially on the Internet), and that of course this modifies what pronouns are stored rather than names. 

You only need provide one pronoun from each set you would like to use (e.g., you only need to input `she/they` instead of `she/her/hers/they/them/theirs`, etc.), __except in the case where you only want to use one set of pronouns__, in which case you will need to provide two. For example, if your pronouns were `he/him/his`, you would need to enter `e$pronouns he/him` or `e$pronouns he/him/his` instead of `e$pronouns he`.

![e$pronouns with arguments](/img/euphy2/pronouns_with_args.png)

### {{% totop %}} Deleting info: `delete` {{%/ totop %}} {#deletesettings}

## {{< totop >}} 2. Accessing the pronoun database {{</ totop>}} {#pronoundb}
### {{% totop %}} Contributing new pronoun sets: `contribute` {{%/ totop %}} {#contribute}
### {{% totop %}} Querying database {{%/ totop %}} {#query}

## {{< totop >}} 3. Trying names and pronouns {{</ totop >}} {#trynamespronouns}
### {{< totop >}} Specifying names and pronouns manually {{</ totop >}} {#specifynamespronouns}

## {{<totop>}} 4. Miscellaneous {{</totop>}} {#miscellaneous}