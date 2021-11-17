---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c3c9af91d8bd14d61b741bce2844213b145ea224acf2fcb6504f1639b82b3bc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57365179"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const deployment = {
  '@odata.type': '#microsoft.graph.windowsUpdates.deployment',
  settings: {
    '@odata.type': 'microsoft.graph.windowsUpdates.windowsDeploymentSettings',
    monitoring: {
      monitoringRules: [
        {
          signal: 'rollback',
          threshold: 5,
          action: 'pauseDeployment'
        }
      ]
    }
  }
};

await client.api('/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5')
    .version('beta')
    .update(deployment);

```