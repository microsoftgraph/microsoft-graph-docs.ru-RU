---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bc22be53514365e66c709098dfa2b84880a8eeac
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223488"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/administrativeUnits/{id}')
    .get();

```