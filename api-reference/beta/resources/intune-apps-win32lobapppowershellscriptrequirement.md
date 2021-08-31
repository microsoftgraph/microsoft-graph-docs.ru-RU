---
title: тип ресурса win32LobAppPowerShellScriptRequirement
description: Содержит свойства скрипта PowerShell для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3025ec2bd0ebc5eb4806f70d8672f4c6126f1d7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58771948"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a>тип ресурса win32LobAppPowerShellScriptRequirement

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства скрипта PowerShell для обнаружения приложения Win32


Наследует [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|Оператор обнаружения, унаследованный от [win32LobAppRequirement.](../resources/intune-apps-win32lobapprequirement.md) Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|detectionValue|Строка|Значение обнаружения, унаследованные от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|displayName|Строка|Уникальное имя отображения для этого правила|
|enforceSignatureCheck|Логический|Значение, указывающее, выполняется ли проверка подписи|
|runAs32Bit|Boolean|Значение, указывающее, должен ли этот скрипт работать как 32-битный|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения, в котором выполняется сценарий. Возможные значения: `system`, `user`.|
|scriptContent|Строка|Кодированное содержимое скрипта base64 для обнаружения приложения Win32 Line of Business (LoB)|
|detectionType|[win32LobAppPowerShellScriptDetectionType](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|Тип обнаружения для вывода скрипта. Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```



