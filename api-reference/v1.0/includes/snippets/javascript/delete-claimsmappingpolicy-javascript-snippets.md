---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c73153210a48825ad082004330b18d816ce09233
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786779"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/claimsMappingPolicies/{id}')
    .delete();

```