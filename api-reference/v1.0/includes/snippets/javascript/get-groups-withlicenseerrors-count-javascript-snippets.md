---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 477c64c509e57dbcb4fefee332fcb3fa2291885b3b8b963cc9480025dd719f50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57256893"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .header('ConsistencyLevel','eventual')
    .filter('hasMembersWithLicenseErrors eq true')
    .select('id,displayName')
    .get();

```