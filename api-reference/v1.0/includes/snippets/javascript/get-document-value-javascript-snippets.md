---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 22e71a70c0d3cf8f0f81379832fe24b7355c73544023d76d6e03bf32a00188f7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57189933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/print/printers/{printerId}/jobs/{printJobId}/documents/{printDocumentId}/$value')
    .get();

```