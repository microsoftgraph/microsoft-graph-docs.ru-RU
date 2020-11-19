---
title: Тип ресурса Девицекустоматтрибутешеллскрипт
description: Представляет скрипт настраиваемого атрибута для macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 71c7630daa03c695284bf225e56c69c2d6172b0b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49293186"
---
# <a name="devicecustomattributeshellscript-resource-type"></a>Тип ресурса Девицекустоматтрибутешеллскрипт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет скрипт настраиваемого атрибута для macOS.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицекустоматтрибутешеллскриптс](../api/intune-devices-devicecustomattributeshellscript-list.md)|Коллекция [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md)|Список свойств и связей объектов [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) .|
|[Получение Девицекустоматтрибутешеллскрипт](../api/intune-devices-devicecustomattributeshellscript-get.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Чтение свойств и связей объекта [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) .|
|[Создание Девицекустоматтрибутешеллскрипт](../api/intune-devices-devicecustomattributeshellscript-create.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Создание нового объекта [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) .|
|[Удаление Девицекустоматтрибутешеллскрипт](../api/intune-devices-devicecustomattributeshellscript-delete.md)|Нет|Удаляет объект [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md).|
|[Обновление Девицекустоматтрибутешеллскрипт](../api/intune-devices-devicecustomattributeshellscript-update.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Обновление свойств объекта [девицекустоматтрибутешеллскрипт](../resources/intune-devices-devicecustomattributeshellscript.md) .|
|[Действие assign](../api/intune-devices-devicecustomattributeshellscript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для объекта настраиваемого атрибута.|
|кустоматтрибутенаме|String|Имя настраиваемого атрибута.|
|кустоматтрибутетипе|[deviceCustomAttributeValueType](../resources/intune-devices-devicecustomattributevaluetype.md)|Ожидаемый тип значения настраиваемого атрибута. Возможные значения: `integer`, `string`, `dateTime`.|
|displayName|String|Имя скрипта управления устройствами.|
|description|String|Необязательное описание скрипта управления устройствами.|
|скриптконтент|Binary|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения скрипта управления устройствами. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|fileName|String|Имя файла сценария.|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.|

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




