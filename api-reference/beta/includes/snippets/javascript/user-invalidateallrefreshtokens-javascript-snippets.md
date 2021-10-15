---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3aec52b943eaf1abe0c0fe3a514d86b40360a01958c45f08fcf3d87ccbac9a1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271439"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/invalidateAllRefreshTokens')
    .version('beta')
    .post();

```