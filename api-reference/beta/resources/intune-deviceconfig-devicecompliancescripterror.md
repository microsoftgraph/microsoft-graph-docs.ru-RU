---
title: Тип ресурса Девицекомплианцескриптеррор
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd8a801d34bb5a7ad07c7e769d25fa0a05e31a53
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260260"
---
# <a name="devicecompliancescripterror-resource-type"></a>Тип ресурса Девицекомплианцескриптеррор

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|code|[code](../resources/intune-deviceconfig-code.md)|Код ошибки. Допустимые значения:,,,,,,,,,,, `none` `jsonFileInvalid` `jsonFileMissing` `jsonFileTooLarge` `rulesMissing` `duplicateRules` `tooManyRulesSpecified` `operatorMissing` `operatorNotSupported` `datatypeMissing` `datatypeNotSupported` `operatorDataTypeCombinationNotSupported` `moreInfoUriMissing` , `moreInfoUriInvalid` , `moreInfoUriTooLarge` , `descriptionMissing` `descriptionInvalid` `descriptionTooLarge` `titleMissing` `titleInvalid` `titleTooLarge` `operandMissing` `operandInvalid` `operandTooLarge` `settingNameMissing` `settingNameInvalid` `settingNameTooLarge` `englishLocaleMissing` `duplicateLocales` `unrecognizedLocale` `unknown` `remediationStringsMissing` ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,.|
|message|String|Сообщение об ошибке.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptError",
  "code": "String",
  "message": "String"
}
```




