---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 28782297c2e9a719f5cbc31b7f2d9f129eb6450e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488724"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .version('beta')
    .filter('MentionsPreview/IsMentioned eq true,')
    .select('subject,sender,receivedDateTime,mentionsPreview')
    .get();

```