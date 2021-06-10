---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ee02dc36e9604e4c957b7dcff6ef9778e5acb702
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870250"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
};

await client.api('/education/classes/11012/assignments/19002/setUpResourcesFolder')
    .version('beta')
    .post(educationAssignment);

```