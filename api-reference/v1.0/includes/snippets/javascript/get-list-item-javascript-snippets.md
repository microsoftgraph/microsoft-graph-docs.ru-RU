---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8c64f8c1569faece90be9a139f520cc65e03c5589ce190a8bc9152fbb50f2e16
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let listItem = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields')
    .get();

```