---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cd4e28162260a8056e2f0330cc71eaf05c8f81ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/permissionGrantPolicies/my-custom-consent-policy')
    .delete();

```