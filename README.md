# Blood-on-the-Clocktower-cards
This repo contains formatted game cards for blood on the clocktower with card generation code. The character portraits are generated using Chatgpt4 (DALL.E 3). The prompts are simple, just ask Chatgpt to create character portraits for a card game in pixel art style like 90s video game, with medieval fantasy world setting. The generated card fronts are stored in '''Fronts/'''

## Card size
Standard boardgame size, 63mm*88mm
## Resolution
The default resolution of Chatgpt generated images are 1024 by 1024 pixels with .webp extension. These source portraits are stored in corresponding folders and then converted to jpg using Python PIL. The final card resolution should be 816 by 1110 pixels.
## Code composition
The code is formed by 3 parts. Once you have all portraits in their corresponding files, a web scrapper written using beautifulsoup will scrap corresponding character description and motto from the official wiki page. Then, portraits, description and motto texts will be added to the blank card front to form initial 1024 by 1024 card. This card is then croped and resized to proper size. Thus, if you would like to add your customized characters and card fronts, you will need to change the scrapper and image postprocess parts correspondingly. Use photoshop to first generate a sample would be helpful for writing automation code.
