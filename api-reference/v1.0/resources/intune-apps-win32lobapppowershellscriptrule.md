---
title: тип ресурса win32LobAppPowerShellScriptRule
description: Сложный тип для хранения данных правила скрипта PowerShell для приложения LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cdbb4c9fc9ec0c3a17e10e79ba782d61a562f9fc
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60446415"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a>тип ресурса win32LobAppPowerShellScriptRule

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сложный тип для хранения данных правила скрипта PowerShell для приложения LOB Win32.


Наследует [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|ruleType|[win32LobAppRuleType](../resources/intune-apps-win32lobappruletype.md)|Тип правила, указывающий цель правила. Унаследованный от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md). Возможные значения: `detection`, `requirement`.|
|displayName|String|Имя отображения правила. Не укажите это значение, если правило используется для обнаружения.|
|enforceSignatureCheck|Логический|Значение, указывающее, выполняется ли проверка подписи.|
|runAs32Bit|Логический|Значение, указывающее, должен ли скрипт работать как 32-битный.|
|runAsAccount|[runAsAccountType](../resources/intune-apps-runasaccounttype.md)|Контекст выполнения сценария. Не укажите это значение, если правило используется для обнаружения. Правила обнаружения скриптов будут работать в том же контексте, что и контекст установки связанного приложения. Возможные значения: `system`, `user`.|
|scriptContent|String|Содержимое скрипта с кодом base64.|
|operationType|[win32LobAppPowerShellScriptRuleOperationType](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|Тип операции сравнения вывода скрипта. Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения. Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|Оператор вывода скрипта. Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|String|Значение сравнения вывода скрипта. Не укажите значение, если правило используется для обнаружения.|

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



