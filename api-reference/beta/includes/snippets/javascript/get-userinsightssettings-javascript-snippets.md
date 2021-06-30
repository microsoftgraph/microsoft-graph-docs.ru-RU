---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c28604f8adb57b0a35aaf52a47cb242c59bfa7a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userInsightsSettings = await client.api('/me/settings/itemInsights')
    .version('beta')
    .get();

```