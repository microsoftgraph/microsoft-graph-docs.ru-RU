---
title: тип ресурса displayNameLocalization
description: Предоставляет администратору возможность настроить строку, используемую в совместном Microsoft 365.
ms.localizationpriority: medium
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c20e4a9478c25a785253f47e86cb0f84db649e0f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072549"
---
# <a name="displaynamelocalization-resource-type"></a>тип ресурса displayNameLocalization

Предоставляет администратору возможность настроить строку, используемую в совместном Microsoft 365.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName   |Строка       | Если это поле присутствует, то значение этого поля содержит строку **displayName,** заданной для языка, присутствуют в **поле languageTag.**|
|LanguageTag   |Строка       | Предоставляет языковой культурный код и удобное имя языка, на который было предоставлено поле **displayName.**                  |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.displayNameLocalization",
  "baseType": null
}-->

```json
{
  "displayName": "string",
  "languageTag": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "displayNameLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


