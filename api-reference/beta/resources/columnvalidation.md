---
author: swapnil1993
title: тип ресурса columnValidation
description: Содержит данные для проверки значений столбцов.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 20bf526aff4f10b0b9b16a31e9912b5695602db6
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63721726"
---
# <a name="columnvalidation-resource-type"></a>тип ресурса columnValidation

Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Содержит метаданные для проверки столбца.

## <a name="properties"></a>Свойства

| Свойство            | Тип                                                | Описание                                                                                                                                                                                                               |
| :------------------ | :-------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **formula**         | string                                              | Формула для проверки значения столбца. Например, см. [примеры распространенных формул в списках](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3) |
| **описания**    | Collection(microsoft.graph.displayNameLocalization) | Локализованные сообщения, объясняя, что необходимо для того, чтобы значение этого столбца считалось допустимым. В случае сбой проверки пользователю будет предложено это сообщение.                                                               |
| **defaultLanguage** | строка                                              | Языковой тег BCP 47 по умолчанию для описания.                                                                                                                                                                          |

В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.
Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].

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
