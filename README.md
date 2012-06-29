# `reload` for Firefox glci

This gcli command allows one to reload things in the page, without reloading all
the page.

# Synopsis
```sh
reload what [when]
```

`what` can be:
- `page`: reload the page ;
- `images`: reload the `img` ;
- `media`: reload the `<audio>` and `<video>` ;
- `css`: reload the `<link rel=stylesheet>`.

`when` is optional, and is composed of a number and a unit:
- `1s`: reload the thing specified before every second ;
- `4min`: -- every four minutes ;
- `4h`: -- every four hours ;
- `1day`: -- every day ;
- `stop`: stop reloading something that was reloading periodically.

# Possible improvements
- Reload multiple things in one command. How to cancel when reloading
  periodically?
- Allow one to reload more things. Maybe allow to pass in a selector?
- Avoid crashing the browser (see <https://bugzilla.mozilla.org/show_bug.cgi?id=768706>).

# License
- MPL2
