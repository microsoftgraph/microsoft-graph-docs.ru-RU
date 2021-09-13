---
title: тип ресурса windowsQualityUpdateProfileAssignment
description: Эта сущность содержит свойства, используемые для назначения группе профиля обновления качества windows.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5c7e78d37e0c1d4fd104a408ff62522b533b3fcc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054221"
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



