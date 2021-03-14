---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b7c7b9f7c0acc833777ee6070645fde1e87dfb6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeBorder = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}')
    .get();

```