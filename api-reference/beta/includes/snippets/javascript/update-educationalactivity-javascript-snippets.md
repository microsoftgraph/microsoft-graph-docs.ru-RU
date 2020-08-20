---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2fd9271d915901bd5e13b833514a89cd6ed86842
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821147"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationalActivity = {
  institution: {
    location: {
      type: "business",
      postOfficeBox: null,
      street: "12000 E Prospect Rd",
      city: "Fort Collins",
      state: "Colorado",
      countryOrRegion: "USA",
      postalCode: "80525"
    }
  }
};

let res = await client.api('/me/profile/educationalActivities/{id}')
    .version('beta')
    .update(educationalActivity);

```