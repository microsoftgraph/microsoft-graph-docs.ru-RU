---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: faf225b9ebb59f972e476861aded65c42708d3ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774196"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAnnotation = {
  allowedAudiences: 'organization'
};

await client.api('/users/{userId}/profile/notes/{id}')
    .version('beta')
    .update(personAnnotation);

```