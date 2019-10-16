---
title: Тип ресурса deviceManagementScript
description: Intune предоставит клиенту возможность запускать свои сценарии PowerShell на зарегистрированных устройствах, подключенных к системе Windows 10 Azure Active Directory. Сценарий можно выполнить один раз или периодически.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e0a3a4bebaa36ef1f2818b6ced6a9836d6ceb8a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538737"
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
|скриптконтент|Binary|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения скрипта управления устройствами. Это свойство доступно только для чтения.|
|runAsAccount|[рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|Свойства enforcesignaturecheck|Логический|Указывает, нужно ли проверять подпись скрипта.|
|fileName|String|Имя файла сценария.|
|roleScopeTagIds|Коллекция String|Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.|
|runAs32Bit|Логический|Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление устройствами**|
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



