# Koubotto
Koubotto is the Anime UC!'s custom made discord bot

# Table of Contents
- [Events](#Events)
    - [Adding Events](#adding-events-addevent-name-date)
    - [Removing Events](#removing-events-removeevent-id)
    - [Editing Events](#editing-events-editevent-id-name-date)
    - [Viewing Calendar](#viewing-calendar)
- [Counting Game](#counting-game)
    - [Setting Channel](#setting-counting-game-channel-countingchannel-channel)
    - [Next Number](#checking-next-number)
    - [Highscore](#checking-highscore)
    - [Lifetime Stats](#checking-lifetime-stats)
- [Economy (Maybe...)]()

# Usage
## Available Commands
The following commands can be used by any user in the server

![help](https://raw.githubusercontent.com/BeastieNate5/Koubotto/refs/heads/main/img/help.png)

The following commands can only be used by admins in the server

![admin_help](https://raw.githubusercontent.com/BeastieNate5/Koubotto/refs/heads/main/img/admin_help.png)

## Events
Koubotto has a calender system where you can view, add, edit, or remove events

### Adding Events `/add_event <name> <date>`
```
/add_event Meeting 1733504400
```
This will create a named event on the calendar with a event ID. The date must be in epoch format. You can use the following [converter](https://www.unixtimestamp.com) to convert human readable date to epoch time

### Removing Events `/remove_event <ID>`
```
/remove_event 312
```
The ID can be retrieved from `/calendar`

### Editing Events `/edit_event <ID> <name?> <date?>`
```
/edit_event 312 Game night 1733505400
```
Both `name` and `date` are optional. You are able to edit the name and date separately, or you can do both in one command

### Viewing Calendar
```
/calendar
```

![calendar_out](https://raw.githubusercontent.com/BeastieNate5/Koubotto/refs/heads/main/img/calendar_out.png)

The following is the sample output of `/calendar`. The `(919)` is the event ID which is needed to use `/remove_event` and `/edit_event`


## Counting Game
Koubotto has a counting game where members of the server goal is to count from 0 to infinity correctly. Each correct number is a point.

### Setting counting game channel `/counting_channel <channel>`
```
/counting_channel #counting
```

### Checking next number
```
/next_number
```

### Checking highscore
```
/counting_highscore
```

### Checking lifetime stats
```
/counting_stats
```