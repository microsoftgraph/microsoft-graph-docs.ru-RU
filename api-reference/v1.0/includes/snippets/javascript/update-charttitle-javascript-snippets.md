---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b69b9aa14ecfb6c20cb37054fe80ef39c5ede7128ed90b2e80072bec2c0ab16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57372455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartTitle = {
  overlay: true,
  text: 'text-value',
  visible: true
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title')
    .update(workbookChartTitle);

```