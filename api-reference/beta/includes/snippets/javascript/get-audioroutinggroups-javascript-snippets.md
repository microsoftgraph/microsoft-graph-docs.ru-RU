---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 089b160f46c07975d4d1f0875e3b7fa0b4529cb3dfc902d85f7c8be21e8f5790
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57361222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let audioRoutingGroups = await client.api('/communications/calls/{id}/audioRoutingGroups')
    .version('beta')
    .get();

```