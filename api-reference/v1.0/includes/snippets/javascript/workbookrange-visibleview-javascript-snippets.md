---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ecf28ce5182132fe0074b30a84ced9f3c9429b5d7415ff1fd7965bfb32c7777b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRangeView = await client.api('/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView')
    .get();

```