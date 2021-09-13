---
title: тип ресурса win32LobAppPowerShellScriptRule
description: Сложный тип для хранения данных правила скрипта PowerShell для приложения LOB Win32.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffd41dc3de305396a7596e6fb0569982ac489bb5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021710"
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
|displayName|Строка|Имя отображения правила. Не укажите это значение, если правило используется для обнаружения.|
|enforceSignatureCheck|Логический|Значение, указывающее, выполняется ли проверка подписи.|
|runAs32Bit|Boolean|Значение, указывающее, должен ли скрипт работать как 32-битный.|
|runAsAccount|[runAsAccountType](../resources/intune-apps-runasaccounttype.md)|Контекст выполнения сценария. Не укажите это значение, если правило используется для обнаружения. Правила обнаружения скриптов будут работать в том же контексте, что и контекст установки связанного приложения. Возможные значения: `system`, `user`.|
|scriptContent|Строка|Содержимое скрипта с кодом base64.|
|operationType|[win32LobAppPowerShellScriptRuleOperationType](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|Тип операции сравнения вывода скрипта. Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения. Возможные значения: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|operator|[win32LobAppRuleOperator](../resources/intune-apps-win32lobappruleoperator.md)|Оператор вывода скрипта. Используйте NotConfigured (значение по умолчанию), если правило используется для обнаружения. Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|comparisonValue|Строка|Значение сравнения вывода скрипта. Не укажите значение, если правило используется для обнаружения.|

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




