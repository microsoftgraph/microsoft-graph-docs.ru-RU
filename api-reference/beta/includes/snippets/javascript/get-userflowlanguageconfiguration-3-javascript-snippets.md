---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a4bef15ceb0f0d4d045d6dd1572f7956981c5e70
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955256"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowLanguageConfiguration = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en')
    .version('beta')
    .get();

```