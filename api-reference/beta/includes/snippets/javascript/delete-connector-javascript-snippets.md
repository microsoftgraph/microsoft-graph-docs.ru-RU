---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8e8a09f75cc8bc387c3a56a026a1ce7b1ab91f5c0770797f5ff54906d5288639
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57253490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/connectors/{id}')
    .version('beta')
    .delete();

```