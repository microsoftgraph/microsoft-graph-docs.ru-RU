---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c94bba4d54dd2903928f9e62a97b24e7c1eb6e20
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = <Image>;

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo')
    .put(stream);

```