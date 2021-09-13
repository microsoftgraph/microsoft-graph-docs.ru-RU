---
title: тип ресурса deviceComplianceScriptValidationResult
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 549bebc23eb927879f21fa8ccd6bb4e023f05e89
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091750"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a>тип ресурса deviceComplianceScriptValidationResult

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|правила|[коллекция deviceComplianceScriptRule](../resources/intune-deviceconfig-devicecompliancescriptrule.md)|Parsed rules from json.|
|scriptErrors|[коллекция deviceComplianceScriptError](../resources/intune-deviceconfig-devicecompliancescripterror.md)|Ошибки в json для сценария.|
|ruleErrors|[коллекция deviceComplianceScriptRuleError](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)|Ошибки в json для сценария правил.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptValidationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptValidationResult",
  "rules": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRule",
      "settingName": "String",
      "operator": "String",
      "deviceComplianceScriptRulOperator": "String",
      "dataType": "String",
      "deviceComplianceScriptRuleDataType": "String",
      "operand": "String"
    }
  ],
  "scriptErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String"
    }
  ],
  "ruleErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
      "code": "String",
      "deviceComplianceScriptRulesValidationError": "String",
      "message": "String",
      "settingName": "String"
    }
  ]
}
```



