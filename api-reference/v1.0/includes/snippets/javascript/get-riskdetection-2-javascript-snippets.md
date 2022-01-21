---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 50c9114ddb388d0a3bec86135b62bea755f60893
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122058"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskDetections = await client.api('/identityProtection/riskDetections')
    .get();

```