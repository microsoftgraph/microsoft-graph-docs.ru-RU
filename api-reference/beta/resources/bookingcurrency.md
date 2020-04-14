---
title: Тип ресурса Букингкурренци
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 6d04522b3a754e5a929fd48f8ea3c94f6ee5a6c3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453764"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="5c223-104">Тип ресурса Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="5c223-104">bookingCurrency resource type</span></span>

<span data-ttu-id="5c223-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c223-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="5c223-106">Представляет денежную валюту, поддерживаемую [букингбусинесс](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="5c223-106">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="5c223-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5c223-107">Methods</span></span>

| <span data-ttu-id="5c223-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5c223-108">Method</span></span>           | <span data-ttu-id="5c223-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c223-109">Return Type</span></span>    |<span data-ttu-id="5c223-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c223-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5c223-111">Список БукингкурренЦиес</span><span class="sxs-lookup"><span data-stu-id="5c223-111">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="5c223-112">Коллекция [букингкурренци](bookingcurrency.md)</span><span class="sxs-lookup"><span data-stu-id="5c223-112">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="5c223-113">Получение списка объектов **букингкурренци** , доступных для корпоративных книг Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5c223-113">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="5c223-114">Получение Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="5c223-114">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="5c223-115">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="5c223-115">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="5c223-116">Получение свойств объекта **букингкурренци** .</span><span class="sxs-lookup"><span data-stu-id="5c223-116">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="5c223-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c223-117">Properties</span></span>
| <span data-ttu-id="5c223-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c223-118">Property</span></span>     | <span data-ttu-id="5c223-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5c223-119">Type</span></span>   |<span data-ttu-id="5c223-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5c223-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c223-121">id</span><span class="sxs-lookup"><span data-stu-id="5c223-121">id</span></span>|<span data-ttu-id="5c223-122">String</span><span class="sxs-lookup"><span data-stu-id="5c223-122">String</span></span>| <span data-ttu-id="5c223-123">3-значный код валюты, основанный на [стандарте ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="5c223-123">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="5c223-124">Например, код валюты для доллара США равен USD, а Австралийский доллар — ауд.</span><span class="sxs-lookup"><span data-stu-id="5c223-124">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="5c223-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c223-125">Read-only.</span></span>|
|<span data-ttu-id="5c223-126">знаки</span><span class="sxs-lookup"><span data-stu-id="5c223-126">symbol</span></span>|<span data-ttu-id="5c223-127">String</span><span class="sxs-lookup"><span data-stu-id="5c223-127">String</span></span>| <span data-ttu-id="5c223-128">Символ валюты.</span><span class="sxs-lookup"><span data-stu-id="5c223-128">The currency symbol.</span></span> <span data-ttu-id="5c223-129">Например, символ денежной единицы для доллара США и Австралийский доллар — $.</span><span class="sxs-lookup"><span data-stu-id="5c223-129">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="5c223-130">Связи</span><span class="sxs-lookup"><span data-stu-id="5c223-130">Relationships</span></span>
<span data-ttu-id="5c223-131">Нет</span><span class="sxs-lookup"><span data-stu-id="5c223-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5c223-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c223-132">JSON representation</span></span>

<span data-ttu-id="5c223-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c223-133">The following is a JSON representation of the resource.</span></span>

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
