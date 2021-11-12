---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1a16ac7ec7d8ba4c562d941ab8de84836c5882bd411cd394c3b83985cd726462
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57368690"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let services = await client.api('/print/services')
    .version('beta')
    .get();

```