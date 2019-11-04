---
title: Тип ресурса Протектбитемплатеактион
description: Информирует приложение о том, что шаблон защиты Azure Information Protection должен быть применен.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a7a557dfd72dac9161ae29436f5fc96eb55075d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939076"
---
# <a name="protectbytemplateaction-resource-type"></a>Тип ресурса Протектбитемплатеактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Информирует приложение о том, что шаблон защиты Azure Information Protection должен быть применен. **протектионбитемплатеактион** может быть возвращено [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md) или [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) , если полученная метка настроена на применение защиты. Приложение-приложение должно прочитать templateId из результата, а затем использовать клиентскую библиотеку, например Microsoft Information Protection SDK, для применения защиты с помощью Azure Information Protection.

## <a name="properties"></a>Свойства

| Свойство   | Тип   | Описание                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| templateId | Строка | GUID шаблона Azure Information Protection для применения к данным. |

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