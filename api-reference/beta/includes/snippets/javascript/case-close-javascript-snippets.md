---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9990a6a07eb44455880c87cbeb9fe0a32b4464bb652daa07d3e952b75ea48e57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57250182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583/close')
    .version('beta')
    .post();

```