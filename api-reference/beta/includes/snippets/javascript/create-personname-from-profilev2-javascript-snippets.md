---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 471a857cd0f3141d61977ff3f8f90c1f0766779f
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821240"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personName = {
  displayName: "Innocenty Popov",
  first: "Innocenty",
  initials: "IP",
  last: "Popov",
  languageTag: "en-US",
  maiden: null
};

let res = await client.api('/me/profile/names')
    .version('beta')
    .post(personName);

```