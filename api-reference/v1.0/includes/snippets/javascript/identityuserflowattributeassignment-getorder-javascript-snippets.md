---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e64b1c46e4d95a91a473e0c1ba1e2d159da216e3d4f164f4eea20b05164e9347
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57432625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignmentOrder = await client.api('/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/getOrder')
    .get();

```