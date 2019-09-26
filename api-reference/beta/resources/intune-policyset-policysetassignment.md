---
title: Тип ресурса Полицисетассигнмент
description: Класс, содержащий свойства, которые используются для назначения политик.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 480e05dafdf4d10ab500271c44b4dd3421877a0c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201254"
---
# <a name="policysetassignment-resource-type"></a>Тип ресурса Полицисетассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, которые используются для назначения политик.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Полицисетассигнментс](../api/intune-policyset-policysetassignment-list.md)|Коллекция [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md)|Список свойств и связей объектов [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .|
|[Получение Полицисетассигнмент](../api/intune-policyset-policysetassignment-get.md)|[полицисетассигнмент](../resources/intune-policyset-policysetassignment.md)|Чтение свойств и связей объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .|
|[Создание Полицисетассигнмент](../api/intune-policyset-policysetassignment-create.md)|[полицисетассигнмент](../resources/intune-policyset-policysetassignment.md)|Создание нового объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .|
|[Удаление Полицисетассигнмент](../api/intune-policyset-policysetassignment-delete.md)|Нет|Удаляет объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md).|
|[Обновление Полицисетассигнмент](../api/intune-policyset-policysetassignment-update.md)|[полицисетассигнмент](../resources/intune-policyset-policysetassignment.md)|Обновление свойств объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Полицисетассигнмент.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетассигнмент.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевая группа Полицисетассигнмент|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



