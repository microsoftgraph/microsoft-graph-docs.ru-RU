---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4283007ec3de590c42f069d5effac4763319d5b75583d967dbf86c3ec62c116b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052099"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let longRunningOperation = await client.api('/users/{id | userPrincipalName}/authentication/operations/{id}')
    .version('beta')
    .get();

```