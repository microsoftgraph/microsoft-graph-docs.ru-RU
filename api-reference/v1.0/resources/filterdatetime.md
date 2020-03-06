---
title: Тип ресурса FilterDatetime
description: Представляет способ фильтрации даты при фильтрации по значениям.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9214e8ecde9b2c09e06cfcc6d6145ea5319eace9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531407"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="23736-103">Тип ресурса FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="23736-103">FilterDatetime resource type</span></span>

<span data-ttu-id="23736-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23736-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23736-105">Представляет способ фильтрации даты при фильтрации по значениям.</span><span class="sxs-lookup"><span data-stu-id="23736-105">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="23736-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="23736-106">Properties</span></span>
| <span data-ttu-id="23736-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="23736-107">Property</span></span>     | <span data-ttu-id="23736-108">Тип</span><span class="sxs-lookup"><span data-stu-id="23736-108">Type</span></span>   |<span data-ttu-id="23736-109">Описание</span><span class="sxs-lookup"><span data-stu-id="23736-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23736-110">дата</span><span class="sxs-lookup"><span data-stu-id="23736-110">date</span></span>|<span data-ttu-id="23736-111">строка</span><span class="sxs-lookup"><span data-stu-id="23736-111">string</span></span>|<span data-ttu-id="23736-112">Дата в формате ISO8601, используемая для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="23736-112">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="23736-113">specificity</span><span class="sxs-lookup"><span data-stu-id="23736-113">specificity</span></span>|<span data-ttu-id="23736-114">string</span><span class="sxs-lookup"><span data-stu-id="23736-114">string</span></span>|<span data-ttu-id="23736-115">Точность, с которой производится фильтрация данных на основе даты.</span><span class="sxs-lookup"><span data-stu-id="23736-115">How specific the date should be used to keep data.</span></span> <span data-ttu-id="23736-116">Например, если указана дата 2005-04-02, а для свойства specificity задано значение month, после фильтрации останутся все строки, датированные апрелем 2009 г.</span><span class="sxs-lookup"><span data-stu-id="23736-116">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="23736-117">Допустимые значения: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="23736-117">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23736-118">Связи</span><span class="sxs-lookup"><span data-stu-id="23736-118">Relationships</span></span>
<span data-ttu-id="23736-119">Нет</span><span class="sxs-lookup"><span data-stu-id="23736-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="23736-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23736-120">JSON representation</span></span>

<span data-ttu-id="23736-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23736-121">Here is a JSON representation of the resource.</span></span>

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
