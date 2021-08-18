---
title: тип ресурса deviceComplianceScriptValidationResult
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2f6a7d25551f386d17d8882f9c693079e0a5b788de3af2de868ce9ede56d4c4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54245039"
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




