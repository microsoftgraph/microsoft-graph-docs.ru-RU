---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6a5816cd6b48a8b9b7b67cac7983578b18164ce
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696365"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authoredNote = {
content: 
  {
    content: 'String',
    contentType: 'text'
  }
};

await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes')
    .post(authoredNote);

```