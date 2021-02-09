---
title: Тип ресурса unmanagedDeviceDiscoveryTask
description: Этот производный тип задачи представляет список неугодных устройств, обнаруженных в сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 039075c13db6a1dba3c7789e0be2ba5b7fdf3782
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162549"
---
# <a name="unmanageddevicediscoverytask-resource-type"></a>Тип ресурса unmanagedDeviceDiscoveryTask

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Этот производный тип задачи представляет список неугодных устройств, обнаруженных в сети.


Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список unmanagedDeviceDiscoveryTasks](../api/intune-partnerintegration-unmanageddevicediscoverytask-list.md)|[коллекция unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|Список свойств и связей объектов [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|
|[Get unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-get.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|Чтение свойств и связей объекта [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|
|[Создание unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-create.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|Создание объекта [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|
|[Удаление unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-delete.md)|Нет|Удаляет [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|
|[Обновление unmanagedDeviceDiscoveryTask](../api/intune-partnerintegration-unmanageddevicediscoverytask-update.md)|[unmanagedDeviceDiscoveryTask](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|Обновление свойств объекта [unmanagedDeviceDiscoveryTask.](../resources/intune-partnerintegration-unmanageddevicediscoverytask.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|String|Имя. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|String|Описание. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|Дата создания. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|Дата окончания. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|Категория. Наследуется [от deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md) Возможные значения: `unknown`, `advancedThreatProtection`.|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|Приоритет. Наследуется [от deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md) Возможные значения: `none`, `high`, `low`.|
|creator|String|Адрес электронной почты создателя. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|creatorNotes|String|Примечания от создателя. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|String|Имя или адрес электронной почты администратора, для которого назначена эта задача. Наследуется [от deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|Состояние. Наследуется [от deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md) Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.|
|unmanagedDevices|[коллекция unmanagedDevice](../resources/intune-partnerintegration-unmanageddevice.md)|Неугодные устройства, обнаруженные в сети.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unmanagedDeviceDiscoveryTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmanagedDeviceDiscoveryTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String",
  "unmanagedDevices": [
    {
      "@odata.type": "microsoft.graph.unmanagedDevice",
      "os": "String",
      "osVersion": "String",
      "ipAddress": "String",
      "deviceName": "String",
      "macAddress": "String",
      "domain": "String",
      "manufacturer": "String",
      "model": "String",
      "location": "String",
      "lastLoggedOnUser": "String",
      "lastSeenDateTime": "String (timestamp)"
    }
  ]
}
```




