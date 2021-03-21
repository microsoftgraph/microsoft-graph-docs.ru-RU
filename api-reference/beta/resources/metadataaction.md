---
title: тип ресурса metadataAction
description: Представляет метаданные, которые будут написаны или удалены из файла.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 23305d8a3e1e89d198b4700e794dd264eabf003b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960399"
---
# <a name="metadataaction-resource-type"></a>тип ресурса metadataAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метаданные, которые будут написаны или удалены из файла. **MetadataAction** может быть возвращено с помощью API [evaluateRemoval,](../api/informationprotectionlabel-evaluateremoval.md) [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)и [evaluateClassificationResults.](../api/informationprotectionlabel-evaluateclassificationresults.md) Действие информирует о потребляемом приложении определенных пар ключей и значений, которые необходимо добавить в файл, или о конкретных ключах метаданных, которые должны быть удалены из файла. Эти метаданные описывают файл или сведения как *помеченные.*

## <a name="properties"></a>Свойства

| Свойство         | Тип                                       | Описание                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| metadataToAdd    | Коллекция [keyValuePair](keyvaluepair.md) | Коллекция пар ключевых значений, которые необходимо добавить в файл.                  |
| metadataToRemove | Коллекция строк                          | Коллекция строк, которые указывают, какие ключи следует удалить из метаданных файла. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "metadataToAdd": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "metadataToRemove": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "metadataAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

