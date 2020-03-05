---
author: JeremyKelley
description: Ресурс currencyColumn в ресурсе columnDefinition указывает, что значения столбца представляют денежные значения.
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 75ef7125c55674b2feb6e617a40313b5bca242bc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507333"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="3ea51-103">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="3ea51-103">CurrencyColumn resource type</span></span>

<span data-ttu-id="3ea51-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3ea51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ea51-105">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="3ea51-105">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ea51-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3ea51-106">JSON representation</span></span>

<span data-ttu-id="3ea51-107">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ea51-107">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="3ea51-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ea51-108">Properties</span></span>

| <span data-ttu-id="3ea51-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="3ea51-109">Property name</span></span> | <span data-ttu-id="3ea51-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3ea51-110">Type</span></span>   | <span data-ttu-id="3ea51-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3ea51-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="3ea51-112">**locale**</span><span class="sxs-lookup"><span data-stu-id="3ea51-112">**locale**</span></span>    | <span data-ttu-id="3ea51-113">string</span><span class="sxs-lookup"><span data-stu-id="3ea51-113">string</span></span> | <span data-ttu-id="3ea51-114">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="3ea51-114">Specifies the locale from which to infer the currency symbol.</span></span>

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
