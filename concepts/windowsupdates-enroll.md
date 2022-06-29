---
title: Регистрация в управлении обновлениями службой клиентский компонент Центра обновления Windows для бизнеса
description: Зарегистрируйте устройство в управлении обновлениями, чтобы можно было использовать службу развертывания клиентский компонент Центра обновления Windows для бизнеса для управления содержимым, доставленным клиентский компонент Центра обновления Windows на это устройство.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: 1606b9a063a11406366f63ae9d26add8ddded96b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437494"
---
# <a name="enroll-in-update-management-by-the-windows-update-for-business-deployment-service"></a>Регистрация в управлении обновлениями службой клиентский компонент Центра обновления Windows для бизнеса

При регистрации устройства в управлении обновлениями службой развертывания клиентский компонент Центра обновления Windows для бизнеса можно использовать службу развертывания для управления содержимым, доставленным клиентский компонент Центра обновления Windows на это устройство. Вы можете зарегистрировать устройство в управлении обновлениями по категории обновлений.

Сейчас служба развертывания поддерживает регистрацию в управлении обновлениями Windows 10 компонентов. В данный момент служба развертывания не требует регистрации в управлении Windows 10 исправлений для развертывания ускоренного обновления качества.

## <a name="enroll-the-device-in-update-management"></a>Регистрация устройства в управлении обновлениями

При регистрации устройства в управлении для определенной категории обновлений служба развертывания становится центром обновления этой категории, поступающих из клиентский компонент Центра обновления Windows. В результате устройства не получают обновления этой категории из клиентский компонент Центра обновления Windows, пока вы не развернете обновление с помощью службы развертывания, назначив его [развертыванию](windowsupdates-deployments.md). Устройства автоматически регистрируются в службе при регистрации в управлении службой (то есть объект [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice) создается автоматически, если он еще не существует).

### <a name="request"></a>Запрос

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    },
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a>Отклик

``` http
HTTP/1.1 202 Accepted
```

## <a name="check-the-enrollment-state-of-a-device"></a>Проверка состояния регистрации устройства

Чтобы проверить состояние регистрации устройства, можно получить устройство и [](/graph/api/windowsupdates-azureaddevice-get) просмотреть свойства регистраций и ошибок в **объекте azureADDevice**.  Устройство, успешно зарегистрированное в управлении обновлениями, имеет объект [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) в коллекции регистраций и не имеет объектов [updatableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) в коллекции ошибок. Устройство, которое служба попытались зарегистрировать, но обнаружило ошибку, заполнит коллекции как для регистраций, так и для ошибок. Устройство, для которого служба не получила запросов на регистрацию, содержит пустые коллекции как для регистраций, так и для ошибок.

В следующем примере показано устройство, которое успешно зарегистрировано в управлении обновлениями компонентов службой.

### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/983f03cd-03cd-983f-cd03-3f98cd033f98
```

### <a name="response"></a>Отклик
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
    "id": "983f03cd-03cd-983f-cd03-3f98cd033f98",
    "errors": [],
    "enrollments": [
      {
        "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment",
        "updateCategory": "feature"
      }
    ]
  }
}
```

## <a name="unenroll-from-management-by-the-service-or-unregister-from-the-service"></a>Отмена регистрации в управлении службой или отмена регистрации в службе 

При отмене регистрации устройства службой для данной категории обновления устройство больше не управляется службой развертывания и может начать получать другие обновления из клиентский компонент Центра обновления Windows в зависимости от конфигурации политики. Если устройство назначено любому развертыванию для данной категории обновления, оно не получает это содержимое. Устройство остается зарегистрированным в службе и по-прежнему зарегистрировано и получает содержимое для других категорий обновлений (если применимо).

### <a name="request"></a>Запрос

``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/unenrollAssets
Content-Type: application/json

{
  "updateCategory": "feature",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a>Отклик

``` http
HTTP/1.1 202 Accepted
```

Вы можете полностью отменить регистрацию устройства в службе, удалив объект устройства. При отмене регистрации устройство автоматически отменяется из управления службой для всех категорий обновлений и удаляется из всех [deploymentAudience](/graph/api/resources/windowsupdates-deploymentaudience) и [updatableAssetGroup](/graph/api/resources/windowsupdates-updatableassetgroup).

### <a name="request"></a>Запрос

``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a>Отклик
``` http
HTTP/1.1 202 Accepted
```

