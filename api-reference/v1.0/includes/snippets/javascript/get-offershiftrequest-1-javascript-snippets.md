---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9b10d5ecb1165cf842ec3c050d7c5ceba7e6eaedf4a53c6004b21336285403e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let offerShiftRequest = await client.api('/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}')
    .get();

```