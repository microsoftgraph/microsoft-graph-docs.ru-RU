---
author: JeremyKelley
description: Ресурс currencyColumn в ресурсе columnDefinition указывает, что значения столбца представляют денежные значения.
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 61a3c968ff48cd3bf59ec3611bc2e50a1a92a797
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973176"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="94ce8-103">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="94ce8-103">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94ce8-104">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="94ce8-104">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94ce8-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="94ce8-105">JSON representation</span></span>

<span data-ttu-id="94ce8-106">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94ce8-106">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="94ce8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="94ce8-107">Properties</span></span>

| <span data-ttu-id="94ce8-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="94ce8-108">Property name</span></span> | <span data-ttu-id="94ce8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="94ce8-109">Type</span></span>   | <span data-ttu-id="94ce8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="94ce8-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="94ce8-111">**locale**</span><span class="sxs-lookup"><span data-stu-id="94ce8-111">**locale**</span></span>    | <span data-ttu-id="94ce8-112">string</span><span class="sxs-lookup"><span data-stu-id="94ce8-112">string</span></span> | <span data-ttu-id="94ce8-113">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="94ce8-113">Specifies the locale from which to infer the currency symbol.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": []
}
-->
