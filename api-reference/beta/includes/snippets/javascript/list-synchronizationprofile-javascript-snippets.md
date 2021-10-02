---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5c70b7eeca1e57acf1a12e3068efc96a106b0e911b0663d94ee75a1de63846cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57310534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let synchronizationProfiles = await client.api('/education/synchronizationProfiles')
    .version('beta')
    .get();

```