---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b9b830f292dfba68dcf7300c068149d81d9ac40bdbd8acc9b80341a61591d37c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57370699"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange')
    .post();

```