---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b5c566a77e633fb1b265a7ea7dc6476439793c3a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applicationSignInDetailedSummary = await client.api('/reports/applicationSignInDetailedSummary')
    .version('beta')
    .get();

```