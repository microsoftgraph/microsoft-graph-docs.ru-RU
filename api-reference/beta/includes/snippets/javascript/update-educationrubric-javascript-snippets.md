---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c70f424398377d299174e96677bd72a78f68fc433157546bf04472f147bc4693
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57319170"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
  displayName: 'Example Credit Rubric after display name patch'
};

await client.api('/education/me/rubrics/{id}')
    .version('beta')
    .update(educationRubric);

```