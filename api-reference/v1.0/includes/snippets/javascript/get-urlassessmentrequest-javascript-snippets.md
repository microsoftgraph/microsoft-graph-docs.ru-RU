---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ad644b4cadb7c2e98500a40ba282680813152ffb57ee30ac29ab2af3e911ab83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57321818"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let threatAssessmentRequest = await client.api('/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b')
    .get();

```