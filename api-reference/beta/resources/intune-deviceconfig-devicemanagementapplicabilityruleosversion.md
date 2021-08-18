---
title: тип ресурса deviceManagementApplicabilityRuleOsVersion
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f5dcb07caf8a9a92835b4019515fbc3cb90f24ef6d3aca94d2ed0cdaaa9f317
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54242946"
---
# <a name="devicemanagementapplicabilityruleosversion-resource-type"></a>тип ресурса deviceManagementApplicabilityRuleOsVersion

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|minOSVersion|String|Min OS version for Applicability Rule.|
|maxOSVersion|Строка|Версия Max OS для правила применимости.|
|name|String|Имя объекта.|
|ruleType|[deviceManagementApplicabilityRuleType](../resources/intune-deviceconfig-devicemanagementapplicabilityruletype.md)|Тип правила применимости. Возможные значения: `include`, `exclude`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
  "minOSVersion": "String",
  "maxOSVersion": "String",
  "name": "String",
  "ruleType": "String"
}
```




