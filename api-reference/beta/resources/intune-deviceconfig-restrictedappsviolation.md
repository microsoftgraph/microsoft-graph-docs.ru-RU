---
title: тип ресурса restrictedAppsViolation
description: Нарушение профиля конфигурации ограниченных приложений на устройство на пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a328938975b67ebce005f3cee05fb753f051ad49
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665513"
---
# <a name="restrictedappsviolation-resource-type"></a>тип ресурса restrictedAppsViolation

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Нарушение профиля конфигурации ограниченных приложений на устройство на пользователя

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список ограниченныхAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|[коллекция restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Список свойств и связей объектов [restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)|
|[Get restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Чтение свойств и связей объекта [restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)|
|[Создание restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Создайте новый [объект restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)|
|[Удаление restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|Нет|Удаляет [ограничениеAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).|
|[Обновление restrictedAppsViolation](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|Обновление свойств объекта [restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта. Составлено из accountId, deviceId, policyId и userId|
|userId|String|Уникальный идентификатор пользователя должен быть Guid|
|userName|String|Имя пользователя|
|managedDeviceId|Строка|Уникальный идентификатор управляемого устройства должен быть Guid|
|deviceName|String|Имя устройства|
|deviceConfigurationId|Строка|Уникальный идентификатор конфигурации устройства должен быть Guid|
|DeviceConfigurationName|Строка|Имя профиля конфигурации устройства|
|platformType|[policyPlatformType](../resources/intune-shared-policyplatformtype.md)|Тип платформы. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `androidAOSP`, `all`.|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|Состояние ограниченных приложений. Возможные значения: `prohibitedApps`, `notApprovedApps`.|
|restrictedApps|[коллекция managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)|Список нарушенных приложений с ограниченным доступом|

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




