---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: be36d4ce06a6c0dcd0e5c9c9e1eba3db6d6020904935d2d4a61627c297f03170
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57201666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/admin/windows/updates/deployments/{deploymentId}')
    .version('beta')
    .delete();

```