---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7e84a0514d53b5b3ad4bee849eb9189a2c89886e
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560947"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSubmissionResource = {
    resource: {
        displayName: '_FTP_EDC-61424749-250820211136.pdf',
        fileUrl: 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3',
        '@odata.type': '#microsoft.graph.educationFileResource'
    }
};

await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources')
    .version('beta')
    .post(educationSubmissionResource);

```