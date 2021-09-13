---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: edd065683696abfe3f0d69e744543e46509ecc721c3809abdb0ceef436b36d17
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57197290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/entireRow')
    .get();

```