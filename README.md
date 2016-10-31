# new2040
import json 
import requests

json_data = {
  "token" = "cd61a19c72bc0773bc933a70edde8d1f"
  "github" = "https://github.com/taviana/new2040"
  }
  
r = requests.post("http://challenge.code2040.org/api/register")
