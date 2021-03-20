---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bdbb925d6ec1bb3901bf07bce878653a7920fd22
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952014"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childTags = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/e54b3f535b434a9a8743b84e34c00504/childTags')
    .version('beta')
    .get();

```