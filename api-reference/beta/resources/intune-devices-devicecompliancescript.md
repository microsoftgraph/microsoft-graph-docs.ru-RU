---
title: Тип ресурса deviceComplianceScript
description: Intune предоставляет клиенту возможность запускать скрипты соответствия (обнаружения) PowerShell на зарегистрированных устройствах, присоединенных к Azure Active Directory windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 04349bd414df14ca1359ea42523a197754b12622
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66666881"
---
# <a name="devicecompliancescript-resource-type"></a>Тип ресурса deviceComplianceScript

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставляет клиенту возможность запускать скрипты соответствия (обнаружения) PowerShell на зарегистрированных устройствах, присоединенных к Azure Active Directory windows 10.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceComplianceScript](../api/intune-devices-devicecompliancescript-list.md)|[Коллекция deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Список свойств и связей объектов [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .|
|[Получение deviceComplianceScript](../api/intune-devices-devicecompliancescript-get.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Чтение свойств и связей объекта [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .|
|[Создание deviceComplianceScript](../api/intune-devices-devicecompliancescript-create.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Создайте объект [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .|
|[Удаление deviceComplianceScript](../api/intune-devices-devicecompliancescript-delete.md)|Нет|Удаляет [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md).|
|[Обновление deviceComplianceScript](../api/intune-devices-devicecompliancescript-update.md)|[deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md)|Обновление свойств объекта [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .|
|[Действие assign](../api/intune-devices-devicecompliancescript-assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор скрипта соответствия устройств|
|publisher|String|Имя издателя скрипта соответствия устройств|
|version|String|Версия сценария соответствия устройств|
|displayName|String|Имя скрипта соответствия устройств|
|description|String|Описание сценария соответствия устройств|
|detectionScriptContent|Binary|Все содержимое скрипта PowerShell для обнаружения|
|createdDateTime|DateTimeOffset|Метка времени создания скрипта соответствия устройств. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Метка времени изменения скрипта соответствия устройств. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-devices-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|enforceSignatureCheck|Логическое|Укажите, нужно ли проверять подпись скрипта|
|runAs32Bit|Логическое|Укажите, должны ли скрипты PowerShell выполняться как 32-разрядные|
|Идентификаторы roleScopeTagId|Коллекция String|Список идентификаторов тегов области для сценария соответствия устройств|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[Коллекция deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Список назначений групп для сценария соответствия устройств|
|runSummary|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Общие сведения о выполнении скрипта соответствия устройств.|
|deviceRunStates|[Коллекция deviceComplianceScriptDeviceState](../resources/intune-devices-devicecompliancescriptdevicestate.md)|Список состояний выполнения для скрипта соответствия устройств на всех устройствах|

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




