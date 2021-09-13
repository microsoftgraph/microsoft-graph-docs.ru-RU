---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9681feded4375aca1ccde07feaa975d935bbfc18cda6be32aba41ea36fe3f80f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57262186"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/connections/contosohr')
    .delete();

```