---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 713da3766f0f246d844ed21581d5ba4d953700a074c94a1c75a2602649008c56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57192019"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attachments = await client.api('/users/{id}/outlook/tasks/{id}/attachments')
    .version('beta')
    .get();

```