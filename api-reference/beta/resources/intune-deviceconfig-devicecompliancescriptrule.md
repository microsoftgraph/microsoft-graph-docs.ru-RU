---
title: тип ресурса deviceComplianceScriptRule
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cdcb9209c71b42169962d35fe44ca2b6490ba2cd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106226"
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
|operand|String|Operand, указанный в правиле.|

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



