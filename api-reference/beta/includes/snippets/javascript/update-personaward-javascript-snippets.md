---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 43126c07061b78c91e494826f5aa58638d6870369dfa32f432dc9503089beaec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57362807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAward = {
  issuingAuthority: 'International Association of Branding Management',
  thumbnailUrl: 'https://iabm.io/sdhdfhsdhshsd.jpg'
};

await client.api('/users/{userId}/profile/awards/{personAwardId}')
    .version('beta')
    .update(personAward);

```