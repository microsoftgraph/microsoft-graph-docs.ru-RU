---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8fee14203b7c878bb311818e4451bf7d3dcb2f6c
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719704"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let operations = await client.api('/sites/root/operations')
    .get();

```