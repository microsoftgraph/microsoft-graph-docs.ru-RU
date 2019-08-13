---
title: Тип ресурса Девицехеалсскрипткомплианцеруле
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8098582bd3e1b91a7e80af141e31847d2d3155cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371561"
---
# <a name="devicehealthscriptcompliancerule-resource-type"></a>Тип ресурса Девицехеалсскрипткомплианцеруле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|детектионтипе|[девицехеалсскриптдетектионтипе](../resources/intune-devices-devicehealthscriptdetectiontype.md)|Еще не задокументировано. Возможные значения: `notConfigured`, `string`.|
|operator|[девицехеалсскрипткомплианцерулеоператор](../resources/intune-devices-devicehealthscriptcomplianceruleoperator.md)|Еще не задокументировано. Возможные значения: `notConfigured`, `equal`, `notEqual`.|
|детектионвалуе|String|Н/Д|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptComplianceRule",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



