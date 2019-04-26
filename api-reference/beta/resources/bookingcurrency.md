---
title: Тип ресурса Букингкурренци
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6ab74cff24e1f575166f6672523ecc5d94bc1826
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328237"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="84631-104">Тип ресурса Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="84631-104">bookingCurrency resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="84631-105">Представляет денежную валюту, поддерживаемую [букингбусинесс](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="84631-105">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="84631-106">Методы</span><span class="sxs-lookup"><span data-stu-id="84631-106">Methods</span></span>

| <span data-ttu-id="84631-107">Метод</span><span class="sxs-lookup"><span data-stu-id="84631-107">Method</span></span>           | <span data-ttu-id="84631-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="84631-108">Return Type</span></span>    |<span data-ttu-id="84631-109">Описание</span><span class="sxs-lookup"><span data-stu-id="84631-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84631-110">Список БукингкурренЦиес</span><span class="sxs-lookup"><span data-stu-id="84631-110">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="84631-111">Коллекция [букингкурренци](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="84631-111">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="84631-112">Получение списка объектов **букингкурренци** , доступных для корпоративных книг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="84631-112">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="84631-113">Получение Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="84631-113">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="84631-114">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="84631-114">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="84631-115">Получение свойств объекта **букингкурренци** .</span><span class="sxs-lookup"><span data-stu-id="84631-115">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="84631-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="84631-116">Properties</span></span>
| <span data-ttu-id="84631-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="84631-117">Property</span></span>     | <span data-ttu-id="84631-118">Тип</span><span class="sxs-lookup"><span data-stu-id="84631-118">Type</span></span>   |<span data-ttu-id="84631-119">Описание</span><span class="sxs-lookup"><span data-stu-id="84631-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84631-120">id</span><span class="sxs-lookup"><span data-stu-id="84631-120">id</span></span>|<span data-ttu-id="84631-121">String</span><span class="sxs-lookup"><span data-stu-id="84631-121">String</span></span>| <span data-ttu-id="84631-122">3-значный код валюты, основанный на [стандарте ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="84631-122">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="84631-123">Например, код валюты для доллара США равен USD, а Австралийский доллар — ауд.</span><span class="sxs-lookup"><span data-stu-id="84631-123">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="84631-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84631-124">Read-only.</span></span>|
|<span data-ttu-id="84631-125">знаки</span><span class="sxs-lookup"><span data-stu-id="84631-125">symbol</span></span>|<span data-ttu-id="84631-126">String</span><span class="sxs-lookup"><span data-stu-id="84631-126">String</span></span>| <span data-ttu-id="84631-127">Символ валюты.</span><span class="sxs-lookup"><span data-stu-id="84631-127">The currency symbol.</span></span> <span data-ttu-id="84631-128">Например, символ денежной единицы для доллара США и Австралийский доллар — $.</span><span class="sxs-lookup"><span data-stu-id="84631-128">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="84631-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="84631-129">Relationships</span></span>
<span data-ttu-id="84631-130">Нет</span><span class="sxs-lookup"><span data-stu-id="84631-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="84631-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84631-131">JSON representation</span></span>

<span data-ttu-id="84631-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84631-132">The following is a JSON representation of the resource.</span></span>

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
