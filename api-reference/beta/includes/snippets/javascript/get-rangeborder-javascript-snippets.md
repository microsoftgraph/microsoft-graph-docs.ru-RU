---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e25b560bde23c105d3f33bfc7df34c4d415d7460b68d786fea3e8d96c3b3f82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141722"
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