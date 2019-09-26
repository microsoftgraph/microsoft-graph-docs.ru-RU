---
title: Тип ресурса deviceManagementScript
description: Intune предоставит клиенту возможность запускать свои сценарии PowerShell на зарегистрированных устройствах, подключенных к системе Windows 10 Azure Active Directory. Сценарий можно выполнить один раз или периодически.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ed2e4a12d7070a93bd47662714d646a640989c1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201230"
---
# <a name="devicemanagementscript-resource-type"></a>Тип ресурса deviceManagementScript

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность запускать свои сценарии PowerShell на зарегистрированных устройствах, подключенных к системе Windows 10 Azure Active Directory. Сценарий можно выполнить один раз или периодически.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScripts](../api/intune-shared-devicemanagementscript-list.md)|Коллекция [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список свойств и связей объектов [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|[Получение deviceManagementScript](../api/intune-shared-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Чтение свойств и связей объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|[Создание deviceManagementScript](../api/intune-shared-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Создание нового объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|[Удаление deviceManagementScript](../api/intune-shared-devicemanagementscript-delete.md)|Нет|Удаляет объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).|
|[Обновление deviceManagementScript](../api/intune-shared-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Обновление свойств объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|**Управление устройствами**|
|[Действие assign](../api/intune-shared-devicemanagementscript-assign.md)|Нет|Н/Д|
|**Набор политик**|
|[действие Хаспайлоадлинкс](../api/intune-shared-devicemanagementscript-haspayloadlinks.md)|Коллекция [хаспайлоадлинкресултитем](../resources/intune-policyset-haspayloadlinkresultitem.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сценария управления устройствами.|
|displayName|Строка|Имя скрипта управления устройствами.|
|description|String|Необязательное описание скрипта управления устройствами.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Интервал для запуска скрипта. Если не определен, сценарий будет выполняться один раз|
|скриптконтент|Binary|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения скрипта управления устройствами. Это свойство доступно только для чтения.|
|runAsAccount|[рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|Свойства enforcesignaturecheck|Boolean.|Указывает, нужно ли проверять подпись скрипта.|
|fileName|String|Имя файла сценария.|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.|
|runAs32Bit|Boolean.|Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|**Управление устройствами**|
|groupAssignments|Коллекция Девицеманажементскриптграупассигнмент|Список назначений групп для сценария управления устройствами.|
|assignments|Коллекция Девицеманажементскриптассигнмент|Список назначений групп для сценария управления устройствами.|
|Свойства навигации runsummary|deviceManagementScriptRunSummary|Сводка по запуску для сценария управления устройствами.|
|deviceRunStates|Коллекция Девицеманажементскриптдевицестате|Список состояний запуска для этого сценария на всех устройствах.|
|userRunStates|Коллекция Девицеманажементскриптусерстате|Список состояний запуска этого сценария для всех пользователей.|

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



