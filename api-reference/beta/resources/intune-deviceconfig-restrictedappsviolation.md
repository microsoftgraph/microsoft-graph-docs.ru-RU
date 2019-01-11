---
title: Тип ресурса restrictedAppsViolation
description: Нарушение профиля конфигурации ограниченных приложений каждого устройства на одного пользователя
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aefd9996805f0ee454bebc8871662b0ceac05a9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849380"
---
# <a name="restrictedappsviolation-resource-type"></a>Тип ресурса restrictedAppsViolation

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Нарушение профиля конфигурации ограниченных приложений каждого устройства на одного пользователя
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список restrictedAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) коллекции|Свойства списка и связей объектов [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Получение restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Чтение свойства и связи объекта [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Создание restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Создание нового объекта [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|
|[Удаление restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|Нет|Удаляет [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).|
|[Обновление restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Обновление свойства объекта [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для объекта. Состоит из accountId, deviceId, policyId и идентификатор пользователя|
|userId|String|Уникальный идентификатор пользователя, должен быть идентификатор Guid|
|userName|String|Имя пользователя|
|managedDeviceId|Строка|Уникальный идентификатор управляемого устройства, должен быть идентификатор Guid|
|deviceName|String|Имя устройства|
|deviceConfigurationId|Строка|Конфигурация профиля уникальный идентификатор устройства, должен быть идентификатор Guid|
|deviceConfigurationName|Строка|Имя профиля конфигурации устройства|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|Тип платформы. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|Состояние ограниченных приложений. Возможные значения: `prohibitedApps`, `notApprovedApps`.|
|restrictedApps|[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) коллекции|Список нарушенных ограниченных приложений|

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





