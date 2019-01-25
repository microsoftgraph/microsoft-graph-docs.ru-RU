---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
ms.openlocfilehash: c89d709c93eeee0003d193d620166f8abffd9d41
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524501"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="2f9b9-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="2f9b9-102">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f9b9-103">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="2f9b9-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f9b9-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2f9b9-104">JSON representation</span></span>

<span data-ttu-id="2f9b9-105">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f9b9-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="2f9b9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f9b9-106">Properties</span></span>

| <span data-ttu-id="2f9b9-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2f9b9-107">Property name</span></span> | <span data-ttu-id="2f9b9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2f9b9-108">Type</span></span>   | <span data-ttu-id="2f9b9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f9b9-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2f9b9-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="2f9b9-110">**locale**</span></span>    | <span data-ttu-id="2f9b9-111">string</span><span class="sxs-lookup"><span data-stu-id="2f9b9-111">string</span></span> | <span data-ttu-id="2f9b9-112">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="2f9b9-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/currencycolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
