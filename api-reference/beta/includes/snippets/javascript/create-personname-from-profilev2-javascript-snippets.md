---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 06ef5a8042cd61d10749214ecb623c5a8a2f94ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798629"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personName = {
  displayName: 'Innocenty Popov',
  first: 'Innocenty',
  initials: 'IP',
  last: 'Popov',
  languageTag: 'en-US',
  maiden: null
};

await client.api('/me/profile/names')
    .version('beta')
    .post(personName);

```