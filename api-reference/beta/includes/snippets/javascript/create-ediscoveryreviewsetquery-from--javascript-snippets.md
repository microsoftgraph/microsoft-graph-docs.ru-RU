---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68f17e0d69a30235337d1466ca29acd80314377f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryReviewSetQuery = {
    displayName: 'My Query 1',
    contentQuery: '(Author=\"edison\")'
};

await client.api('/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries')
    .version('beta')
    .post(ediscoveryReviewSetQuery);

```