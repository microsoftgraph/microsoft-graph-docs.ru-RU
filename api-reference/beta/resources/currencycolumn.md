---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
ms.openlocfilehash: 8b39f20830da6621b1b6379674d5ef191afe5d9f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341029"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="fe25b-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="fe25b-102">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe25b-103">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="fe25b-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe25b-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe25b-104">JSON representation</span></span>

<span data-ttu-id="fe25b-105">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe25b-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="fe25b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe25b-106">Properties</span></span>

| <span data-ttu-id="fe25b-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="fe25b-107">Property name</span></span> | <span data-ttu-id="fe25b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fe25b-108">Type</span></span>   | <span data-ttu-id="fe25b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fe25b-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="fe25b-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="fe25b-110">**locale**</span></span>    | <span data-ttu-id="fe25b-111">string</span><span class="sxs-lookup"><span data-stu-id="fe25b-111">string</span></span> | <span data-ttu-id="fe25b-112">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="fe25b-112">Specifies the locale from which to infer the currency symbol.</span></span>

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
