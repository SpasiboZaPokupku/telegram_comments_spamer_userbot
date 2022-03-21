<h1 align="center">
Comments Spam Bot
</h1>
<p align="center">
This bot writes spam message at new post comments as fast as possible.
</p>

# Installation 
```
git clone https://github.com/plutonium777/telegram_comments_spamer_userbot.git
cd telegram_comments_spamer_userbot
pip install -r requirements.txt
python userbot.py
```
*Don't forget to configure data/config.ini file and variables in userbot.py*

# Post types
## TextPost
Syntax:
```python
spam_posts = [TextPost("text")]
```
Example:
```python
spam_posts = [TextPost("Simple text post")]
```
![](readme/TextPost.png)

Multiline example:
```python
spam_posts = [TextPost("""
This will be at first line
This will be at second line
This will be at third line
""")]
```

## PicturePost

*Image file needs to be in one directory with __userbot.py__*

Syntax:

```python
spam_posts = [PicturePost("photo", "caption")]
```
Example:
```python
spam_posts = [PicturePost("nat.jpg", "Beautiful nature! 😉")]
```
![](readme/PicturePost.png)
## StickerPost
*You can get sticker id here:* https://t.me/sticker_file_id_bot

Syntax:
```python
spam_posts = [StickerPost("sticker_id")]
```
Example:
```python
spam_posts = [StickerPost("CAACAgIAAxkBAAL6PGIzHXlhIR_MIRDTXaXz116O2Ic8AAJpAAOmysgM41g56v0Hj1wjBA")]
```
![](readme/StickerPost.png)
## RandomPost

Syntax:
```python
spam_posts = [RandomPost(posts))]
```
Example:
```python
spam_posts = [RandomPost(TextPost("Random 1"), TextPost("Random 2"))]
```
![](readme/RandomPost.png)
## MultiPost

Syntax:
```python
spam_posts = [posts]
```
Example:
```python
spam_posts = [TextPost("Some text!"), PicturePost("nat.jpg", "And a beautiful nature!")]
```
![](readme/MultiPost.png)
## DelayedPost (beta)

Syntax:
```python
spam_posts = [DelayedPost(delay(seconds), posts)]
```
Example:
```python
spam_posts = [DelayedPost(60, TextPost("This post will be sent after minute from publication."))]
```
![](readme/DelayedPost.png)
## Used Python modules
```
pyrogram
tgcrypto
```

## Have any questions ?
* Ask me on [Telegram](https://t.me/wasd_plutonium)