---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a545f3d59558d1ee5f4531016d48eaed93554f71b95cc1eb9a1401d254bed408
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57367346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sharedDriveItem = await client.api('/shares/{shareIdOrEncodedSharingUrl}')
    .version('beta')
    .get();

```