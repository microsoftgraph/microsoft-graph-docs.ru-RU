---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 88780e10bc2fa69c98766bd28fc938e89c1455d1bb89dad30073cca4136e9c23
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255152"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: 'Fabrikam Arts High School',
  description: 'Magnate school for the arts. Los Angeles School District'
};

await client.api('/education/schools/{school-id}')
    .update(educationSchool);

```