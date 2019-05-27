---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a1d7ec71ec175b4717532b5774ca3397b51dc0d7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const closeSession = {

};

let res = await client.api('/me/drive/items/{id}/workbook/closeSession')
    .post(closeSession);

```