import urllib
import json 
import string
import sys

token = sys.argv[1]
githubURL = "https://github.com/taviana/new2040"

data = urllib.urlencode({"token": token, "github": githubURL})

url = "http://challenge.code2040.org/api/register"

conn = urllib.urlopen(url, data)

print conn.read()
