---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b70ef455bf056d45b78dfee30c8e10977d8c61eb814c0a54d998e9bd7ffac225
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144611"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columnDefinition = await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}')
    .version('beta')
    .get();

```