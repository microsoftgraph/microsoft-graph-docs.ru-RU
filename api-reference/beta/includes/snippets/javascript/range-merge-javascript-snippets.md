---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c5d4667583590dce89d4963cb38977d19b5eeeb5d0bcd7e8e260ef5b9f7cc103
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252052"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const merge = {
  across: true
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/merge')
    .version('beta')
    .post(merge);

```