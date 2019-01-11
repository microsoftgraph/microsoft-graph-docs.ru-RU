---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
ms.openlocfilehash: 179c0bb1e5c82d7f2af17dcbcae08be8726f2ecd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888937"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="5c0d5-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="5c0d5-102">CurrencyColumn resource type</span></span>

> <span data-ttu-id="5c0d5-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c0d5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c0d5-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c0d5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5c0d5-105">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="5c0d5-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c0d5-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5c0d5-106">JSON representation</span></span>

<span data-ttu-id="5c0d5-107">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c0d5-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="5c0d5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c0d5-108">Properties</span></span>

| <span data-ttu-id="5c0d5-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5c0d5-109">Property name</span></span> | <span data-ttu-id="5c0d5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5c0d5-110">Type</span></span>   | <span data-ttu-id="5c0d5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5c0d5-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5c0d5-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="5c0d5-112">**locale**</span></span>    | <span data-ttu-id="5c0d5-113">строка</span><span class="sxs-lookup"><span data-stu-id="5c0d5-113">string</span></span> | <span data-ttu-id="5c0d5-114">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="5c0d5-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
