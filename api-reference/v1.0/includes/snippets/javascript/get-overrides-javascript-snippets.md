---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ed78aecade0363f09d6b7711231a18a4e62925d14cfd18434357ac30a22842ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57323035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let overrides = await client.api('/me/inferenceClassification/overrides')
    .get();

```