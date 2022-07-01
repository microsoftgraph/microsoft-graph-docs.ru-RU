---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 16eb2783aabf3bcf8085571ccd27258c6e397900
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694542"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setCloudPcReviewStatus = {
  reviewStatus: {
    inReview: true,
    userAccessLevel: 'restricted',
    azureStorageAccountId: '/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview'
  }
};

await client.api('/deviceManagement/managedDevices/185f01c2de954929afb129392e5d9f47/setCloudPcReviewStatus')
    .version('beta')
    .post(setCloudPcReviewStatus);

```