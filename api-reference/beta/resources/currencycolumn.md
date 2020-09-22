---
author: JeremyKelley
description: Ресурс currencyColumn в ресурсе columnDefinition указывает, что значения столбца представляют денежные значения.
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 4cd887d4ca7e38ff6d22189760adf12e1479acb9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050026"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="7214e-103">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="7214e-103">CurrencyColumn resource type</span></span>

<span data-ttu-id="7214e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7214e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7214e-105">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="7214e-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7214e-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7214e-106">JSON representation</span></span>

<span data-ttu-id="7214e-107">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7214e-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="7214e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7214e-108">Properties</span></span>

| <span data-ttu-id="7214e-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7214e-109">Property name</span></span> | <span data-ttu-id="7214e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7214e-110">Type</span></span>   | <span data-ttu-id="7214e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7214e-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="7214e-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="7214e-112">**locale**</span></span>    | <span data-ttu-id="7214e-113">string</span><span class="sxs-lookup"><span data-stu-id="7214e-113">string</span></span> | <span data-ttu-id="7214e-114">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="7214e-114">Specifies the locale from which to infer the currency symbol.</span></span>

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


