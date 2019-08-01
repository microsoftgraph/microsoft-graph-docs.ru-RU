---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
description: Ресурс currencyColumn в ресурсе columnDefinition указывает, что значения столбца представляют денежные значения.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d01ae79c8c271f1076d14e44f5f4cb5b147f4b79
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029570"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="5b0e9-103">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="5b0e9-103">CurrencyColumn resource type</span></span>

<span data-ttu-id="5b0e9-104">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="5b0e9-104">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b0e9-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5b0e9-105">JSON representation</span></span>

<span data-ttu-id="5b0e9-106">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b0e9-106">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="5b0e9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b0e9-107">Properties</span></span>

| <span data-ttu-id="5b0e9-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5b0e9-108">Property name</span></span> | <span data-ttu-id="5b0e9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5b0e9-109">Type</span></span>   | <span data-ttu-id="5b0e9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5b0e9-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5b0e9-111">**locale**</span><span class="sxs-lookup"><span data-stu-id="5b0e9-111">**locale**</span></span>    | <span data-ttu-id="5b0e9-112">string</span><span class="sxs-lookup"><span data-stu-id="5b0e9-112">string</span></span> | <span data-ttu-id="5b0e9-113">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="5b0e9-113">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
