---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f073ed4d3d331b9848cc72c7715e3bdaf627b2e2e3d42085a5e3025e44db892f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let search = await client.api('/me/drive/search(q='Contoso Project')')
    .get();

```