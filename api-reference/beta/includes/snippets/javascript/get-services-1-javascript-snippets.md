---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 524e16f28de85049950f5d53f3674afc162f823f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let services = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services')
    .version('beta')
    .get();

```