---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ac2a1db7e378debca721a41d2086f0b9809d70e7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  policyViolation: {
    policyTip: {
      generalText: 'This item has been blocked by the administrator.',
      complianceUrl: 'https://contoso.com/dlp-policy-page',
      matchedConditionDescriptions: ['Credit Card Number']
    },
    verdictDetails: 'AllowOverrideWithoutJustification,AllowFalsePositiveOverride',
    dlpAction: 'BlockAccess'
  }
};

await client.api('/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19:a21b0b0c05194ebc9e30000000000f61@thread.skype')
    .version('beta')
    .update(chatMessage);

```