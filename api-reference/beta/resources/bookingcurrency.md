---
title: Тип ресурса Букингкурренци
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: f7b12f8ac48457ed0ea36c2fec2aa39be2ff7a01
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013117"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="5d33d-104">Тип ресурса Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="5d33d-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="5d33d-105">Представляет денежную валюту, поддерживаемую [букингбусинесс](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="5d33d-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="5d33d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5d33d-106">Methods</span></span>

| <span data-ttu-id="5d33d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5d33d-107">Method</span></span>           | <span data-ttu-id="5d33d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5d33d-108">Return Type</span></span>    |<span data-ttu-id="5d33d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5d33d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5d33d-110">Список БукингкурренЦиес</span><span class="sxs-lookup"><span data-stu-id="5d33d-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="5d33d-111">Коллекция [букингкурренци](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="5d33d-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="5d33d-112">Получение списка объектов **букингкурренци** , доступных для корпоративных книг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5d33d-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="5d33d-113">Получение Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="5d33d-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="5d33d-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="5d33d-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="5d33d-115">Получение свойств объекта **букингкурренци** .</span><span class="sxs-lookup"><span data-stu-id="5d33d-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="5d33d-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d33d-116">Properties</span></span>
| <span data-ttu-id="5d33d-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d33d-117">Property</span></span>     | <span data-ttu-id="5d33d-118">Тип</span><span class="sxs-lookup"><span data-stu-id="5d33d-118">Type</span></span>   |<span data-ttu-id="5d33d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5d33d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d33d-120">id</span><span class="sxs-lookup"><span data-stu-id="5d33d-120">id</span></span>|<span data-ttu-id="5d33d-121">String</span><span class="sxs-lookup"><span data-stu-id="5d33d-121">String</span></span>| <span data-ttu-id="5d33d-122">3-значный код валюты, основанный на [стандарте ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="5d33d-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="5d33d-123">Например, код валюты для доллара США равен USD, а Австралийский доллар — ауд.</span><span class="sxs-lookup"><span data-stu-id="5d33d-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="5d33d-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5d33d-124">Read-only.</span></span>|
|<span data-ttu-id="5d33d-125">знаки</span><span class="sxs-lookup"><span data-stu-id="5d33d-125">symbol</span></span>|<span data-ttu-id="5d33d-126">String</span><span class="sxs-lookup"><span data-stu-id="5d33d-126">String</span></span>| <span data-ttu-id="5d33d-127">Символ валюты.</span><span class="sxs-lookup"><span data-stu-id="5d33d-127">The currency symbol.</span></span> <span data-ttu-id="5d33d-128">Например, символ денежной единицы для доллара США и Австралийский доллар — $.</span><span class="sxs-lookup"><span data-stu-id="5d33d-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="5d33d-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="5d33d-129">Relationships</span></span>
<span data-ttu-id="5d33d-130">Нет</span><span class="sxs-lookup"><span data-stu-id="5d33d-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5d33d-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d33d-131">JSON representation</span></span>

<span data-ttu-id="5d33d-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d33d-132">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
