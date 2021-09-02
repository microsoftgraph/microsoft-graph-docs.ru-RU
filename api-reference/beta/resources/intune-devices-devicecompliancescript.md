---
title: тип ресурса deviceComplianceScript
description: Intune предоставит клиенту возможность запускать свои скрипты соответствия требованиям Powershell (обнаружение) на зарегистрированных устройствах windows 10 Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e3c29d21784032e970d083ab4ee0300f57332a2
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58791503"
---
# <a name="devicecompliancescript-resource-type"></a>тип ресурса deviceComplianceScript

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность запускать свои скрипты соответствия требованиям Powershell (обнаружение) на зарегистрированных устройствах windows 10 Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список устройствComplianceScripts](../api/intune-devices-devicecompliancescript-list.md)|[коллекция deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Список свойств и связей объектов [deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)|
|[Get deviceComplianceScript](../api/intune-devices-devicecompliancescript-get.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Чтение свойств и связей [объекта deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)|
|[Создание deviceComplianceScript](../api/intune-devices-devicecompliancescript-create.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Создайте новый [объект deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)|
|[Удаление deviceComplianceScript](../api/intune-devices-devicecompliancescript-delete.md)|Нет|Удаляет [устройствоComplianceScript](../resources/intune-devices-devicecompliancescript.md).|
|[Обновление deviceComplianceScript](../api/intune-devices-devicecompliancescript-update.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Обновление свойств объекта [deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)|
|[Действие assign](../api/intune-devices-devicecompliancescript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сценария соответствия требованиям к устройству|
|publisher|String|Имя издателя сценариев соответствия требованиям устройств|
|version|String|Версия сценария соответствия требованиям устройства|
|displayName|Строка|Имя сценария соответствия требованиям устройства|
|description|Строка|Описание сценария соответствия требованиям устройства|
|detectionScriptContent|В двоичном формате|Все содержимое сценария powershell обнаружения|
|createdDateTime|DateTimeOffset|Время создания сценария соответствия требованиям устройства. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Время изменения сценария соответствия требованиям устройства. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|enforceSignatureCheck|Логический|Указать, нужно ли проверять подпись скрипта|
|runAs32Bit|Логический|Указать, должен ли сценарий PowerShell работать как 32-битный|
|roleScopeTagIds|Коллекция String|Список ID-тегов области для сценария соответствия требованиям к устройству|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Список групповых назначений для сценария соответствия требованиям к устройству|
|runSummary|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Сводка выполнения на высоком уровне для сценария соответствия требованиям устройств.|
|deviceRunStates|[коллекция deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Список состояния выполнения для сценария соответствия требованиям устройств на всех устройствах|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "String (identifier)",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```



