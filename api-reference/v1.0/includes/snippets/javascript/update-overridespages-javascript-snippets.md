---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9fba54f6b61467db7a4609b689fdd6cf84dc6f36509d34fbf72845b6b31f5be5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57250580"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = {
LocalizedStrings: [
      {
          ElementType: 'UxElement',
          ElementId: null,
          StringId: 'alert_message',
          Override: true,
          Value: 'Are you sure that you want to cancel entering your information?'
      }
  ]
};

await client.api('/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value')
    .put(stream);

```