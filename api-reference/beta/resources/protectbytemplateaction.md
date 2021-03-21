---
title: тип ресурса protectByTemplateAction
description: Информирует приложение о том, что должен применяться шаблон защиты от информационных данных Azure.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6524774af3faa496b141e37ec270f8a73770ee63
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956829"
---
# <a name="protectbytemplateaction-resource-type"></a>тип ресурса protectByTemplateAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Информирует приложение о том, что должен применяться шаблон защиты от информационных данных Azure. **ProtectionByTemplateAction** может быть возвращена с помощью [оценкиApplication](../api/informationprotectionlabel-evaluateapplication.md) или [evaluateClassificationResults,](../api/informationprotectionlabel-evaluateclassificationresults.md) если в результате метка настроена на применение защиты. Потребляющие приложения должны считыть шаблонId из результата, а затем использовать клиентскую библиотеку, например SDK Microsoft Information Protection, для применения защиты с помощью Azure Information Protection.

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

