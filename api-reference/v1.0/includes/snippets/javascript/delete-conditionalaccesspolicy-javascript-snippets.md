---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 205d062b9f2119313f1e9e05ccf685068b777c35001ecf6ddea8a6381c142850
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57365066"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/conditionalAccess/policies/{id}')
    .delete();

```