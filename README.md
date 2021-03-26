# eml2mbox

Updates to the [eml2mbox script](https://www.broobles.com/eml2mbox/).

## Usage

```
Usage: [ruby] eml2mbx.rb [-c] [-l] [-s] [-yz] [emlpath [trgtmbx]]
         Switches:
            -c Remove CRs (^M) appearing at end of lines (Unix)
            -l Remove LFs appearing at beggining of lines (old Mac) - not tested
            -s Don't use standard mbox postmark formatting (for From_ line)
               This will force the use of original From and Date found in mail headers.
               Not recommended, unless you really have problems importing emls.
           -yz Use this to force the order of the year and timezone in date in the From_
               line from the default [timezone][year] to [year][timezone].
         emlpath - Path of dir with eml files. Defaults to the current dir if not specified
         trgtmbx - Name of the target mbox file. Defaults to "archive.mbox" in 'emlpath'
```

## Resources

Additional documentation can be found [on the wiki][man].

Discussion and paches are welcome and should be directed to my public
inbox: [~mjorgensen@lists.sr.ht][lists]. Please use `--subjecct-prefix
PATCH eml2mbox` for clarity when sending patches.

Bugs and issues are tracked in the tracker: [~mjorgensen/eml2mbox][todo].

[man]:https://man.sr.ht/~mjorgensen/eml2mbox
[lists]:https://lists.sr.ht/~mjorgensen/public-inbox
[todo]:https://todo.sr.ht/~mjorgensen/eml2mbox