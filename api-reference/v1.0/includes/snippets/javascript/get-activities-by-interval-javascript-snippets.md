---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68f40bd4638ab7adafdd097522053d65b8aeb1881e42e0347632a552ad61500c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57194730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getActivitiesByInterval = await client.api('/drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')')
    .get();

```