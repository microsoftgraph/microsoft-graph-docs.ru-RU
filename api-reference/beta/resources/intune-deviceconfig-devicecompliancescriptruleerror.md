---
title: Тип ресурса Девицекомплианцескриптрулиррор
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fcb57fb187e41ac7d451f7cdd4bda09481ab6933
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260245"
---
# <a name="devicecompliancescriptruleerror-resource-type"></a>Тип ресурса Девицекомплианцескриптрулиррор

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.


Наследуется от [девицекомплианцескриптеррор](../resources/intune-deviceconfig-devicecompliancescripterror.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|[code](../resources/intune-deviceconfig-code.md)|Код ошибки. Наследуется от [девицекомплианцескриптеррор](../resources/intune-deviceconfig-devicecompliancescripterror.md). Допустимые значения:,,,,,,,,,,, `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` , `moreInfoUriInvalid` , `moreInfoUriTooLarge` , `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,.|
|message|String|Сообщение об ошибке. Наследуется от [девицекомплианцескриптеррор](../resources/intune-deviceconfig-devicecompliancescripterror.md)|
|settingName|String|Имя параметра для правила с ошибкой.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRuleError",
  "code": "String",
  "message": "String",
  "settingName": "String"
}
```




