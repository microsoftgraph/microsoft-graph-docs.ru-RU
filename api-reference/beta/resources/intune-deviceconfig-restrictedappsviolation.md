---
title: тип ресурса restrictedAppsViolation
description: Нарушение профиля конфигурации ограниченных приложений на устройство на пользователя
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a0e1df4eacf84c096bf814dfd9d37289977e826b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075440"
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
|id|String|Уникальный идентификатор объекта. Составлено из accountId, deviceId, policyId и userId|
|userId|String|Уникальный идентификатор пользователя должен быть Guid|
|userName|String|Имя пользователя|
|managedDeviceId|String|Уникальный идентификатор управляемого устройства должен быть Guid|
|deviceName|String|Имя устройства|
|deviceConfigurationId|String|Уникальный идентификатор конфигурации устройства должен быть Guid|
|DeviceConfigurationName|String|Имя профиля конфигурации устройства|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|Тип платформы. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `androidAOSP`, `all`.|
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



