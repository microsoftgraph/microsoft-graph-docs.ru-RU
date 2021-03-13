---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 63cb20304b7643f0e3aed6ce3f0e230355070403
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationUser = {
  displayName: 'Rogelio Cazares',
  givenName: 'Rogelio',
  middleName: 'Fernando',
  surname: 'Cazares',
};

await client.api('/education/users/13020')
    .version('beta')
    .update(educationUser);

```