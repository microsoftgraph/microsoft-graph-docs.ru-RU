---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff3dbfc4626268b2ba561cd870be09f3d679ecaa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: '',
      content: 'content-value'
    },
    receivedDateTime: '2016-10-19T10:37:00Z',
    hasAttachments: true,
    from: {
      emailAddress: {
        name: 'name-value',
        address: 'address-value'
      }
    },
    sender: {
      emailAddress: {
        name: 'name-value',
        address: 'address-value'
      }
    },
    conversationThreadId: 'conversationThreadId-value',
    newParticipants: [
      {
        emailAddress: {
          name: 'name-value',
          address: 'address-value'
        }
      }
    ],
    conversationId: 'conversationId-value',
    createdDateTime: '2016-10-19T10:37:00Z',
    lastModifiedDateTime: '2016-10-19T10:37:00Z',
    changeKey: 'changeKey-value',
    categories: [
      'categories-value'
    ],
    id: 'id-value',
    inReplyTo: {
    },
    attachments: [
      {
        '@odata.type': '#microsoft.graph.fileAttachment',
        lastModifiedDateTime: '2016-10-19T10:37:00Z',
        name: 'name-value',
        contentType: 'contentType-value',
        size: 99,
        isInline: true,
        id: 'id-value'
      }
    ]
  }
};

await client.api('/groups/{id}/threads/{id}/posts/{id}/reply')
    .version('beta')
    .post(reply);

```