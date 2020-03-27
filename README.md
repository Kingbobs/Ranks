# Ranks
# commands:
 srank:
  description: "Sets a player rank"
  usage: "/srank <player> <rank>"
  permission: "customranks.command.srank"
 lrank:
  description: "Lists the existing ranks"
  usage: "/lrank"
  permission: "customranks.command.lrank"

# permissions:
 customranks:
  default: op
  description: "Allows using all the CustomRanks things"
  children:
   customranks.command:
    default: op
    description: "Allows using all the CustomRanks commands"
    children:
     customranks.command.srank:
      default: op
      description: "Allows setting a player rank"
     customranks.command.lrank:
      default: true #allowed for everyone
      description: "Allows listing the existing ranks"
