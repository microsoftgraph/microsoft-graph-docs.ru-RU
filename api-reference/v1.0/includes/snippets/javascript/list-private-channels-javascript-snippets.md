---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 02da20b6f63dee437a58d5d924fe805565963c9f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channels = await client.api('/teams/64c323f2-226a-4e64-8ba4-3e6e3f7b9330/channels')
    .filter('membershipType eq \'private\'')
    .get();

```