---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2e92c1aefce952ff41b6535d45faf2ea2945c04142f6a7f3af5a1f118e210b10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57317850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/directoryObjects/15c1a2d5-9101-44b2-83ab-885db8a647ca'
};

await client.api('/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830/members/$ref')
    .post(directoryObject);

```