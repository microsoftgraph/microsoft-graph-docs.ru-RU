---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5b0c6b3dbae9441c559088c37476b0a14f02cdce9bd61bc416d5dff6778bed4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57394034"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setPosition = {
  startCell: 'startCell-value',
  endCell: 'endCell-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition')
    .version('beta')
    .post(setPosition);

```