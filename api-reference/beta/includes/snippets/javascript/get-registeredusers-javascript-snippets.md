---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8fb3d8a7c8ff1db6ef5c3cb5494f5b41279e510bc90b0dab55b5cdd052aefba2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57212278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredUsers = await client.api('/devices/{id}/registeredUsers')
    .version('beta')
    .get();

```