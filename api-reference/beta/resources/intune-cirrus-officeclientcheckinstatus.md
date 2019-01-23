---
title: Тип ресурса officeClientCheckinStatus
description: Сущности, которая описывает клиента возврат stats.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403261"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Тип ресурса officeClientCheckinStatus

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущности, которая описывает клиента возврат stats.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userPrincipalName|String|Имя участника-пользователя с помощью устройства.|
|deviceName|String|Имя устройства для возврата.|
|devicePlatform|String|Устройство платформы для возврата.|
|devicePlatformVersion|String|Для возврата версии платформы устройства.|
|wasSuccessful|Логический|Если последний checkin прошла успешно.|
|userId|String|Идентификатор пользователя, с помощью устройства.|
|checkinDateTime|DateTimeOffset|Последний устройства возврат времени в формате UTC.|
|сообщение об ошибке|String|Сообщение об ошибке, если какие-либо связанные для последнего checkin.|
|appliedPolicies|Коллекция String|Список политик доставки на устройство как последний checkin.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



