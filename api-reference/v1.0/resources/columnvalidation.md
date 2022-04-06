---
author: swapnil1993
title: тип ресурса columnValidation
description: Содержит данные, которые проверяют значения столбцов.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 41136c74347e0acdfe41b5b8fd9a5ddc1501a08b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757852"
---
# <a name="columnvalidation-resource-type"></a>тип ресурса columnValidation

Пространство имен: microsoft.graph

Представляет свойства, которые проверяют значения столбцов.
## <a name="properties"></a>Свойства

| Свойство  | Тип    | Описание|
|:---------------|:--------|:--------------------------------------------------|
| **formula**    | string  | Формула для проверки значения столбца. Примеры см. в [примере общих формул в списках](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3).|
| **описания**    | Collection(microsoft.graph.displayNameLocalization)  | Локализованные сообщения, объясняя, что необходимо для того, чтобы значение этого столбца считалось допустимым. В случае сбой проверки пользователю будет предложено это сообщение. |
| **defaultLanguage**    | String  | Языковой тег BCP 47 по умолчанию для описания.|

В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.
Дополнительные сведения см. [в примере общих формул в SharePoint Списки][SPFormulas].

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON ресурса **columnValidation** .
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnValidation"} -->

```json
{
  "formula": "string",
  "descriptions": [{ "@type": "microsoft.graph.displayNameLocalization" }],
  "defaultLanguage": "string"
}
```

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3
