---
title: Тип ресурса Букингкурренци
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c1d56dde0c239245f6724040229df7d417a79613
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508005"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="80d83-104">Тип ресурса Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="80d83-104">bookingCurrency resource type</span></span>

<span data-ttu-id="80d83-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="80d83-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="80d83-106">Представляет денежную валюту, поддерживаемую [букингбусинесс](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="80d83-106">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="80d83-107">Методы</span><span class="sxs-lookup"><span data-stu-id="80d83-107">Methods</span></span>

| <span data-ttu-id="80d83-108">Метод</span><span class="sxs-lookup"><span data-stu-id="80d83-108">Method</span></span>           | <span data-ttu-id="80d83-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="80d83-109">Return Type</span></span>    |<span data-ttu-id="80d83-110">Описание</span><span class="sxs-lookup"><span data-stu-id="80d83-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80d83-111">Список БукингкурренЦиес</span><span class="sxs-lookup"><span data-stu-id="80d83-111">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="80d83-112">Коллекция [букингкурренци](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="80d83-112">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="80d83-113">Получение списка объектов **букингкурренци** , доступных для корпоративных книг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="80d83-113">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="80d83-114">Получение Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="80d83-114">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="80d83-115">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="80d83-115">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="80d83-116">Получение свойств объекта **букингкурренци** .</span><span class="sxs-lookup"><span data-stu-id="80d83-116">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="80d83-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="80d83-117">Properties</span></span>
| <span data-ttu-id="80d83-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="80d83-118">Property</span></span>     | <span data-ttu-id="80d83-119">Тип</span><span class="sxs-lookup"><span data-stu-id="80d83-119">Type</span></span>   |<span data-ttu-id="80d83-120">Описание</span><span class="sxs-lookup"><span data-stu-id="80d83-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80d83-121">id</span><span class="sxs-lookup"><span data-stu-id="80d83-121">id</span></span>|<span data-ttu-id="80d83-122">String</span><span class="sxs-lookup"><span data-stu-id="80d83-122">String</span></span>| <span data-ttu-id="80d83-123">3-значный код валюты, основанный на [стандарте ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="80d83-123">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="80d83-124">Например, код валюты для доллара США равен USD, а Австралийский доллар — ауд.</span><span class="sxs-lookup"><span data-stu-id="80d83-124">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="80d83-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="80d83-125">Read-only.</span></span>|
|<span data-ttu-id="80d83-126">знаки</span><span class="sxs-lookup"><span data-stu-id="80d83-126">symbol</span></span>|<span data-ttu-id="80d83-127">String</span><span class="sxs-lookup"><span data-stu-id="80d83-127">String</span></span>| <span data-ttu-id="80d83-128">Символ валюты.</span><span class="sxs-lookup"><span data-stu-id="80d83-128">The currency symbol.</span></span> <span data-ttu-id="80d83-129">Например, символ денежной единицы для доллара США и Австралийский доллар — $.</span><span class="sxs-lookup"><span data-stu-id="80d83-129">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="80d83-130">Связи</span><span class="sxs-lookup"><span data-stu-id="80d83-130">Relationships</span></span>
<span data-ttu-id="80d83-131">Нет</span><span class="sxs-lookup"><span data-stu-id="80d83-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="80d83-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80d83-132">JSON representation</span></span>

<span data-ttu-id="80d83-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80d83-133">The following is a JSON representation of the resource.</span></span>

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
