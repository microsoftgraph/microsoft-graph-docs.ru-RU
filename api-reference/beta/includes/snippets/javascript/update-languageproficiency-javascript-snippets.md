---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 49dfe9f666b239765be618dfe62893a42d4e1d44441f81b9f4e2530b611dbf88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140785"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const languageProficiency = {
  allowedAudiences: 'organization'
};

await client.api('/me/profile/languages/{id}')
    .version('beta')
    .update(languageProficiency);

```