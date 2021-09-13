---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7bc3e34f18ca2160ffb9e8b46d61187d834a98ed05c9d9de9f801984d4ce9aee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57139421"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/{class-id}/teachers/{teacher-id}')
    .delete();

```