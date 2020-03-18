---
title: Тип ресурса Девицешеллскрипт
description: Intune предоставит клиенту возможность выполнять сценарии оболочки на зарегистрированных устройствах Mac OS. Сценарий можно выполнить один раз или периодически.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e0583eb6dca38af0e490fc23bf57c852bd195ba5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784128"
---
# <a name="deviceshellscript-resource-type"></a>Тип ресурса Девицешеллскрипт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность выполнять сценарии оболочки на зарегистрированных устройствах Mac OS. Сценарий можно выполнить один раз или периодически.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицешеллскриптс](../api/intune-devices-deviceshellscript-list.md)|Коллекция [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md)|Список свойств и связей объектов [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .|
|[Получение Девицешеллскрипт](../api/intune-devices-deviceshellscript-get.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Чтение свойств и связей объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .|
|[Создание Девицешеллскрипт](../api/intune-devices-deviceshellscript-create.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Создание нового объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .|
|[Удаление Девицешеллскрипт](../api/intune-devices-deviceshellscript-delete.md)|Нет|Удаляет объект [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md).|
|[Обновление Девицешеллскрипт](../api/intune-devices-deviceshellscript-update.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Обновление свойств объекта [девицешеллскрипт](../resources/intune-devices-deviceshellscript.md) .|
|[Действие assign](../api/intune-devices-deviceshellscript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сценария управления устройствами.|
|displayName|Строка|Имя скрипта управления устройствами.|
|description|String|Необязательное описание скрипта управления устройствами.|
|скриптконтент|Binary|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения скрипта управления устройствами. Это свойство доступно только для чтения.|
|runAsAccount|[рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|fileName|String|Имя файла сценария.|
|roleScopeTagIds|Коллекция String|Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
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
  "@odata.type": "microsoft.graph.deviceShellScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceShellScript",
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



