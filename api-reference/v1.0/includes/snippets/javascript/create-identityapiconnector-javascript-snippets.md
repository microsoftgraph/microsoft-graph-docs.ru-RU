---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2457e8202372536b24f7e2f665c2f472b617dd354d33bc39e2942440b5c885a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306638"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    displayName: 'Test API',
    targetUrl: 'https://someotherapi.com/api',
    authenticationConfiguration: {
        '@odata.type':'#microsoft.graph.pkcs12Certificate',
        pkcs12Value: 'eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA',
        password: 'CertificatePassword'
    }
};

await client.api('/identity/apiConnectors')
    .post(identityApiConnector);

```