---
title: Тип ресурса managedDeviceMobileAppConfigurationAssignment
description: Содержит свойства, используемые для назначения конфигурации приложения MDM группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 064f881f0d90d2748446bcd618b07767c4836db5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149982"
---
# <a name="manageddevicemobileappconfigurationassignment-resource-type"></a>Тип ресурса managedDeviceMobileAppConfigurationAssignment

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения конфигурации приложения MDM группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedDeviceMobileAppConfigurationAssignments](../api/intune-apps-manageddevicemobileappconfigurationassignment-list.md)|Коллекция [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Перечисление свойств и связей объектов [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|
|[Получение managedDeviceMobileAppConfigurationAssignment](../api/intune-apps-manageddevicemobileappconfigurationassignment-get.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Считывание свойств и связей объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|
|[Создание managedDeviceMobileAppConfigurationAssignment](../api/intune-apps-manageddevicemobileappconfigurationassignment-create.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Создание объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|
|[Удаление managedDeviceMobileAppConfigurationAssignment](../api/intune-apps-manageddevicemobileappconfigurationassignment-delete.md)|Отсутствует|Удаление [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|
|[Обновление managedDeviceMobileAppConfigurationAssignment](../api/intune-apps-manageddevicemobileappconfigurationassignment-update.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)|Обновление свойств объекта [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Объект, для которого назначается политика соблюдения условий.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




