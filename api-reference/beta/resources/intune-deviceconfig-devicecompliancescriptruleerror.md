---
title: тип ресурса deviceComplianceScriptRuleError
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8cb3deb625b3fc98a22622ae19f86acbca974455
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789335"
---
# <a name="devicecompliancescriptruleerror-resource-type"></a>тип ресурса deviceComplianceScriptRuleError

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.


Наследует от [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|[code](../resources/intune-deviceconfig-code.md)|Код ошибки. Наследуется [от deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md). Возможные значения: `none` `jsonFileInvalid` , `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` . `remediationStringsMissing`|
|deviceComplianceScriptRulesValidationError|[deviceComplianceScriptRulesValidationError](../resources/intune-deviceconfig-devicecompliancescriptrulesvalidationerror.md)|Код ошибки. Наследуется [от deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md). Возможные значения: `none` `jsonFileInvalid` , `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` `moreInfoUriInvalid` `moreInfoUriTooLarge` `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` . `remediationStringsMissing`|
|message|String|Сообщение об ошибке. Унаследованный от [deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)|
|settingName|String|Настройка имени правила с ошибкой.|

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
  "deviceComplianceScriptRulesValidationError": "String",
  "message": "String",
  "settingName": "String"
}
```



