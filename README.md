import urllib
import json 
import string
import sys

token = "cd61a19c72bc0773bc933a70edde8d1f"
githubURL = "https://github.com/taviana/new2040"

data = urllib.urlencode({"token": token, "github": githubURL})

url = "http://challenge.code2040.org/api/register"

conn = urllib.urlopen(url, data)

print conn.read()
