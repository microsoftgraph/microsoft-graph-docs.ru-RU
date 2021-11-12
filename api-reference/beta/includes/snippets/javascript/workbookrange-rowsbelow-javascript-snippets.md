---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 988255c42a46308f15e980045ee0702201b5650f3a24494826f9868c85e89487
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57316297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)')
    .version('beta')
    .get();

```