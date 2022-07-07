---
title: Тип ресурса deviceCustomAttributeShellScript
description: Представляет скрипт настраиваемого атрибута для macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 73f970193eb2386d98ad128660681efe70d287bc
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671306"
---
# <a name="devicecustomattributeshellscript-resource-type"></a>Тип ресурса deviceCustomAttributeShellScript

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет скрипт настраиваемого атрибута для macOS.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-list.md)|[Коллекция deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Список свойств и связей объектов [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) .|
|[Получение deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-get.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Чтение свойств и связей объекта [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) .|
|[Создание deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-create.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Создайте объект [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) .|
|[Удаление deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-delete.md)|Нет|Удаляет [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md).|
|[Обновление deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-update.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Обновление свойств объекта [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) .|
|[Действие assign](../api/intune-devices-devicecustomattributeshellscript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для сущности настраиваемого атрибута.|
|customAttributeName|String|Имя настраиваемого атрибута.|
|customAttributeType|[deviceCustomAttributeValueType](../resources/intune-devices-devicecustomattributevaluetype.md)|Ожидаемый тип значения настраиваемого атрибута. Возможные значения: `integer`, `string`, `dateTime`.|
|displayName|String|Имя скрипта управления устройствами.|
|description|String|Необязательное описание скрипта управления устройствами.|
|scriptContent|Binary|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания скрипта управления устройствами. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения скрипта управления устройствами. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-devices-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|fileName|String|Имя файла скрипта.|
|Идентификаторы roleScopeTagId|Коллекция строк|Список идентификаторов тегов области для этого экземпляра PowerShellScript.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[Коллекция deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Список назначений групп для скрипта управления устройствами.|
|assignments|[Коллекция deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Список назначений групп для скрипта управления устройствами.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Выполните сводку для скрипта управления устройствами.|
|deviceRunStates|[Коллекция deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список состояний выполнения для этого скрипта на всех устройствах.|
|userRunStates|[Коллекция deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Список состояний выполнения для этого скрипта для всех пользователей.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCustomAttributeShellScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
  "id": "String (identifier)",
  "customAttributeName": "String",
  "customAttributeType": "String",
  "displayName": "String",
  "description": "String",
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




