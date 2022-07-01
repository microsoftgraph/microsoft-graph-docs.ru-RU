---
title: Тип ресурса deviceManagementScript
description: Intune предоставляет клиенту возможность запускать скрипты PowerShell на зарегистрированных устройствах, присоединенных к Azure Active Directory windows 10. Скрипт может выполняться один раз или периодически.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fbb6e2bc1cdbd2e567f124228a7ed56315bde71
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441743"
---
# <a name="devicemanagementscript-resource-type"></a>Тип ресурса deviceManagementScript

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставляет клиенту возможность запускать скрипты PowerShell на зарегистрированных устройствах, присоединенных к Azure Active Directory windows 10. Скрипт может выполняться один раз или периодически.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceManagementScript](../api/intune-shared-devicemanagementscript-list.md)|[Коллекция deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Список свойств и связей объектов [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|[Получение deviceManagementScript](../api/intune-shared-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Чтение свойств и связей объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|[Создание deviceManagementScript](../api/intune-shared-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Создайте объект [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|[Удаление deviceManagementScript](../api/intune-shared-devicemanagementscript-delete.md)|Нет|Удаляет [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).|
|[Обновление deviceManagementScript](../api/intune-shared-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)|Обновление свойств объекта [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .|
|**Управление устройствами**|
|[Действие assign](../api/intune-shared-devicemanagementscript-assign.md)|Нет|Н/Д|
|**Набор политик**|
|[Действие hasPayloadLinks](../api/intune-shared-devicemanagementscript-haspayloadlinks.md)|[Коллекция hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор скрипта управления устройствами.|
|displayName|String|Имя скрипта управления устройствами.|
|description|String|Необязательное описание скрипта управления устройствами.|
|scriptContent|Binary|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания скрипта управления устройствами. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения скрипта управления устройствами. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|enforceSignatureCheck|Логическое|Укажите, требуется ли проверять подпись скрипта.|
|fileName|String|Имя файла скрипта.|
|Идентификаторы roleScopeTagId|Коллекция String|Список идентификаторов тегов области для этого экземпляра PowerShellScript.|
|runAs32Bit|Логическое|Значение, указывающее, должен ли скрипт PowerShell выполняться как 32-разрядный|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Управление устройствами**|
|groupAssignments|[Коллекция deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Список назначений групп для скрипта управления устройствами.|
|assignments|[Коллекция deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Список назначений групп для скрипта управления устройствами.|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md);|Выполните сводку для скрипта управления устройствами.|
|deviceRunStates|[Коллекция deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|Список состояний выполнения для этого скрипта на всех устройствах.|
|userRunStates|[Коллекция deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|Список состояний выполнения для этого скрипта для всех пользователей.|

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



