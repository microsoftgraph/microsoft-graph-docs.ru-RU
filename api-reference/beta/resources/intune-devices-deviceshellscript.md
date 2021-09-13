---
title: Тип ресурса deviceShellScript
description: Intune предоставит клиенту возможность запускать свои скрипты Shell на зарегистрированных устройствах Mac OS. Сценарий можно запускать один раз или периодически.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cc3553e5b2ca63f7d202b1cf197429815363780e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125829"
---
# <a name="deviceshellscript-resource-type"></a>Тип ресурса deviceShellScript

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность запускать свои скрипты Shell на зарегистрированных устройствах Mac OS. Сценарий можно запускать один раз или периодически.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список устройствShellScripts](../api/intune-devices-deviceshellscript-list.md)|[коллекция deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Список свойств и связей объектов [deviceShellScript.](../resources/intune-devices-deviceshellscript.md)|
|[Get deviceShellScript](../api/intune-devices-deviceshellscript-get.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Чтение свойств и связей [объекта deviceShellScript.](../resources/intune-devices-deviceshellscript.md)|
|[Создание deviceShellScript](../api/intune-devices-deviceshellscript-create.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Создание нового [объекта deviceShellScript.](../resources/intune-devices-deviceshellscript.md)|
|[Удаление deviceShellScript](../api/intune-devices-deviceshellscript-delete.md)|Нет|Удаляет [deviceShellScript](../resources/intune-devices-deviceshellscript.md).|
|[Обновление deviceShellScript](../api/intune-devices-deviceshellscript-update.md)|[deviceShellScript](../resources/intune-devices-deviceshellscript.md)|Обновление свойств объекта [deviceShellScript.](../resources/intune-devices-deviceshellscript.md)|
|[Действие assign](../api/intune-devices-deviceshellscript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|executionFrequency|Длительность|Интервал для запуска скрипта. Если сценарий не определен, он будет работать один раз|
|retryCount|Int32|Количество случаев повторного и повторного и повторного повторного и повторного списания сценария|
|blockExecutionNotifications|Логическое|Не уведомляет пользователя о выполнении сценария|
|id|String|Уникальный идентификатор для сценария управления устройствами.|
|displayName|String|Имя сценария управления устройствами.|
|description|String|Необязательное описание сценария управления устройствами.|
|scriptContent|В двоичном формате|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сценария управления устройствами. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|fileName|String|Имя файла скрипта.|
|roleScopeTagIds|Коллекция объектов string|Список ID-тегов области для этого экземпляра PowerShellScript.|

## <a name="relationships"></a>Связи
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



