---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7a752f52419f3badb0365bac9f302197f469980bbd4310271e2bc483b9da8da4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57366715"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{site-id}/contentTypes/{contentType-id}')
    .version('beta')
    .delete();

```