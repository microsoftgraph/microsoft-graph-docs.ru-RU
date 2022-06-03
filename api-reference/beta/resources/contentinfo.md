---
title: Тип ресурса contentInfo
description: Представляет текущее состояние некоторых сведений, которые должны быть помечены.
ms.localizationpriority: medium
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7dc6c99e1c4c19564e17c406beca02971071c671
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884176"
---
# <a name="contentinfo-resource-type"></a>Тип ресурса contentInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет текущее состояние некоторых сведений, которые должны быть помечены. **contentInfo передается** в API [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md) и [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) , чтобы описать API текущее состояние информации. Эта **подробная версия contentInfo** определяет, какие метаданные, маркировку содержимого и защиту следует добавлять или удалять при применении, обновлении или удалении метки. 

## <a name="properties"></a>Свойства

| Свойство   | Тип                                       | Описание                                                                                                                     |
| :--------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------ |
| format     | String                                     | Возможные значения: `default`, `email`.                                                                                        |
| идентификатор | Строка                                     | Идентификатор, используемый для Аналитики Azure Information Protection.                                                                     |
| Метаданных   | Коллекция [keyValuePair](keyvaluepair.md) | Существующие метаданные Microsoft Purview Information Protection передаются в виде пар "ключ-значение", где ключом является MSIP_Label_GUID_PropName. |
| state      | String                                     | Возможные значения: `rest`, `motion`, `use`.                                                                                   |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.contentInfo",
  "baseType": null
}-->

```json
{
  "format": "String",
  "identifier": "String",
  "metadata": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contentInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

