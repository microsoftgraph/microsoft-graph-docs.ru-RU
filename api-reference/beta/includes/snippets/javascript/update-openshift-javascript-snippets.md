---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c2c79fb0100a52e953fdd1fa6304a55d1a04414f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786876"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const openShift = {
schedulingGroupId: 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0',
sharedOpenShift: {
notes: 'Inventory Management',
openSlotCount: 5,
displayName: 'Field shift',
startDateTime: '2018-10-04T00:58:45.340Z',
endDateTime: '2018-10-04T09:50:45.332Z',
theme: 'white',
activities: [
{
isPaid: true,
startDateTime: '2018-10-04T00:58:45.340Z',
endDateTime: '2018-10-04T01:58:45.340Z',
code: '',
displayName: 'Lunch'
}
]
},
draftOpenShift: null
};

await client.api('/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8')
    .version('beta')
    .put(openShift);

```