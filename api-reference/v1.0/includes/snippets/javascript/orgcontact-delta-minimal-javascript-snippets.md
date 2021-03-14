---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5674f371b463a444800fdfb18aa8d4b3778253dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802756"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .header('Prefer','return=minimal')
    .select('displayName,jobTitle,mail')
    .get();

```