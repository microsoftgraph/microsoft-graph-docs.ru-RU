---
title: Тип ресурса deviceManagementScript
description: Intune будет предоставлять возможности выполнения их скриптов Powershell на устройствах 10 зарегистрированных windows Azure Active Directory в состав клиента. Скрипт может выполняться периодически или один раз.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4fda826ec8033cd51ad4dd13dbc5b523a21e9e3a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412529"
---
# <a name="devicemanagementscript-resource-type"></a>Тип ресурса deviceManagementScript

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Уникальный идентификатор для сценарий управления устройства.|
|displayName|String|Имя скрипта управления устройства.|
|description|String|Необязательное описание сценарий управления устройства.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Интервал для запуска сценария. Если не определена сценарий будет выполняться один раз|
|scriptContent|Binary|Содержимое сценария.|
|createdDateTime|DateTimeOffset|Дата и время создания сценарий управления устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сценарий управления устройства.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения скрипта управления устройства выполняется в. Возможные значения: `system`, `user`.|
|enforceSignatureCheck|Логический|Указывает, должно быть извлеченных подписи скрипта.|
|fileName|String|Имя файла сценария.|
|roleScopeTagIds|Коллекция String|Список идентификаторов тег области для этого экземпляра PowerShellScript.|
|runAs32Bit|Логический|Значение, указывающее ли сценарий PowerShell должна запускаться в 32-разрядная версия|

## <a name="relationships"></a>Отношения
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
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": true
}
```




