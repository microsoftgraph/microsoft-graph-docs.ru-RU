---
title: тип ресурса windowsFeatureUpdateProfileAssignment
description: Эта сущность содержит свойства, используемые для назначения группе профиля обновления функций windows.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf2abc682ae3a26ecc0b73c6b53101cf958647b4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029838"
---
# <a name="windowsfeatureupdateprofileassignment-resource-type"></a>тип ресурса windowsFeatureUpdateProfileAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит свойства, используемые для назначения группе профиля обновления функций windows.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsFeatureUpdateProfileAssignments](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-list.md)|[коллекция windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Список свойств и связей [объектов windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|
|[Get windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-get.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Чтение свойств и связей [объекта windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|
|[Создание windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-create.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Создайте [новый объект windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|
|[Удаление windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-delete.md)|Нет|Удаляет [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).|
|[Обновление windowsFeatureUpdateProfileAssignment](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-update.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Обновление свойств объекта [windowsFeatureUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор сущности|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения, назначенная профилем обновления функций.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```



