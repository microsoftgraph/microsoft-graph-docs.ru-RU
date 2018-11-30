---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: currencyColumn
ms.openlocfilehash: 21c95026eb61eb68c98010d8ac288be115e95ec8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082524"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="585eb-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="585eb-102">CurrencyColumn resource type</span></span>

> <span data-ttu-id="585eb-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="585eb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="585eb-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="585eb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="585eb-105">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="585eb-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="585eb-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="585eb-106">JSON representation</span></span>

<span data-ttu-id="585eb-107">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="585eb-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="585eb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="585eb-108">Properties</span></span>

| <span data-ttu-id="585eb-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="585eb-109">Property name</span></span> | <span data-ttu-id="585eb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="585eb-110">Type</span></span>   | <span data-ttu-id="585eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="585eb-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="585eb-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="585eb-112">**locale**</span></span>    | <span data-ttu-id="585eb-113">строка</span><span class="sxs-lookup"><span data-stu-id="585eb-113">string</span></span> | <span data-ttu-id="585eb-114">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="585eb-114">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
