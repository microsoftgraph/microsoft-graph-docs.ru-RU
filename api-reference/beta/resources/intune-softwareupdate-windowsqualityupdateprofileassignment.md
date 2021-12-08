---
title: тип ресурса windowsQualityUpdateProfileAssignment
description: Эта сущность содержит свойства, используемые для назначения группе профиля обновления качества windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 875ce2dc0ab7da6308a8163ac0652200d4c370c7
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346698"
---
# <a name="windowsqualityupdateprofileassignment-resource-type"></a>тип ресурса windowsQualityUpdateProfileAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит свойства, используемые для назначения группе профиля обновления качества windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsQualityUpdateProfileAssignments](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-list.md)|[коллекция windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Список свойств и связей [объектов windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Get windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-get.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Чтение свойств и связей [объекта windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Создание windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-create.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Создайте [новый объект WindowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|
|[Удаление windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-delete.md)|Нет|Удаляет [windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md).|
|[Обновление windowsQualityUpdateProfileAssignment](../api/intune-softwareupdate-windowsqualityupdateprofileassignment-update.md)|[windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|Обновление свойств объекта [windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор сущности|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения, на которую назначен профиль обновления качества.|

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




