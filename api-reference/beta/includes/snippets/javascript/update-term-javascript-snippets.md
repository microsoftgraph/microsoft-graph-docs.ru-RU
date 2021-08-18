---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 85841ef9d9cad8ea0d3c6a3f7db90ca75fe3e64794f0ad3e769aa79b349f172a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138225"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const term = {
  labels: [
      {
          name: 'changedLabel',
          languageTag: 'en-US',
          isDefault: true
      }
  ]
};

await client.api('/termStore/sets/{setId}/terms/{termId}')
    .version('beta')
    .update(term);

```