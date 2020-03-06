---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7365e09db16de13bd09c9248eb33da2321da980d
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversation = {
    topic:"New locations for this quarter",
    threads:[
        {
            posts:[
                {
                    body:{
                        contentType:"html",
                        content:"What do we know so far?"
                    },
                    newParticipants:[
                        {
                            emailAddress:{
                                name:"Adele Vance",
                                address:"AdeleV@contoso.onmicrosoft.com"
                            }
                        }
                    ]
                }
            ]
        }
    ]
};

let res = await client.api('/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations')
    .post(conversation);

```