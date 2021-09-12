---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 397db10f3753ce55059e0a23f1e989a23a49b1fdbfbc57245019d7f949287a2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let shiftPreferences = await client.api('/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences')
    .get();

```