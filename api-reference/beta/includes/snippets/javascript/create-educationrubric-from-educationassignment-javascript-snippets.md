---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aa0ab4efa14b62d8abb8afc1a6d8ed262fa15e7b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785336"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/education/me/rubrics/{id}'
};

await client.api('/education/classes/{id}/assignments/{id}/rubric/$ref')
    .version('beta')
    .put(educationRubric);

```