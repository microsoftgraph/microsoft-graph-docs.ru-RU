---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 91677a87421edbe6c914e8f5daf423ec30bc2bf1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797239"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleDefinition = await client.api('/roleManagement/directory/roleDefinitions/fdd7a751-b60b-444a-984c-02652fe8fa1c')
    .version('beta')
    .expand('inheritsPermissionsFrom')
    .get();

```