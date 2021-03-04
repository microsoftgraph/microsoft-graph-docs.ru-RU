---
author: swapnil1993
title: тип ресурса columnValidation
description: Содержит данные для проверки значений столбцов.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8c1b20b239b894aa0da63222bb69a8d720e5ab50
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447490"
---
# <a name="columnvalidation-resource-type"></a><span data-ttu-id="ce96a-103">тип ресурса columnValidation</span><span class="sxs-lookup"><span data-stu-id="ce96a-103">columnValidation resource type</span></span>

<span data-ttu-id="ce96a-104">Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="ce96a-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>
<span data-ttu-id="ce96a-105">Содержит метаданные для проверки столбца.</span><span class="sxs-lookup"><span data-stu-id="ce96a-105">Contains metadata for validating the column.</span></span>


## <a name="properties"></a><span data-ttu-id="ce96a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce96a-106">Properties</span></span>

| <span data-ttu-id="ce96a-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ce96a-107">Property name</span></span>  | <span data-ttu-id="ce96a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ce96a-108">Type</span></span>    | <span data-ttu-id="ce96a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ce96a-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="ce96a-110">**formula**</span><span class="sxs-lookup"><span data-stu-id="ce96a-110">**formula**</span></span>    | <span data-ttu-id="ce96a-111">string</span><span class="sxs-lookup"><span data-stu-id="ce96a-111">string</span></span>  | <span data-ttu-id="ce96a-112">Формула для проверки значения столбца.</span><span class="sxs-lookup"><span data-stu-id="ce96a-112">The formula to validate column value.</span></span> <span data-ttu-id="ce96a-113">Например, см. [примеры распространенных формул в списках](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3)</span><span class="sxs-lookup"><span data-stu-id="ce96a-113">For examples, see [Examples of common formulas in lists](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3)</span></span> 
| <span data-ttu-id="ce96a-114">**описания**</span><span class="sxs-lookup"><span data-stu-id="ce96a-114">**descriptions**</span></span>    | <span data-ttu-id="ce96a-115">Collection(microsoft.graph.displayNameLocalization)</span><span class="sxs-lookup"><span data-stu-id="ce96a-115">Collection(microsoft.graph.displayNameLocalization)</span></span>  | <span data-ttu-id="ce96a-116">Локализованные сообщения, объясняя, что необходимо для того, чтобы значение этого столбца считалось допустимым.</span><span class="sxs-lookup"><span data-stu-id="ce96a-116">Localized messages that explain what is needed for this column's value to be considered valid.</span></span> <span data-ttu-id="ce96a-117">В случае сбой проверки пользователю будет предложено это сообщение.</span><span class="sxs-lookup"><span data-stu-id="ce96a-117">User will be prompted with this message if validation fails.</span></span> 
| <span data-ttu-id="ce96a-118">**defaultLanguage**</span><span class="sxs-lookup"><span data-stu-id="ce96a-118">**defaultLanguage**</span></span>    | <span data-ttu-id="ce96a-119">string</span><span class="sxs-lookup"><span data-stu-id="ce96a-119">string</span></span>  | <span data-ttu-id="ce96a-120">Языковой тег BCP 47 по умолчанию для описания.</span><span class="sxs-lookup"><span data-stu-id="ce96a-120">Default BCP 47 language tag for the description.</span></span>

<span data-ttu-id="ce96a-121">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="ce96a-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="ce96a-122">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="ce96a-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce96a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce96a-123">JSON representation</span></span>

<span data-ttu-id="ce96a-124">Ниже приводится представление JSON ресурса **columnValidation.**</span><span class="sxs-lookup"><span data-stu-id="ce96a-124">The following is a JSON representation of a **columnValidation** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnValidation"} -->

```json
{
  "formula": "string",
  "descriptions": [{ "@type": "microsoft.graph.displayNameLocalization" }],
  "defaultLanguage": "string"
}
```

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3
