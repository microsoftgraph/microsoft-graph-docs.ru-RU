---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a04cbbbc30b6a6246868e409c6be4c659744b25
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)')
    .version('beta')
    .get();

```