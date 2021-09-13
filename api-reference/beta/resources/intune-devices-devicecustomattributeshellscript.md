---
title: тип ресурса deviceCustomAttributeShellScript
description: Представляет настраиваемый скрипт атрибута для macOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53e6daffb2445fba581b66eec0a497eaa9091aa4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023467"
---
# <a name="devicecustomattributeshellscript-resource-type"></a>тип ресурса deviceCustomAttributeShellScript

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет настраиваемый скрипт атрибута для macOS.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список устройствCustomAttributeShellScripts](../api/intune-devices-devicecustomattributeshellscript-list.md)|[коллекция deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Список свойств и связей объектов [deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)|
|[Get deviceCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-get.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Чтение свойств и связей [объекта deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)|
|[Создание устройстваCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-create.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Создайте новый [объект deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)|
|[Удаление устройстваCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-delete.md)|Нет|Удаляет [устройствоCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md).|
|[Обновление устройстваCustomAttributeShellScript](../api/intune-devices-devicecustomattributeshellscript-update.md)|[deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md)|Обновление свойств объекта [deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)|
|[Действие assign](../api/intune-devices-devicecustomattributeshellscript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для настраиваемого объекта атрибута.|
|customAttributeName|Строка|Имя настраиваемого атрибута.|
|customAttributeType|[deviceCustomAttributeValueType](../resources/intune-devices-devicecustomattributevaluetype.md)|Ожидаемый тип значения настраиваемого атрибута. Возможные значения: `integer`, `string`, `dateTime`.|
|displayName|String|Имя сценария управления устройствами.|
|description|Строка|Необязательное описание сценария управления устройствами.|
|scriptContent|В двоичном формате|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сценария управления устройствами. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|fileName|String|Имя файла скрипта.|
|roleScopeTagIds|Коллекция строк|Список ID-тегов области для этого экземпляра PowerShellScript.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|[коллекция deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Список групповых назначений для сценария управления устройствами.|
|assignments|[коллекция deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Список групповых назначений для сценария управления устройствами.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Запустите сводку для сценария управления устройствами.|
|deviceRunStates|[коллекция deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список состояния запуска для этого скрипта на всех устройствах.|
|userRunStates|[коллекция deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Список состояния запуска для этого скрипта для всех пользователей.|

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



