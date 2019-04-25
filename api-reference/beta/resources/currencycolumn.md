---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
ms.openlocfilehash: f38fc2a29a5fdee77456a5ceee7c7689cfe3f412
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543233"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="4d289-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="4d289-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="4d289-103">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="4d289-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d289-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4d289-104">JSON representation</span></span>

<span data-ttu-id="4d289-105">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d289-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="4d289-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d289-106">Properties</span></span>

| <span data-ttu-id="4d289-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="4d289-107">Property name</span></span> | <span data-ttu-id="4d289-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4d289-108">Type</span></span>   | <span data-ttu-id="4d289-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4d289-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="4d289-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="4d289-110">**locale**</span></span>    | <span data-ttu-id="4d289-111">string</span><span class="sxs-lookup"><span data-stu-id="4d289-111">string</span></span> | <span data-ttu-id="4d289-112">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="4d289-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
