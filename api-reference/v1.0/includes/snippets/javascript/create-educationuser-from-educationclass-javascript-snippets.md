---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c55de579fe680b0a4edf6a74b6d8a5d97fa7ada
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  '@odata.id':'https://graph.microsoft.com/v1.0/education/users/13015'
};

await client.api('/education/classes/{class-id}/members/$ref')
    .post(educationUser);

```