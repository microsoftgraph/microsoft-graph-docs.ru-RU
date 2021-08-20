---
title: тип ресурса deviceManagementScript
description: Intune предоставит клиенту возможность запускать свои скрипты Powershell на зарегистрированных устройствах Windows 10 Azure Active Directory. Сценарий можно запускать один раз или периодически.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a16f7634f0951649ae0a670c48e5598dbbf3c14d0fa1c06751e9d313ffe51f17
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206174"
---
# <a name="devicemanagementscript-resource-type"></a>тип ресурса deviceManagementScript

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность запускать свои скрипты Powershell на зарегистрированных устройствах Windows 10 Azure Active Directory. Сценарий можно запускать один раз или периодически.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScripts](../api/intune-shared-devicemanagementscript-list.md)|[коллекция deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список свойств и связей объектов [deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)|
|[Get deviceManagementScript](../api/intune-shared-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Чтение свойств и связей [объекта deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)|
|[Создание deviceManagementScript](../api/intune-shared-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Создание нового [объекта deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)|
|[Удаление deviceManagementScript](../api/intune-shared-devicemanagementscript-delete.md)|Нет|Удаляет [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).|
|[Обновление deviceManagementScript](../api/intune-shared-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Обновление свойств объекта [deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)|
|**Управление устройствами**|
|[Действие assign](../api/intune-shared-devicemanagementscript-assign.md)|Нет|Н/Д|
|**Набор политик**|
|[действие hasPayloadLinks](../api/intune-shared-devicemanagementscript-haspayloadlinks.md)|[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для сценария управления устройствами.|
|displayName|String|Имя сценария управления устройствами.|
|description|Строка|Необязательное описание сценария управления устройствами.|
|scriptContent|В двоичном формате|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сценария управления устройствами. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|enforceSignatureCheck|Логический|Указать, нужно ли проверять подпись скрипта.|
|fileName|String|Имя файла скрипта.|
|roleScopeTagIds|Коллекция String|Список ID-тегов области для этого экземпляра PowerShellScript.|
|runAs32Bit|Логический|Значение, указывающее, должен ли скрипт PowerShell работать как 32-битный|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление устройствами**|
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
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
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




