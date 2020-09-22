---
title: Тип ресурса win32LobAppPowerShellScriptRule
description: Сложный тип для хранения данных правила скрипта PowerShell для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4857bbc8493e453785ba95336c2976fab0504381
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092827"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a>Тип ресурса win32LobAppPowerShellScriptRule

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения данных правила скрипта PowerShell для бизнес-приложения Win32.


Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|Тип правила, указывающий назначение правила. Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Возможные значения: `detection`, `requirement`.|
|displayName|Строка|Отображаемое имя правила. Не указывайте это значение, если правило используется для обнаружения.|
|Свойства enforcesignaturecheck|Boolean|Значение, указывающее, применяется ли проверка подписи.|
|runAs32Bit|Boolean|Значение, указывающее, должен ли скрипт выполняться как 32 бит.|
|runAsAccount|[рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Контекст выполнения скрипта. Не указывайте это значение, если правило используется для обнаружения. Правила определения скрипта будут выполняться в том же контексте, что и связанный контекст установки приложения. Возможные значения: `system`, `user`.|
|скриптконтент|Строка|Содержимое скрипта в кодировке Base64.|
|оператионтипе|[win32LobAppPowerShellScriptRuleOperationType](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|Тип операции сравнения выходных данных скрипта. Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения. Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|Оператор вывода скрипта. Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|компарисонвалуе|Строка|Значение для сравнения вывода скрипта. Не указывайте значение, если правило используется для обнаружения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRule",
  "ruleType": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```






