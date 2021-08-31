---
title: тип ресурса deviceHealthScript
description: Intune предоставит клиенту возможность запускать свои скрипты Powershell Health (исправление + обнаружение) на зарегистрированных устройствах Windows 10 Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0a8dd615f783be39f02949d9535bcefdda5d2b64
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58799460"
---
# <a name="devicehealthscript-resource-type"></a>тип ресурса deviceHealthScript

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Intune предоставит клиенту возможность запускать свои скрипты Powershell Health (исправление + обнаружение) на зарегистрированных устройствах Windows 10 Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список устройствHealthScripts](../api/intune-devices-devicehealthscript-list.md)|[коллекция deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Список свойств и связей [объектов deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)|
|[Get deviceHealthScript](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Чтение свойств и связей [объекта deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)|
|[Создание deviceHealthScript](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Создайте новый [объект deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)|
|[Удаление deviceHealthScript](../api/intune-devices-devicehealthscript-delete.md)|Нет|Удаляет [устройствоHealthScript](../resources/intune-devices-devicehealthscript.md).|
|[Обновление устройстваHealthScript](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|Обновление свойств объекта [deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)|
|[Действие assign](../api/intune-devices-devicehealthscript-assign.md)|Нет|Н/Д|
|[updateGlobalScript action](../api/intune-devices-devicehealthscript-updateglobalscript.md)|Строка|Обновление скрипта здоровья несвободных устройств|
|[getGlobalScriptHighestAvailableVersion action](../api/intune-devices-devicehealthscript-getglobalscripthighestavailableversion.md)|Строка|Обновление скрипта здоровья несвободных устройств|
|[включить действиеGlobalScripts](../api/intune-devices-devicehealthscript-enableglobalscripts.md)|Нет|Н/Д|
|[areGlobalScriptsAvailable function](../api/intune-devices-devicehealthscript-areglobalscriptsavailable.md)|[globalDeviceHealthScriptState](../resources/intune-devices-globaldevicehealthscriptstate.md)|Пока не задокументировано.|
|[функция getRemediationSummary](../api/intune-devices-devicehealthscript-getremediationsummary.md)|[deviceHealthScriptRemediationSummary](../resources/intune-devices-devicehealthscriptremediationsummary.md)|Пока не задокументировано.|
|[функция getRemediationHistory](../api/intune-devices-devicehealthscript-getremediationhistory.md)|[deviceHealthScriptRemediationHistory](../resources/intune-devices-devicehealthscriptremediationhistory.md)|Функция получения количества исправлений скриптами для здоровья устройств|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для скрипта здоровья устройств|
|publisher|String|Имя издателя скриптов для здоровья устройств|
|version|String|Версия сценария состояния устройства|
|displayName|String|Имя сценария состояния устройства|
|description|Строка|Описание сценария состояния устройства|
|detectionScriptContent|В двоичном формате|Все содержимое сценария powershell обнаружения|
|remediationScriptContent|В двоичном формате|Все содержимое сценария powershell исправлений|
|createdDateTime|DateTimeOffset|Время создания скрипта здоровья устройства. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Время изменения скрипта здоровья устройства. Это свойство доступно только для чтения.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|enforceSignatureCheck|Логический|Указать, нужно ли проверять подпись скрипта|
|runAs32Bit|Boolean|Указать, должен ли сценарий PowerShell работать как 32-битный|
|roleScopeTagIds|Коллекция String|Список ID-тегов области для скрипта здоровья устройств|
|isGlobalScript|Логический|Определяет, является ли это microsoft Proprietary Script. Несвободные скрипты являются только для чтения|
|highestAvailableVersion|String|Самая доступная версия для сценария Microsoft Proprietary|
|detectionScriptParameters|[коллекция deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|Список объектов ComplexType DetectionScriptParameters.|
|remediationScriptParameters|[коллекция deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)|Список объектов ComplexType RemediationScriptParameters.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md)|Список групповых назначений для скрипта здоровья устройств|
|runSummary|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Сводка для скрипта здоровья устройств на высоком уровне.|
|deviceRunStates|[коллекция deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md)|Список состояния запуска для скрипта здоровья устройств на всех устройствах|

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



