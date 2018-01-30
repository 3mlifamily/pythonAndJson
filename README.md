# pythonAndJson

import json

data  = {'completed_in': 0.074,
 'max_id': 264043230692245504,
 'max_id_str': '264043230692245504',
 'next_page': '?page=2&max_id=264043230692245504&q=python&rpp=5',
 'page': 1,
 'query': 'python',
 'refresh_url': '?since_id=264043230692245504&q=python',
 'results': [{'created_at': 'Thu, 01 Nov 2012 16:36:26 +0000',
              'from_user': 'user1'
             },
             {'created_at': 'Thu, 01 Nov 2012 16:36:14 +0000',
              'from_user':'user2'
             },
             {'created_at': 'Thu, 01 Nov 2012 16:36:13 +0000',
              'from_user': 'user3'
             },
             {'created_at': 'Thu, 01 Nov 2012 16:36:07 +0000',
              'from_user': 'user4'
             },
             {'created_at': 'Thu, 01 Nov 2012 16:36:04 +0000',
              'from_user': 'user4'
             }],
 'results_per_page': 5,
 'since_id': 0,
 'since_id_str': '0'}
 
dumpStr = json.dumps(data)

pythonDict = json.loads(dumpStr)
print(pythonDict["results"][1]["created_at"])

##from pprint import pprint
##pprint(pythonDict)

