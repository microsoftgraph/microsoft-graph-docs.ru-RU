---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bbe8c97dddb1746ef3dc0d815a3b1e80598596be
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let submissions = await client.api('/education/classes/f4a941ff-9da6-4707-ba5b-0eae93cad0b4/assignments/3c77de7f-539b-49e1-9c96-1274f2f0ee3b/submissions')
    .get();

```