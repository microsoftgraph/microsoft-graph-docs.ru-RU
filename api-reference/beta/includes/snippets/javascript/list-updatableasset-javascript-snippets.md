---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 241b3cb5bf0135d5e9ffafc3280f37253ef38f96
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668711"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/admin/windows/updates/deployments/{deploymentId}/audience/members')
    .version('beta')
    .get();

```