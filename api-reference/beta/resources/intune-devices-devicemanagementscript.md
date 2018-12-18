---
title: Тип ресурса deviceManagementScript
description: Intune будет предоставлять возможности выполнения их скриптов Powershell на устройствах 10 зарегистрированных windows Azure Active Directory в состав клиента. Скрипт может выполняться периодически или один раз.
author: tfitzmac
ms.openlocfilehash: f35a0b4159c84535c4696f7b57c8486b866504b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351424"
---
# <a name="devicemanagementscript-resource-type"></a>Тип ресурса deviceManagementScript

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Intune будет предоставлять возможности выполнения их скриптов Powershell на устройствах 10 зарегистрированных windows Azure Active Directory в состав клиента. Скрипт может выполняться периодически или один раз.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScripts](../api/intune-devices-devicemanagementscript-list.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) коллекции|Свойства списка и связей объектов [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Получение deviceManagementScript](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Чтение свойства и связи объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Создание deviceManagementScript](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Создание нового объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Удаление deviceManagementScript](../api/intune-devices-devicemanagementscript-delete.md)|Нет|Удаляет [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).|
|[Обновление deviceManagementScript](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|Обновление свойства объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .|
|[Действие assign](../api/intune-devices-devicemanagementscript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сценарий управления устройства.|
|displayName|Строка|Имя скрипта управления устройства.|
|описание|Строка|Необязательное описание сценарий управления устройства.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Интервал для запуска сценария. Если не определена сценарий будет выполняться один раз|
|scriptContent|Binary|Содержимое сценария.|
|createdDateTime|DateTimeOffset|Дата и время создания сценарий управления устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сценарий управления устройства.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения скрипта управления устройства выполняется в. Возможные значения: `system`, `user`.|
|enforceSignatureCheck|Boolean.|Указывает, должно быть извлеченных подписи скрипта.|
|fileName|String|Имя файла сценария.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) коллекции|Список назначений группы для скрипта управления устройства.|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) коллекции|Список назначений группы для скрипта управления устройства.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Запустите сводки по сценарий управления устройства.|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) коллекции|Список выполнения состояний для этого скрипта на всех устройствах.|
|userRunStates|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) коллекции|Список выполнения состояний для этого скрипта для всех пользователей.|

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
  "fileName": "String"
}
```





