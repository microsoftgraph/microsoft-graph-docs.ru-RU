---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 60cc29e140949ff21df897a55db6843cc27c4754
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794681"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let scopedRoleMembers = await client.api('/administrativeUnits/{id}/scopedRoleMembers')
    .version('beta')
    .get();

```