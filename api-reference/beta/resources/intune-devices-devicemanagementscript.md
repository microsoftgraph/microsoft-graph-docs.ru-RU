---
title: Тип ресурса deviceManagementScript
description: Intune предоставит клиенту возможность запускать свои сценарии PowerShell на зарегистрированных устройствах, подключенных к системе Windows 10 Azure Active Directory. Сценарий можно выполнить один раз или периодически.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3587bcf683662f64de95eeef435ca59381aa63c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999880"
---
# <a name="devicemanagementscript-resource-type"></a>Тип ресурса deviceManagementScript

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность запускать свои сценарии PowerShell на зарегистрированных устройствах, подключенных к системе Windows 10 Azure Active Directory. Сценарий можно выполнить один раз или периодически.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScripts](../api/intune-devices-devicemanagementscript-list.md)|Коллекция [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Список свойств и связей объектов [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Получение deviceManagementScript](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Чтение свойств и связей объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Создание deviceManagementScript](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Создание нового объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Удаление deviceManagementScript](../api/intune-devices-devicemanagementscript-delete.md)|Нет|Удаляет объект [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).|
|[Обновление deviceManagementScript](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Обновление свойств объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Действие assign](../api/intune-devices-devicemanagementscript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сценария управления устройствами.|
|displayName|Строка|Имя скрипта управления устройствами.|
|description|String|Необязательное описание скрипта управления устройствами.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Интервал для запуска скрипта. Если не определен, сценарий будет выполняться один раз|
|Скриптконтент|Binary|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения скрипта управления устройствами.|
|runAsAccount|[Рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|Свойства enforcesignaturecheck|Boolean|Указывает, нужно ли проверять подпись скрипта.|
|fileName|String|Имя файла сценария.|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.|
|runAs32Bit|Boolean|Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Список назначений групп для сценария управления устройствами.|
|assignments|Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)|Список назначений групп для сценария управления устройствами.|
|Свойства навигации runsummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Сводка по запуску для сценария управления устройствами.|
|deviceRunStates|Коллекция [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список состояний запуска для этого сценария на всех устройствах.|
|userRunStates|Коллекция [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md)|Список состояний запуска этого сценария для всех пользователей.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": true
}
```





