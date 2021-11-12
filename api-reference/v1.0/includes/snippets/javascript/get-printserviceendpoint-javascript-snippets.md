---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: de5314d769a96713213ff4648f1d2fb47bd5b4225d3e39492bffe18cf3554825
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57268480"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printServiceEndpoint = await client.api('/print/services/{printServiceId}/endpoints/{printServiceEndpointId}')
    .get();

```