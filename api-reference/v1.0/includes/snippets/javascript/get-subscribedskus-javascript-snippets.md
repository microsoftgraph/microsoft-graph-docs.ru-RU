---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ccdc3591476f892df0208d866cfb549a6b95123df2e2c87ebfd41d027235cb65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57430354"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscribedSkus = await client.api('/subscribedSkus')
    .get();

```