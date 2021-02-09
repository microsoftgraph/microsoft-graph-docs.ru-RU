---
title: Тип ресурса windowsQualityUpdateProfileAssignment
description: Этот объект содержит свойства, используемые для назначения профиля обновления качества Windows группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e42d5129bde3fc3df988eebac4712f15f9efe60
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162450"
---
# <a name="windowsqualityupdateprofileassignment-resource-type"></a>Тип ресурса windowsQualityUpdateProfileAssignment

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Этот объект содержит свойства, используемые для назначения профиля обновления качества Windows группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsQualityUpdateProfileAssignments](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-list.md)|[Коллекция windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Список свойств и связей объектов [windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Get windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-get.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Чтение свойств и связей объекта [windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Создание windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-create.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Создание объекта [windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Удаление windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-delete.md)|Нет|Удаляет [windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Обновление windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-update.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Обновление свойств объекта [windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор сущности|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевой объект назначения, для который назначен профиль обновления функций.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdateProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




