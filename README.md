# About
Automated Discord notifications when cicada3301's websites are updated.

Uses very little RAM (maybe a megabyte) and is not CPU-intensive. Network requests are made as often as configured.

# How to set up
1. Clone this repository.
```
git clone https://github.com/Arinerron/discord3301/
```

2. Copy the file `Config.java.example` to `Config.java`
3. Paste your notification endpoint from Discord between the quotation marks in the variable `DISCORD_URL`.
4. Save the file. You're ready to run the bot now.
5. To run the bot, execute `sh run.sh` on any linux system with bash. If you don't have bash, just execute the following...
```
javac Main.java
java Main
```
6. If you'd like to change how often a site is checked, or add a new site to be checked, simply edit the file `sites.txt`.

# Debugging
Getting an error similar to this?

```
Main.java:125: error: cannot find symbol
            URL url = new URL(Config.DISCORD_URL);
                              ^
  symbol:   variable Config
  location: class Main
2 errors
```

That means you forgot to configure the file `Config.java`, or the file `Config.java` does not exist
