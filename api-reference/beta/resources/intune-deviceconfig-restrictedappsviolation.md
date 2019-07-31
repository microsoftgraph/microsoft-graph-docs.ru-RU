---
title: Тип ресурса Рестриктедаппсвиолатион
description: Нарушение профиля конфигурации ограниченных приложений на каждое устройство для каждого пользователя
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34c52c7d9d013563378ffbed4cb5af656c7c0502
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969732"
---
# <a name="restrictedappsviolation-resource-type"></a>Тип ресурса Рестриктедаппсвиолатион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Нарушение профиля конфигурации ограниченных приложений на каждое устройство для каждого пользователя

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Рестриктедаппсвиолатионс](../api/intune-deviceconfig-restrictedappsviolation-list.md)|Коллекция [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md)|Список свойств и связей объектов [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Получение Рестриктедаппсвиолатион](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Чтение свойств и связей объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Создание Рестриктедаппсвиолатион](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Создание нового объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Удаление Рестриктедаппсвиолатион](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|Нет|Удаляет объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md).|
|[Обновление Рестриктедаппсвиолатион](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Обновление свойств объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта. Состоит из accountId, deviceId, Полициид и userId|
|userId|String|Уникальный идентификатор пользователя, должен быть GUID|
|userName|String|Имя пользователя|
|Манажеддевицеид|String|Уникальный идентификатор управляемого устройства, должен быть GUID|
|deviceName|String|Имя устройства|
|Девицеконфигуратионид|String|Уникальный идентификатор профиля конфигурации устройства, должен быть GUID|
|Девицеконфигуратионнаме|String|Имя профиля конфигурации устройства|
|platformType|[Полициплатформтипе](../resources/intune-deviceconfig-policyplatformtype.md)|Тип платформы. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|Состояние ограниченных приложений. Возможные значения: `prohibitedApps`, `notApprovedApps`.|
|restrictedApps|Коллекция [манажеддевицерепортедапп](../resources/intune-deviceconfig-manageddevicereportedapp.md)|Список нарушенных приложений с ограниченным доступом|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```





