---
title: Тип ресурса win32LobAppPowerShellScriptRule
description: Сложный тип для хранения данных правила скрипта PowerShell для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c392d43f6e9836118f1d32320c5e63498226fed9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48712066"
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
|Свойства enforcesignaturecheck|Логический|Значение, указывающее, применяется ли проверка подписи.|
|runAs32Bit|Логический|Значение, указывающее, должен ли скрипт выполняться как 32 бит.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Контекст выполнения скрипта. Не указывайте это значение, если правило используется для обнаружения. Правила определения скрипта будут выполняться в том же контексте, что и связанный контекст установки приложения. Возможные значения: `system`, `user`.|
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





