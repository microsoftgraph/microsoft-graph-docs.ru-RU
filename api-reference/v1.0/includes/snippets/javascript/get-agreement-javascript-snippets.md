---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 86502b0e6eda123ec914bace90c6c80622accd20
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreement = await client.api('/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be')
    .expand('files')
    .get();

```