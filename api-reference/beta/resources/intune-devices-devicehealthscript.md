---
title: Тип ресурса deviceHealthScript
description: Intune предоставляет клиенту возможность запускать свои скрипты PowerShell Health (исправление и обнаружение) на зарегистрированных устройствах, присоединенных к Azure Active Directory windows 10.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01250fa2ad479de8fbe37eed627fbda2b6ddb24c
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670816"
---
# <a name="devicehealthscript-resource-type"></a>Тип ресурса deviceHealthScript

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставляет клиенту возможность запускать свои скрипты PowerShell Health (исправление и обнаружение) на зарегистрированных устройствах, присоединенных к Azure Active Directory windows 10.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceHealthScript](../api/intune-devices-devicehealthscript-list.md)|[Коллекция deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Список свойств и связей объектов [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Получение deviceHealthScript](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Чтение свойств и связей объекта [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Создание deviceHealthScript](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Создайте объект [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Удаление deviceHealthScript](../api/intune-devices-devicehealthscript-delete.md)|Нет|Удаляет [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).|
|[Обновление deviceHealthScript](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Обновление свойств объекта [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .|
|[Действие assign](../api/intune-devices-devicehealthscript-assign.md)|Нет|Н/Д|
|[Действие updateGlobalScript](../api/intune-devices-devicehealthscript-updateglobalscript.md)|String|Обновление скрипта работоспособности защищаемой системы устройства|
|[Действие getGlobalScriptHighestAvailableVersion](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|String|Обновление скрипта работоспособности защищаемой системы устройства|
|[Действие enableGlobalScripts](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|Нет|Н/Д|
|[Функция areGlobalScriptsAvailable](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[globalDeviceHealthScriptState](../resources/intune-devices-globaldevicehealthscriptstate.md)|Пока не задокументировано.|
|[Функция getRemediationSummary](../api/intune-devices-devicehealthscript-getremediationsummary.md)|[deviceHealthScriptRemediationSummary](../resources/intune-devices-devicehealthscriptremediationsummary.md)|Пока не задокументировано.|
|[Функция getRemediationHistory](../api/intune-devices-devicehealthscript-getremediationhistory.md)|[deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md)|Функция для получения количества исправлений с помощью скриптов работоспособности устройства|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор скрипта работоспособности устройства|
|publisher|String|Имя издателя скрипта работоспособности устройства|
|version|String|Версия скрипта работоспособности устройства|
|displayName|String|Имя скрипта работоспособности устройства|
|description|String|Описание сценария работоспособности устройства|
|detectionScriptContent|Binary|Все содержимое скрипта PowerShell для обнаружения|
|remediationScriptContent|Binary|Все содержимое скрипта PowerShell для исправления|
|createdDateTime|DateTimeOffset|Метка времени создания скрипта работоспособности устройства. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Метка времени изменения скрипта работоспособности устройства. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-devices-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|enforceSignatureCheck|Логическое|Укажите, нужно ли проверять подпись скрипта|
|runAs32Bit|Логическое|Укажите, должны ли скрипты PowerShell выполняться как 32-разрядные|
|Идентификаторы roleScopeTagId|Коллекция String|Список идентификаторов тегов области для скрипта работоспособности устройства|
|isGlobalScript|Логическое|Определяет, является ли это проприетарным скриптом Майкрософт. Собственные скрипты доступны только для чтения|
|highestAvailableVersion|String|Наивысшая доступная версия для проприетарного скрипта Майкрософт|
|detectionScriptParameters|[Коллекция deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|Список объектов ComplexType DetectionScriptParameters.|
|remediationScriptParameters|[Коллекция deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|Список объектов ComplexType RemediationScriptParameters.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[Коллекция deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Список назначений групп для скрипта работоспособности устройства|
|runSummary|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Высокоуровневая сводка по выполнению скрипта работоспособности устройства.|
|deviceRunStates|[Коллекция deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Список состояний выполнения для скрипта работоспособности устройства на всех устройствах|

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
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "binary",
  "remediationScriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "String"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "String",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "String",
      "description": "String",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "String"
    }
  ]
}
```




