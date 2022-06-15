---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 281a74681e7ec621e5ea9b1be8dc7a0eabc7cfdb
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let caseOperation = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/operations/850c2f64b1ee44a4a69729327aac2b04')
    .version('beta')
    .get();

```