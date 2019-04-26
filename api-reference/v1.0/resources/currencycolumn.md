---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: currencyColumn
localization_priority: Normal
ms.openlocfilehash: 065ac52a4d5216a4b3e62df892c8fe0a07a82ed0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574752"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="8b926-102">Тип ресурса currencyColumn</span><span class="sxs-lookup"><span data-stu-id="8b926-102">CurrencyColumn resource type</span></span>

<span data-ttu-id="8b926-103">Ресурс **currencyColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют денежные значения.</span><span class="sxs-lookup"><span data-stu-id="8b926-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b926-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8b926-104">JSON representation</span></span>

<span data-ttu-id="8b926-105">Ниже показано представление ресурса **currencyColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b926-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="8b926-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b926-106">Properties</span></span>

| <span data-ttu-id="8b926-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8b926-107">Property name</span></span> | <span data-ttu-id="8b926-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8b926-108">Type</span></span>   | <span data-ttu-id="8b926-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8b926-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8b926-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="8b926-110">**locale**</span></span>    | <span data-ttu-id="8b926-111">string</span><span class="sxs-lookup"><span data-stu-id="8b926-111">string</span></span> | <span data-ttu-id="8b926-112">Указывает языковой стандарт, на основании которого требуется выбрать обозначение денежной единицы.</span><span class="sxs-lookup"><span data-stu-id="8b926-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn"
} -->
