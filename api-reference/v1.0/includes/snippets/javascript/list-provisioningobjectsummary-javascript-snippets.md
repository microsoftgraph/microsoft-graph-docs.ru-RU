---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 290c09677633495ec827edae86b3cef0c47cb3fa08c74800ecb6b8d529ae5209
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57206702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let provisioning = await client.api('/auditLogs/provisioning')
    .get();

```