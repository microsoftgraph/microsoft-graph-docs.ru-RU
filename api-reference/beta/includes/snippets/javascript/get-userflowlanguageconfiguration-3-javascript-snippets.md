---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 824acbca0825d360d66b6fb1ef92ae95a08b33f1421a03c4ec32125aeaa4ad0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138197"
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