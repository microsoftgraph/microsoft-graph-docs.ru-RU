---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b076dc27d99fe78766cd817db192d31dec2605fbe6ad37d0a3a188640df8945d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57142102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connector = await client.api('/onPremisesPublishingProfiles/applicationProxy/connectors/{id}')
    .version('beta')
    .get();

```