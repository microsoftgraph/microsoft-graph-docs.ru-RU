---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0348d894c3a3a4b45cdcf1beaddc1c4702de0322b4cedac59d8a94a093c54293
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/me/getMemberObjects')
    .post(string);

```