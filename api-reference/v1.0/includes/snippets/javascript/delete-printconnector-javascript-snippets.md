---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c37567a28a3ad72be0ccb861d6dc45f2519c11ef0179f5f21c9147267a1ccfeb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57250846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/connectors/{printConnectorId}')
    .delete();

```