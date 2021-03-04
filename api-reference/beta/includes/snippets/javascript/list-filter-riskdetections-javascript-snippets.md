---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 88049981d37e9cdcbb71d0b4fe1452cd337946d3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProtection/riskDetections')
    .version('beta')
    .filter('riskEventType eq \'unfamiliarFeatures\' or riskLevel eq \'medium\'')
    .get();

```