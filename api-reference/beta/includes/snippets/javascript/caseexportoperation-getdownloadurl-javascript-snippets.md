---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 78abf671ba7678a11571f6004bd2eb8ff006c7becb5bcc1115e8fb29317021d9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57307267"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/operations/63926d4779c243458902328d83f61f53/microsoft.graph.ediscovery.caseExportOperation/getDownloadUrl')
    .version('beta')
    .get();

```