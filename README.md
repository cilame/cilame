```python
zstring = (
'JZHdcoIwEEbveWrUiooWxPKjolbFsaCiqKNG1PIwzW6Sq75ClzLDRch+5+wmwbaDjbMKY6'
'UbeKlB3+HM1MCJZb6VhYWPBQZz9DJkCY59DAJgk99nj9+HYqqryMLLBod17Ow0zqwqCrdY'
'nRiZYJWIJJdFDb5HJfN84vDAXzZMYtm8c5ZCZvM850xX4ybxLvR3VCO4KqtaIIv7j16DRU'
'+NbmAZYJ9oX4zfZNNVLNIwXWFwJTfsG5hGBAs3BjMsOzRYqXh+QCvHzIVwqYHVpR/lFfSR'
'g+cODHrVzGK6wOWaALncygGjGAUgnEFhwKStge2o5oX6SIPEetlwElfHIwazFWYnwtTa1l'
'Q94nlIGujPOOuSpsTGnoo+aY1+C4cWjQ3tB2XQDHEwKMeuRJc9MqZh8MWZL7weAWJpiU6L'
'vyx5SEVSyKtZjn2sE8Nfc6mfhedSCd4LTR6O/7f5jn6KD4ceAG9HZCasNqT/Aw=='
)

# len(zstring): 484
import base64, zlib
zstring = base64.b64decode(zstring)
zstring = zlib.decompress(zstring,-15)
string = zstring.decode("utf-8")
print(string)
```
