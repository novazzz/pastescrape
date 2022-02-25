# pastescrape
`pastescrape` is a simple script to regularly read recent, public pastes on pastebin and save anything interesting.

### Why?
Simple curiosity. Lots of interesting things get posted to PasteBin, from drug dealer's menus to malware. I am interested in documenting and recording the interesting things that would otherwise go unnoticed.

### Installation and Setup
1. Run `gh repo clone pastescrape`.

2. Run `python pastescrape.py` once to generate config file.

3. Configure `config.conf`, a sample is provided. Keywords are **not** case sensitive. You must provide absolute paths. Pastescrape will **not** create the directories for you, and it will not run without them.

4. Run `python pastescrape.py` once manually to make sure everything is configured correctly.

5. Schedule it to run automatically with a cronjob. Scheduling it for every 5-6 hours should be plenty, and the longer you wait the less likely you are to get blocked.

6. (Optional) cd to the `saved` directory and run `python -m http.server 80`. This allows you to type your devices ip anywhere on your network and see the saved pastes.

### Todo
Store parsed saves better?
