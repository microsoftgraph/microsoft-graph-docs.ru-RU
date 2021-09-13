---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9e525372b0c683063d04d364a0e3014202f1dd7475d8132c8de54ed9132fe543
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57323269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/applications/delta')
    .get();

```