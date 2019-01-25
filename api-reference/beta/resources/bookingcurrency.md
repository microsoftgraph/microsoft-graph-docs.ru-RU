---
title: Тип ресурса bookingCurrency
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9d4feac66e72c756173113101a88bf8bbe35563a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518200"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="55d42-104">Тип ресурса bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="55d42-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="55d42-105">Представляет денежных валюты, поддерживаемый [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="55d42-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="55d42-106">Методы</span><span class="sxs-lookup"><span data-stu-id="55d42-106">Methods</span></span>

| <span data-ttu-id="55d42-107">Метод</span><span class="sxs-lookup"><span data-stu-id="55d42-107">Method</span></span>           | <span data-ttu-id="55d42-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55d42-108">Return Type</span></span>    |<span data-ttu-id="55d42-109">Описание</span><span class="sxs-lookup"><span data-stu-id="55d42-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55d42-110">Список bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="55d42-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="55d42-111">[bookingCurrency](bookingcurrency.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="55d42-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="55d42-112">Получите список объектов **bookingCurrency** , доступные для резервирования Microsoft business.</span><span class="sxs-lookup"><span data-stu-id="55d42-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="55d42-113">Получение bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="55d42-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="55d42-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="55d42-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="55d42-115">Получение свойств объекта **bookingCurrency** .</span><span class="sxs-lookup"><span data-stu-id="55d42-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="55d42-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="55d42-116">Properties</span></span>
| <span data-ttu-id="55d42-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="55d42-117">Property</span></span>     | <span data-ttu-id="55d42-118">Тип</span><span class="sxs-lookup"><span data-stu-id="55d42-118">Type</span></span>   |<span data-ttu-id="55d42-119">Описание</span><span class="sxs-lookup"><span data-stu-id="55d42-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55d42-120">id</span><span class="sxs-lookup"><span data-stu-id="55d42-120">id</span></span>|<span data-ttu-id="55d42-121">String</span><span class="sxs-lookup"><span data-stu-id="55d42-121">String</span></span>| <span data-ttu-id="55d42-122">Код 3-символ валюты, на основании [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="55d42-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="55d42-123">К примеру код валюты доллара США — долларов США, а для Австралии доллар — AUD.</span><span class="sxs-lookup"><span data-stu-id="55d42-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="55d42-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55d42-124">Read-only.</span></span>|
|<span data-ttu-id="55d42-125">Symbol</span><span class="sxs-lookup"><span data-stu-id="55d42-125">symbol</span></span>|<span data-ttu-id="55d42-126">String</span><span class="sxs-lookup"><span data-stu-id="55d42-126">String</span></span>| <span data-ttu-id="55d42-127">Символ валюты.</span><span class="sxs-lookup"><span data-stu-id="55d42-127">The currency symbol.</span></span> <span data-ttu-id="55d42-128">Например символ валюты доллара США, а также для Австралии доллар — $.</span><span class="sxs-lookup"><span data-stu-id="55d42-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="55d42-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="55d42-129">Relationships</span></span>
<span data-ttu-id="55d42-130">Нет</span><span class="sxs-lookup"><span data-stu-id="55d42-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="55d42-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55d42-131">JSON representation</span></span>

<span data-ttu-id="55d42-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55d42-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCurrency"
}-->

```json
{
  "id": "String (identifier)",
  "symbol": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcurrency.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
