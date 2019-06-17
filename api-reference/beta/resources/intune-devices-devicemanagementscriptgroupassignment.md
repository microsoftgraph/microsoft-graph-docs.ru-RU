---
title: Тип ресурса Девицеманажементскриптграупассигнмент
description: Содержит свойства, используемые для назначения скрипта управления устройствами группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d8b3c7c64330016c71131095277ca932ba7f98f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995324"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a>Тип ресурса Девицеманажементскриптграупассигнмент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения скрипта управления устройствами группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементскриптграупассигнментс](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Список свойств и связей объектов [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|
|[Получение Девицеманажементскриптграупассигнмент](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Чтение свойств и связей объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|
|[Создание Девицеманажементскриптграупассигнмент](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Создание нового объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|
|[Удаление Девицеманажементскриптграупассигнмент](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|Нет|Удаляет объект [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md).|
|[Обновление Девицеманажементскриптграупассигнмент](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Обновление свойств объекта [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта назначения группы сценариев управления устройствами.|
|Таржетграупид|String|Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```





