---
title: Тип ресурса deviceShellScript
description: Intune предоставляет клиенту возможность запускать скрипты оболочки на зарегистрированных устройствах Mac OS. Скрипт может выполняться один раз или периодически.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f5c4b7a5687c10b4aa8cb00a2561eccac96f9d12
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671313"
---
# <a name="deviceshellscript-resource-type"></a>Тип ресурса deviceShellScript

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставляет клиенту возможность запускать скрипты оболочки на зарегистрированных устройствах Mac OS. Скрипт может выполняться один раз или периодически.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceShellScript](../api/intune-devices-deviceshellscript-list.md)|[Коллекция deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Список свойств и связей объектов [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .|
|[Получение deviceShellScript](../api/intune-devices-deviceshellscript-get.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Чтение свойств и связей объекта [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .|
|[Создание deviceShellScript](../api/intune-devices-deviceshellscript-create.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Создайте объект [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .|
|[Удаление deviceShellScript](../api/intune-devices-deviceshellscript-delete.md)|Нет|Удаляет [deviceShellScript](../resources/intune-devices-deviceshellscript.md).|
|[Обновление deviceShellScript](../api/intune-devices-deviceshellscript-update.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Обновление свойств объекта [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .|
|[Действие assign](../api/intune-devices-deviceshellscript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|executionFrequency|Длительность|Интервал выполнения скрипта. Если скрипт не определен, он будет выполняться один раз.|
|retryCount|Int32|Количество повторных попыток скрипта в случае сбоя|
|blockExecutionNotifications|Логическое|Не уведомляет пользователя о выполнении скрипта|
|id|String|Уникальный идентификатор скрипта управления устройствами.|
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
  "@odata.type": "microsoft.graph.deviceShellScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "String (duration)",
  "retryCount": 1024,
  "blockExecutionNotifications": true,
  "id": "String (identifier)",
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




