---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 507ec24c26e639de971501e8dadff9b4848c293bc8661b131caa8ae1b0227ac9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052418"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  '@odata.type': '#Microsoft.OutlookServices.ItemAttachment',
  name: 'name-value',
  item: {
    '@odata.type': 'microsoft.graph.message'
  }
};

await client.api('/me/events/{id}/attachments')
    .post(attachment);

```