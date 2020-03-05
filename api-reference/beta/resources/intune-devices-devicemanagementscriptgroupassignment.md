---
title: Тип ресурса Девицеманажементскриптграупассигнмент
description: Содержит свойства, используемые для назначения скрипта управления устройствами группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ef4119ca102fdc4ea473c058d9e3698ce914532e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528622"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a>Тип ресурса Девицеманажементскриптграупассигнмент

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Ключ объекта назначения группы сценариев управления устройствами. Это свойство доступно только для чтения.|
|таржетграупид|String|Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.|

## <a name="relationships"></a>Связи
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



