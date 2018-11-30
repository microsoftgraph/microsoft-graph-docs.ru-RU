---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: currencyColumn
ms.openlocfilehash: 796bd9fc7bf379ea38dc2d2f602411740caf4b86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028179"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="55cbf-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="55cbf-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="55cbf-103">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="55cbf-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55cbf-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="55cbf-104">JSON representation</span></span>

<span data-ttu-id="55cbf-105">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55cbf-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="55cbf-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="55cbf-106">Properties</span></span>

| <span data-ttu-id="55cbf-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="55cbf-107">Property name</span></span> | <span data-ttu-id="55cbf-108">Тип</span><span class="sxs-lookup"><span data-stu-id="55cbf-108">Type</span></span>   | <span data-ttu-id="55cbf-109">Описание</span><span class="sxs-lookup"><span data-stu-id="55cbf-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="55cbf-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="55cbf-110">**locale**</span></span>    | <span data-ttu-id="55cbf-111">string</span><span class="sxs-lookup"><span data-stu-id="55cbf-111">string</span></span> | <span data-ttu-id="55cbf-112">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="55cbf-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
