---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fd43f8014e4329dfc47c51dd49ec761ba5d96a42
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789542"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let lists = await client.api('/sites/{site-id}/lists')
    .get();

```