---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b913fde7d225ce909afdf79da76c81f26889a43942525c647416b47e506b09bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57323745"
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