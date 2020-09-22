---
title: Тип ресурса Протектбитемплатеактион
description: Информирует приложение о том, что шаблон защиты Azure Information Protection должен быть применен.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 19103cd07404677b680606a6fd0ec9d4caa43600
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993162"
---
# <a name="protectbytemplateaction-resource-type"></a>Тип ресурса Протектбитемплатеактион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Информирует приложение о том, что шаблон защиты Azure Information Protection должен быть применен. **протектионбитемплатеактион** может быть возвращено [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) или [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) , если полученная метка настроена на применение защиты. Приложение-приложение должно прочитать templateId из результата, а затем использовать клиентскую библиотеку, например Microsoft Information Protection SDK, для применения защиты с помощью Azure Information Protection.

## <a name="properties"></a>Свойства

| Свойство   | Тип   | Описание                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| templateId | String | GUID шаблона Azure Information Protection для применения к данным. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectByTemplateAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "templateId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "protectByTemplateAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

