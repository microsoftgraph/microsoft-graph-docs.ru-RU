---
title: Тип ресурса officeConfiguration
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
ms.openlocfilehash: 4a3657153ead53a5367c23cdc51b0e40a8efe535
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077088"
---
# <a name="officeconfiguration-resource-type"></a>Тип ресурса officeConfiguration

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|Получение officeConfiguration|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Чтение свойства и связи объекта [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .|
|Обновление officeConfiguration|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Обновление свойства объекта [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор конфигурации office.|
|tenantCheckinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) коллекции|Список office состояние возврата клиента.|
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Сущности, которая описывает клиента возврат statues|

## <a name="relationships"></a>Связи
|Связь|Тип|Description|
|:---|:---|:---|
|clientConfigurations|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) коллекции|Список настройки клиента office.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
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
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```



