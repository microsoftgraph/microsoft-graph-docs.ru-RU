---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a717e8b7b339b042d00c43f9d258621b7a9d904e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095498"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ediscoveryReviewSetQuery = await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries/fcb86cd1-50e0-427c-840e-ba6f087364e5')
    .version('beta')
    .get();

```