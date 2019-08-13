---
title: Тип ресурса Девицехеалсскрипт
description: Intune предоставит клиенту возможность запускать свои сценарии PowerShell на зарегистрированных устройствах, подключенных к системе Windows 10 Azure Active Directory. Сценарий можно выполнить один раз или периодически.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ccde92a3d69cae27bc1a62926e733bc903c978e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36376111"
---
# <a name="devicehealthscript-resource-type"></a>Тип ресурса Девицехеалсскрипт

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность запускать свои сценарии PowerShell на зарегистрированных устройствах, подключенных к системе Windows 10 Azure Active Directory. Сценарий можно выполнить один раз или периодически.


Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицехеалсскриптс](../api/intune-devices-devicehealthscript-list.md)|Коллекция [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md)|Список свойств и связей объектов [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .|
|[Получение Девицехеалсскрипт](../api/intune-devices-devicehealthscript-get.md)|[девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md)|Чтение свойств и связей объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .|
|[Создание Девицехеалсскрипт](../api/intune-devices-devicehealthscript-create.md)|[девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md)|Создание нового объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .|
|[Удаление Девицехеалсскрипт](../api/intune-devices-devicehealthscript-delete.md)|Нет|Удаляет объект [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md).|
|[Обновление Девицехеалсскрипт](../api/intune-devices-devicehealthscript-update.md)|[девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md)|Обновление свойств объекта [девицехеалсскрипт](../resources/intune-devices-devicehealthscript.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сценария управления устройствами. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|displayName|Строка|Имя скрипта управления устройствами. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|description|String|Необязательное описание скрипта управления устройствами. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Интервал для запуска скрипта. Если не определен, сценарий будет выполняться один раз наследуемый от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|скриптконтент|Binary|Содержимое скрипта. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения скрипта управления устройствами. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|runAsAccount|[рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md). Возможные значения: `system`, `user`.|
|Свойства enforcesignaturecheck|Boolean|Указывает, нужно ли проверять подпись скрипта. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|fileName|String|Имя файла сценария. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого экземпляра Повершеллскрипт. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|runAs32Bit|Boolean|Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 – бит, наследуемый от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|комплианцеруле|[девицехеалсскрипткомплианцеруле](../resources/intune-devices-devicehealthscriptcompliancerule.md)|Пока не задокументировано.|
|ремедиатионскриптконтент|Binary|Пока не задокументировано.|
|рунремедиатионскрипт|Boolean|Н/Д|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [девицеманажементскриптграупассигнмент](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Список назначений групп для сценария управления устройствами. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|assignments|Коллекция [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md)|Список назначений групп для сценария управления устройствами. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|Свойства навигации runsummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Сводка по запуску для сценария управления устройствами. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|deviceRunStates|Коллекция [девицеманажементскриптдевицестате](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список состояний запуска для этого сценария на всех устройствах. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|
|userRunStates|Коллекция [девицеманажементскриптусерстате](../resources/intune-devices-devicemanagementscriptuserstate.md)|Список состояний запуска этого сценария для всех пользователей. Наследуется от [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
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
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "String",
    "operator": "String",
    "detectionValue": "String"
  },
  "remediationScriptContent": "binary",
  "runRemediationScript": true
}
```



