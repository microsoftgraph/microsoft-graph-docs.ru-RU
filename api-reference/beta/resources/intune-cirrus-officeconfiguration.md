---
title: Тип ресурса Оффицеконфигуратион
description: Одноэлементный объект, служащий контейнером для всех функций управления устройствами.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6967972cbc94d28d6fde605ba72f3497b9b48e46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488245"
---
# <a name="officeconfiguration-resource-type"></a>Тип ресурса Оффицеконфигуратион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Одноэлементный объект, служащий контейнером для всех функций управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|Получение Оффицеконфигуратион|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Чтение свойств и связей объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .|
|Обновление Оффицеконфигуратион|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|Обновление свойств объекта [оффицеконфигуратион](../resources/intune-cirrus-officeconfiguration.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор конфигурации Office.|
|тенантчеккинстатусес|Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)|Список состояния возврата клиента Office.|
|тенантусерчеккинсуммари|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Сущность, описывающая возврат клиента статуес|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|клиентконфигуратионс|Коллекция [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|Список конфигураций клиентов Office.|

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



