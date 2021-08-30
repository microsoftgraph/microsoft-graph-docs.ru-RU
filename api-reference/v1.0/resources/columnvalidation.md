---
author: swapnil1993
title: тип ресурса columnValidation
description: Содержит данные, которые проверяют значения столбцов.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 5a92f15d4f8decf07f6791ee704f38f49d91fe00
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58696810"
---
# <a name="columnvalidation-resource-type"></a>тип ресурса columnValidation

Пространство имен: microsoft.graph

Представляет свойства, которые проверяют значения столбцов.
## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание|
|:---------------|:--------|:--------------------------------------------------|
| **formula**    | string  | Формула для проверки значения столбца. Примеры см. в [примерах распространенных формул в списках.](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3)|
| **описания**    | Collection(microsoft.graph.displayNameLocalization)  | Локализованные сообщения, объясняя, что необходимо для того, чтобы значение этого столбца считалось допустимым. В случае сбой проверки пользователю будет предложено это сообщение. |
| **defaultLanguage**    | string  | Языковой тег BCP 47 по умолчанию для описания.|

В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.
Дополнительные сведения см. [в примере распространенных формул в SharePoint списках.][SPFormulas]

## <a name="json-representation"></a>Представление JSON

Ниже приводится представление JSON ресурса **columnValidation.**
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnValidation"} -->

```json
{
  "formula": "string",
  "descriptions": [{ "@type": "microsoft.graph.displayNameLocalization" }],
  "defaultLanguage": "string"
}
```

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3
