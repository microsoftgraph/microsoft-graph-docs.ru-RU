---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f78db3906614376f0dfb2a87affa67b368c4a0ed17510a22d4b9c329da27d7c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57211838"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  ids: [
    '80a963dd-84af-4eb8-b2a6-781e444d4fb0',
    '62e90394-69f5-4237-9190-012177145e10',
    '86a64f51-3a64-4cc6-a8c8-6b8f000c0f52',
    'ac38546e-ddf3-437a-ac5c-27a94cd7a0f1'
  ]
};

await client.api('/me/checkMemberObjects')
    .post(string);

```