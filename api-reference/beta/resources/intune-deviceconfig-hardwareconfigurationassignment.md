---
title: тип ресурса hardwareConfigurationAssignment
description: Содержит свойства, используемые для назначения конфигурации оборудования группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ba4a9f20a0f71bbc02f2f91570de56c7f391372
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345662"
---
# <a name="hardwareconfigurationassignment-resource-type"></a>тип ресурса hardwareConfigurationAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения конфигурации оборудования группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список hardwareConfigurationAssignments](../api/intune-deviceconfig-hardwareconfigurationassignment-list.md)|[коллекция hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Список свойств и связей объектов [hardwareConfigurationAssignment.](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|
|[Get hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-get.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Чтение свойств и связей объекта [hardwareConfigurationAssignment.](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|
|[Создание hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-create.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Создание нового [объекта hardwareConfigurationAssignment.](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|
|[Удаление hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-delete.md)|Нет|Удаляет [hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md).|
|[Обновление hardwareConfigurationAssignment](../api/intune-deviceconfig-hardwareconfigurationassignment-update.md)|[hardwareConfigurationAssignment](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|Обновление свойств объекта [hardwareConfigurationAssignment.](../resources/intune-deviceconfig-hardwareconfigurationassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта назначения группы конфигурации оборудования. Это свойство доступно только для чтения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Id группы Azure Active Directory, на который ориентирована конфигурация.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




