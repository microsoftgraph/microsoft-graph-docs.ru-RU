---
title: Тип ресурса Рестриктедаппсвиолатион
description: Нарушение профиля конфигурации ограниченных приложений на каждое устройство для каждого пользователя
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae4212ce13a71f33d493de61e00a321577b8d16a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444925"
---
# <a name="restrictedappsviolation-resource-type"></a>Тип ресурса Рестриктедаппсвиолатион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|манажеддевицеид|String|Уникальный идентификатор управляемого устройства, должен быть GUID|
|deviceName|String|Имя устройства|
|девицеконфигуратионид|String|Уникальный идентификатор профиля конфигурации устройства, должен быть GUID|
|девицеконфигуратионнаме|String|Имя профиля конфигурации устройства|
|platformType|[полициплатформтипе](../resources/intune-shared-policyplatformtype.md)|Тип платформы. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|Состояние ограниченных приложений. Возможные значения: `prohibitedApps`, `notApprovedApps`.|
|restrictedApps|Коллекция [манажеддевицерепортедапп](../resources/intune-deviceconfig-manageddevicereportedapp.md)|Список нарушенных приложений с ограниченным доступом|

## <a name="relationships"></a>Связи
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



