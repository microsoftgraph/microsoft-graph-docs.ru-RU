---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 70fcea48626fdf50ae1990571046fc20375a4ecd
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const regionalAndLanguageSettings = {
  authoringLanguages: [
    {
     locale: "en-US" },
    {
     locale: "es-MX" }
  ],
  defaultRegionalFormat: {
     locale: "en-US"
   }
};

let res = await client.api('/me/settings/regionalandlanguagesettings')
    .version('beta')
    .update(regionalAndLanguageSettings);

```