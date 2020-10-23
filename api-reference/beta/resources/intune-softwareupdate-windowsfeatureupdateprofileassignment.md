---
title: Тип ресурса Виндовсфеатуреупдатепрофилеассигнмент
description: Эта сущность содержит свойства, используемые для назначения профиля обновления компонентов Windows группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a71545503db977ed3ca98da9fb6d8be80d537218
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702245"
---
# <a name="windowsfeatureupdateprofileassignment-resource-type"></a>Тип ресурса Виндовсфеатуреупдатепрофилеассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Эта сущность содержит свойства, используемые для назначения профиля обновления компонентов Windows группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Виндовсфеатуреупдатепрофилеассигнментс](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-list.md)|Коллекция [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Список свойств и связей объектов [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .|
|[Получение Виндовсфеатуреупдатепрофилеассигнмент](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-get.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Чтение свойств и связей объекта [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .|
|[Создание Виндовсфеатуреупдатепрофилеассигнмент](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-create.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Создание нового объекта [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .|
|[Удаление Виндовсфеатуреупдатепрофилеассигнмент](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-delete.md)|Нет|Удаляет объект [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md).|
|[Обновление Виндовсфеатуреупдатепрофилеассигнмент](../api/intune-softwareupdate-windowsfeatureupdateprofileassignment-update.md)|[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)|Обновление свойств объекта [виндовсфеатуреупдатепрофилеассигнмент](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения, которой назначен профиль обновления компонента.|

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





