---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
description: Ресурс currencyColumn в ресурсе columnDefinition указывает, что значения столбца представляют денежные значения.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1270900c11a65bf974ac78ffe6af37bf93c51af6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531743"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="ac06c-103">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="ac06c-103">CurrencyColumn resource type</span></span>

<span data-ttu-id="ac06c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac06c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac06c-105">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="ac06c-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac06c-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ac06c-106">JSON representation</span></span>

<span data-ttu-id="ac06c-107">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac06c-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="ac06c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac06c-108">Properties</span></span>

| <span data-ttu-id="ac06c-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="ac06c-109">Property name</span></span> | <span data-ttu-id="ac06c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ac06c-110">Type</span></span>   | <span data-ttu-id="ac06c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ac06c-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="ac06c-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="ac06c-112">**locale**</span></span>    | <span data-ttu-id="ac06c-113">string</span><span class="sxs-lookup"><span data-stu-id="ac06c-113">string</span></span> | <span data-ttu-id="ac06c-114">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="ac06c-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
