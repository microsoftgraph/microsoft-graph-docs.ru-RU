---
title: Тип ресурса Девицекомплианцескриптрулиррор
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3fe2782ed50f0fcd67f6c4865e92803642909924
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729730"
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





