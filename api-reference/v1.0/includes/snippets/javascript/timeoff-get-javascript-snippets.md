---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: db731eeff9310bd9a848f6ab5115c669b24ed4d60ff8fa8be82d7e02b2260af0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57364951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOff = await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .get();

```