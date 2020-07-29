---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6986ef5e892ec710968df911daf33ea055256c0c
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemInsights = {
  disabledForGroup: "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
};

let res = await client.api('/organization/{organizationId}/settings/itemInsights')
    .version('beta')
    .update(itemInsights);

```