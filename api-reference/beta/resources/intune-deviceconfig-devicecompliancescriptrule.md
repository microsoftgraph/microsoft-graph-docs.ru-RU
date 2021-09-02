---
title: тип ресурса deviceComplianceScriptRule
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 723fa805042e055075a52a5a134e213f1feef3bc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801152"
---
# <a name="devicecompliancescriptrule-resource-type"></a>тип ресурса deviceComplianceScriptRule

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingName|String|Настройка имени, указанного в правиле.|
|operator|[operator](../resources/intune-deviceconfig-operator.md)|Оператор, указанный в правиле. Возможные значения: `none` `and` , `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` . `excludesAll`|
|deviceComplianceScriptRulOperator|[deviceComplianceScriptRulOperator](../resources/intune-deviceconfig-devicecompliancescriptruloperator.md)|Оператор, указанный в правиле. Возможные значения: `none` `and` , `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` . `excludesAll`|
|dataType|[DataType](../resources/intune-deviceconfig-datatype.md)|Тип данных, указанный в правиле. Возможные значения: `none` `boolean` , , , , , `int64` , `double` , `string` `dateTime` `version` `base64` `xml` , `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` , .|
|deviceComplianceScriptRuleDataType|[deviceComplianceScriptRuleDataType](../resources/intune-deviceconfig-devicecompliancescriptruledatatype.md)|Тип данных, указанный в правиле. Возможные значения: `none` `boolean` , , , , , `int64` , `double` , `string` `dateTime` `version` `base64` `xml` , `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` , .|
|operand|Строка|Operand, указанный в правиле.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRule",
  "settingName": "String",
  "operator": "String",
  "deviceComplianceScriptRulOperator": "String",
  "dataType": "String",
  "deviceComplianceScriptRuleDataType": "String",
  "operand": "String"
}
```



