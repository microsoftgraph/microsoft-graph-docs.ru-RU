---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9026bfdeaf41f3941726b1d694c0002679fd67d1360813fea2f81d700f76eee6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57270797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .post();

```