---
title: Тип ресурса Девицекомплианцескриптвалидатионресулт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8bb60af47f7c06b17dcc54468aa48dd85215a3da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998777"
---
# <a name="devicecompliancescriptvalidationresult-resource-type"></a>Тип ресурса Девицекомплианцескриптвалидатионресулт

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|правила|Коллекция [девицекомплианцескриптруле](../resources/intune-deviceconfig-devicecompliancescriptrule.md)|Проанализированные правила из JSON.|
|скриптеррорс|Коллекция [девицекомплианцескриптеррор](../resources/intune-deviceconfig-devicecompliancescripterror.md)|Ошибки в JSON для скрипта.|
|рулиррорс|Коллекция [девицекомплианцескриптрулиррор](../resources/intune-deviceconfig-devicecompliancescriptruleerror.md)|Ошибки в JSON для сценария для правил.|

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
      "dataType": "String",
      "operand": "String"
    }
  ],
  "scriptErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptError",
      "code": "String",
      "message": "String"
    }
  ],
  "ruleErrors": [
    {
      "@odata.type": "microsoft.graph.deviceComplianceScriptRuleError",
      "code": "String",
      "message": "String",
      "settingName": "String"
    }
  ]
}
```






