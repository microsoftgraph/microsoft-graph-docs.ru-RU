---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8dc193b38af873c913ec5acc009adefa6e6808b140b8358b9516d1fb49dc7bed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144177"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
  shift: 'shift-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/insert')
    .post(workbookRange);

```