---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 42152872820754ce42c87b0ae34aeaea04f80c66
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783429"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeBorder = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}')
    .version('beta')
    .get();

```