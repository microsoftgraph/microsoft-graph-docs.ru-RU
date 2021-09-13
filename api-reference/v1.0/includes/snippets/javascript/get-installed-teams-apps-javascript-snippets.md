---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bbae5c50ffbf32c5079c229d48d5a678f2934d84673715263175f3cdf507cb2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57313021"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppInstallation = await client.api('/teams/{id}/installedApps/{id}')
    .get();

```