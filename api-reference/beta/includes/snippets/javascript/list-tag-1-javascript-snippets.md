---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07ebf709cabce3e3eb97d86e415e2184d197a27ea45999d635e2994cecb74a1c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052591"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tags = await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags')
    .version('beta')
    .get();

```