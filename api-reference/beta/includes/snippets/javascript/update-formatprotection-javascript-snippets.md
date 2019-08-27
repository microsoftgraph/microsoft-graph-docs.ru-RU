---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 31b2e206c60e54ad46ae64c87654bb0cfeb0a6e9
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638187"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookFormatProtection = {
  locked: true,
  formulaHidden: true
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/protection')
    .version('beta')
    .update(workbookFormatProtection);

```