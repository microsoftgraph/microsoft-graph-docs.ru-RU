---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9c17aca5b12a8e7cba4b311c10491f1cf9883ca6f9c8a006475e13583fc8cbf5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57316397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskDetections = await client.api('/identityProtection/riskDetections')
    .version('beta')
    .filter('riskEventType eq \'unfamiliarFeatures\' or riskLevel eq \'medium\'')
    .get();

```