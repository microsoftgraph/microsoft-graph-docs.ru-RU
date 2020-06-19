---
title: Тип ресурса Девицекомплианцескриптруле
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5c524202b8e15d077895c47c1c66256d58ca2c3
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789423"
---
# <a name="devicecompliancescriptrule-resource-type"></a>Тип ресурса Девицекомплианцескриптруле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|settingName|String|Имя параметра, указанное в правиле.|
|operator|[or](../resources/intune-deviceconfig-operator.md)|Оператор, указанный в правиле. Возможные значения:,,,,,,,,,,, `none` `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` , `notBeginsWith` ,,, `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` ,, `excludesAll` ,,,,,,,,,,,,,.|
|dataType|[Типа](../resources/intune-deviceconfig-datatype.md)|Тип данных, указанный в правиле. Возможные значения: `none` , `boolean` ,,,,, `int64` `double` `string` `dateTime` `version` ,,, `base64` `xml` `booleanArray` , `int64Array` , `doubleArray` , `stringArray` , `dateTimeArray` , `versionArray` .|
|начинается|String|Операнд, указанный в правиле.|

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
  "dataType": "String",
  "operand": "String"
}
```



