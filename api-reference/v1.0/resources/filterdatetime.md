---
title: Тип ресурса FilterDatetime
description: Представляет способ фильтрации даты при фильтрации по значениям.
localization_priority: Normal
ms.openlocfilehash: 26d42b45a2e9b9cdd279f33330a877a64ea1c8d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564248"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="d67ea-103">Тип ресурса FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="d67ea-103">FilterDatetime resource type</span></span>

<span data-ttu-id="d67ea-104">Представляет способ фильтрации даты при фильтрации по значениям.</span><span class="sxs-lookup"><span data-stu-id="d67ea-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="d67ea-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d67ea-105">Properties</span></span>
| <span data-ttu-id="d67ea-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d67ea-106">Property</span></span>     | <span data-ttu-id="d67ea-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d67ea-107">Type</span></span>   |<span data-ttu-id="d67ea-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d67ea-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d67ea-109">дата</span><span class="sxs-lookup"><span data-stu-id="d67ea-109">date</span></span>|<span data-ttu-id="d67ea-110">строка</span><span class="sxs-lookup"><span data-stu-id="d67ea-110">string</span></span>|<span data-ttu-id="d67ea-111">Дата в формате ISO8601, используемая для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="d67ea-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="d67ea-112">specificity</span><span class="sxs-lookup"><span data-stu-id="d67ea-112">specificity</span></span>|<span data-ttu-id="d67ea-113">string</span><span class="sxs-lookup"><span data-stu-id="d67ea-113">string</span></span>|<span data-ttu-id="d67ea-114">Точность, с которой производится фильтрация данных на основе даты.</span><span class="sxs-lookup"><span data-stu-id="d67ea-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="d67ea-115">Например, если указана дата 2005-04-02, а для свойства specificity задано значение month, после фильтрации останутся все строки, датированные апрелем 2009 г.</span><span class="sxs-lookup"><span data-stu-id="d67ea-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="d67ea-116">Возможные `Year`значения:, `Monday`, `Day`, `Hour`, `Minute`,. `Second`</span><span class="sxs-lookup"><span data-stu-id="d67ea-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d67ea-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="d67ea-117">Relationships</span></span>
<span data-ttu-id="d67ea-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d67ea-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d67ea-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d67ea-119">JSON representation</span></span>

<span data-ttu-id="d67ea-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d67ea-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
