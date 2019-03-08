---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: 065ac52a4d5216a4b3e62df892c8fe0a07a82ed0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481533"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="e2064-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="e2064-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="e2064-103">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="e2064-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2064-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e2064-104">JSON representation</span></span>

<span data-ttu-id="e2064-105">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2064-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="e2064-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2064-106">Properties</span></span>

| <span data-ttu-id="e2064-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e2064-107">Property name</span></span> | <span data-ttu-id="e2064-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e2064-108">Type</span></span>   | <span data-ttu-id="e2064-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e2064-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e2064-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="e2064-110">**locale**</span></span>    | <span data-ttu-id="e2064-111">string</span><span class="sxs-lookup"><span data-stu-id="e2064-111">string</span></span> | <span data-ttu-id="e2064-112">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="e2064-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
