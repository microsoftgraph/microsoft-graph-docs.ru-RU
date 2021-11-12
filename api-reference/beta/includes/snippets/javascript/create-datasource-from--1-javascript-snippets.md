---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a4a2114a0119792ca23901c12c23113adb80545
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "60936892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dataSource = {
    '@odata.type': 'microsoft.graph.ediscovery.siteSource',
    site: {
        webUrl: 'https://contoso.sharepoint.com/sites/SecretSite'
    }
};

await client.api('/compliance/ediscovery/cases/15d80234-8320-4f10-96d0-d98d53ffdfc9/sourceCollections/39b0bafd920e4360995c62e18a5e8a49/additionalsources')
    .version('beta')
    .post(dataSource);

```