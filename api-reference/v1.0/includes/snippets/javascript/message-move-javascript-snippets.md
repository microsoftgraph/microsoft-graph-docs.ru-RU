---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 09607d2c1fafb713510f5060019bdaee8cd075699b2874739ff024c67da1f9fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57206779"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  destinationId: 'deleteditems'
};

await client.api('/me/messages/AAMkADhAAATs28OAAA=/move')
    .post(message);

```