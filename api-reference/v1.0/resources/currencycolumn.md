---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: currencyColumn
ms.openlocfilehash: 4f3ae97e5abfb84ad523caf74fa70b1f1ec0322a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="9046a-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="9046a-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="9046a-103">Ресурс **currencyColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="9046a-103">The **currencyColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9046a-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9046a-104">JSON representation</span></span>

<span data-ttu-id="9046a-105">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9046a-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="9046a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9046a-106">Properties</span></span>

| <span data-ttu-id="9046a-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9046a-107">Property name</span></span> | <span data-ttu-id="9046a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9046a-108">Type</span></span>   | <span data-ttu-id="9046a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9046a-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="9046a-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="9046a-110">**Locale**</span></span>    | <span data-ttu-id="9046a-111">строка</span><span class="sxs-lookup"><span data-stu-id="9046a-111">string</span></span> | <span data-ttu-id="9046a-112">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="9046a-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
