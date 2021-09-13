---
title: Регистрация в управлении обновлениями службой Windows обновления для бизнеса
description: Когда устройство зачислилось в управление обновлениями службой развертывания Windows для бизнеса, вы можете использовать службу развертывания для управления контентом, доставленным из Windows Update на это устройство.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: conceptualPageType
ms.openlocfilehash: cfa1d9fe41acc0b8a872c8f0e8a9b64bb6750c90
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117538"
---
# <a name="enroll-in-update-management-by-the-windows-update-for-business-deployment-service"></a>Регистрация в управлении обновлениями службой Windows обновления для бизнеса

При регистрации устройства в управлении обновлениями службой развертывания Windows обновления для бизнеса можно использовать службу развертывания для управления контентом, доставленным из Windows Update на это устройство. Вы можете записать устройство в управление обновлениями по категории обновления.

Сегодня служба развертывания поддерживает регистрацию в управлении обновлениями Windows 10 функций. В настоящее время служба развертывания не требует регистрации в управлении обновлениями Windows 10 качества, чтобы развернуть ускоренные обновления качества.

## <a name="enroll-the-device-in-update-management"></a>Регистрация устройства в управлении обновлениями

При регистрации устройства в управлении для определенной категории обновлений служба развертывания становится органом для обновлений этой категории, исходя из Windows Update. В результате устройства не получают обновления этой категории из Windows, пока не развернуто обновление с помощью службы развертывания, назначив его [развертыванию.](windowsupdates-deployments.md) Устройства автоматически регистрируются в службе при регистрации в управлении службой (например, объект [azureADDevice](/graph/api/resources/windowsupdates-azureaddevice.md) автоматически создается, если он еще не существует).

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

Вы можете проверить состояние регистрации [](/graph/api/windowsupdates-azureaddevice-get) устройства, получив устройство  и посмотрев свойства регистраций и ошибок на **объекте azureADDevice.**  Устройство, успешно зарегистрированное в управлении обновлениями, имеет объект [updateManagementEnrollment](/graph/api/resources/windowsupdates-updatemanagementenrollment) в коллекции регистраций и не имеет объектов [updatableAssetError](/graph/api/resources/windowsupdates-updatableasseterror) в коллекции ошибок. Устройство, которое служба пыталась зарегистрировать, но столкнулось с ошибкой, заполнялось коллекциями как для регистрации, так и для ошибок. Устройство, для которого служба не получала запросов на регистрацию, имеет пустые коллекции как для регистрации, так и для ошибок.

В следующем примере показано устройство, успешно зарегистрированное службой в управлении обновлениями функций.

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

## <a name="unenroll-from-management-by-the-service-or-unregister-from-the-service"></a>Отстранить от управления службой или оторегистрить из службы 

При откреплении устройства от управления службой для данной категории обновлений устройство больше не управляется службой развертывания и может начать получать другие обновления из Windows Update в зависимости от конфигурации политики. Если устройство назначено любому развертыванию для данной категории обновлений, оно не получает этого контента. Устройство остается зарегистрированным в службе и по-прежнему регистрируется и получает контент для других категорий обновлений (если это применимо).

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

Вы можете полностью оторегистрить устройство из службы, удалив объект устройства. При незарегистрированном устройстве оно автоматически отключается от управления службой для всех категорий обновлений и удаляется из каждого [развертыванияAudience](/graph/api/resources/windowsupdates-deploymentaudience) и [updatableAssetGroup.](/graph/api/resources/windowsupdates-updatableassetgroup)

### <a name="request"></a>Запрос

``` http
DELETE https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{azureADDeviceId}
```

### <a name="response"></a>Отклик
``` http
HTTP/1.1 202 Accepted
```

