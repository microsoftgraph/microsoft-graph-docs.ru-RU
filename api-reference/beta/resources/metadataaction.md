---
title: Тип ресурса Метадатаактион
description: Представляет метаданные, которые необходимо записать или удалить из файла.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55ddd644428662f6a646fd9c003761ab6f7c1e9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021387"
---
# <a name="metadataaction-resource-type"></a>Тип ресурса Метадатаактион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метаданные, которые необходимо записать или удалить из файла. **метадатаактион** могут возвращаться с помощью API [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md), [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md)и [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) . Действие информирует приложение использования определенных пар "ключ-значение", которые следует добавить в файл, или конкретные ключи метаданных, которые следует удалить из файла. Эти метаданные описывают файл или сведения, *помеченные как отмеченные*.

## <a name="properties"></a>Свойства

| Свойство         | Тип                                       | Описание                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| метадататоадд    | Коллекция [keyValuePair](keyvaluepair.md) | Коллекция пар "ключ-значение", которые следует добавить в файл.                  |
| метадататоремове | Коллекция String                          | Коллекция строк, указывающая, какие ключи необходимо удалить из метаданных файла. |

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

