---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 44b616cfaad5fdd6185765ecc3a81d49ecefe891d39a4fc8315691b6869453cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050423"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removePassword = {
    keyId: 'f0b0b335-1d71-4883-8f98-567911bfdca6'
};

await client.api('/applications/{id}/removePassword')
    .post(removePassword);

```