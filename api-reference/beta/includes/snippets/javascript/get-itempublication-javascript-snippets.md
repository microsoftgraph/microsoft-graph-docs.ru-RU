---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b4b58130f0ecbbd314ded357dd7567e1848ea0f3b48bc3fc873c84e0e9abbca6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322572"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemPublication = await client.api('/me/profile/publications/{id}')
    .version('beta')
    .get();

```