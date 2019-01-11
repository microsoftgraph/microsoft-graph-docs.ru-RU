---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
ms.openlocfilehash: e4ee085882cadafc0102ee31e17841978cef7822
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836458"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="edf2e-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="edf2e-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="edf2e-103">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="edf2e-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="edf2e-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="edf2e-104">JSON representation</span></span>

<span data-ttu-id="edf2e-105">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edf2e-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="edf2e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="edf2e-106">Properties</span></span>

| <span data-ttu-id="edf2e-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="edf2e-107">Property name</span></span> | <span data-ttu-id="edf2e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="edf2e-108">Type</span></span>   | <span data-ttu-id="edf2e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="edf2e-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="edf2e-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="edf2e-110">**locale**</span></span>    | <span data-ttu-id="edf2e-111">string</span><span class="sxs-lookup"><span data-stu-id="edf2e-111">string</span></span> | <span data-ttu-id="edf2e-112">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="edf2e-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
