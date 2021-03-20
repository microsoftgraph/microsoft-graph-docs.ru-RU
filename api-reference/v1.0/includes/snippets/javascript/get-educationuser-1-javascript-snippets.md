---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9c7052f801bc84da364b906583fce7a93629ef4e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/education/me/user')
    .get();

```