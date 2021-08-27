---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d923171853dc7e9e657720eb1ad54400b639db65486db48251d1c67d654456a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57432106"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .get();

```