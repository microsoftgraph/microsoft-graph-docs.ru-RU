---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 545e78a11e0b4d75784846e335d12a0f2154b35ec40588b35b8301e04f7a00a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userAttributeAssignments = await client.api('/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments')
    .get();

```