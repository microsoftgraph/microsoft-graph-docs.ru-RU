---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d4ef07d5b700d3485b889aec4219d509e49f721a87aa62f3146172caaab340f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57431293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
    displayName: 'Seattle District Technical Schools',
    description: 'Seattle district technical schools administration',
    visibility: 'HiddenMembership'
};

await client.api('/directory/administrativeUnits')
    .post(administrativeUnit);

```