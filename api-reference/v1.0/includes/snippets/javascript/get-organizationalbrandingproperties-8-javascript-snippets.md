---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d435c9b73ce79979d8b3a90ff72776953ed277756ca19b457524277feb49e0ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57308730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBrandingLocalization = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr')
    .get();

```