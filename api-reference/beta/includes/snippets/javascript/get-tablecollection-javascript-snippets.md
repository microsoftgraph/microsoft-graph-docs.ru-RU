---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fdefb2a5778de6499b51e4ceca4685ebc944aa3f79c3f9369eb329490f251f9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57310141"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tables = await client.api('/me/drive/items/{id}/workbook/tables')
    .version('beta')
    .get();

```