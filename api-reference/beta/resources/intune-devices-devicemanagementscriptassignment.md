---
title: Тип ресурса Девицеманажементскриптассигнмент
description: Содержит свойства, используемые для назначения скрипта управления устройствами группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: def29ebd398b56514ad6c1e5897715b603429d4c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550646"
---
# <a name="devicemanagementscriptassignment-resource-type"></a>Тип ресурса Девицеманажементскриптассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения скрипта управления устройствами группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементскриптассигнментс](../api/intune-devices-devicemanagementscriptassignment-list.md)|Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)|Список свойств и связей объектов [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .|
|[Получение Девицеманажементскриптассигнмент](../api/intune-devices-devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md);|Чтение свойств и связей объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .|
|[Создание Девицеманажементскриптассигнмент](../api/intune-devices-devicemanagementscriptassignment-create.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md);|Создание нового объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .|
|[Удаление Девицеманажементскриптассигнмент](../api/intune-devices-devicemanagementscriptassignment-delete.md)|Нет|Удаляет объект [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md).|
|[Обновление Девицеманажементскриптассигнмент](../api/intune-devices-devicemanagementscriptassignment-update.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md);|Обновление свойств объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта назначения группы сценариев управления устройствами.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





