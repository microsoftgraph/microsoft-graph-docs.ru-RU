---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b16cd9490738328b6486e73385f06d5385f3abf
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507442"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let team = await client.api('/teams/893075dd-2487-4122-925f-022c42e20265')
    .version('beta')
    .get();

```