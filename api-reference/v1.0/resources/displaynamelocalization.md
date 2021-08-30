---
title: тип ресурса displayNameLocalization
description: Предоставляет администратору возможность настроить строку, используемую в совместном Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a45c64d8cb80d94a702cfd4be57012949a7c86e3
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696736"
---
# <a name="displaynamelocalization-resource-type"></a>тип ресурса displayNameLocalization

Предоставляет администратору возможность настроить строку, используемую в совместном Microsoft 365.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName   |String       | Если это поле присутствует, то значение этого поля содержит строку **displayName,** заданной для языка, присутствуют в **поле languageTag.**|
|LanguageTag   |String       | Предоставляет языковой культурный код и удобное имя языка, на который было предоставлено поле **displayName.**                  |

## <a name="json-representation"></a>Представление JSON

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


