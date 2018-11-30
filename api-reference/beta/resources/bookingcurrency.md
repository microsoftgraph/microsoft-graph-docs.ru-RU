---
title: Тип ресурса bookingCurrency
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: a68b88160e42217f3605c4a4bb30f692e8dafc06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076261"
---
# <a name="bookingcurrency-resource-type"></a><span data-ttu-id="610a9-104">Тип ресурса bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="610a9-104">bookingCurrency resource type</span></span>

 > <span data-ttu-id="610a9-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="610a9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="610a9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="610a9-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="610a9-107">Представляет денежных валюты, поддерживаемый [bookingBusiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="610a9-107">Represents a monetary currency supported by a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="610a9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="610a9-108">Methods</span></span>

| <span data-ttu-id="610a9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="610a9-109">Method</span></span>           | <span data-ttu-id="610a9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="610a9-110">Return Type</span></span>    |<span data-ttu-id="610a9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="610a9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="610a9-112">Список bookingCurrencies</span><span class="sxs-lookup"><span data-stu-id="610a9-112">List bookingCurrencies</span></span>](../api/bookingcurrency-list.md) | <span data-ttu-id="610a9-113">[bookingCurrency](bookingcurrency.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="610a9-113">[bookingCurrency](bookingcurrency.md) collection</span></span> |<span data-ttu-id="610a9-114">Получите список объектов **bookingCurrency** , доступные для резервирования Microsoft business.</span><span class="sxs-lookup"><span data-stu-id="610a9-114">Get a list of **bookingCurrency** objects available to a Microsoft Bookings business.</span></span>|
|[<span data-ttu-id="610a9-115">Получение bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="610a9-115">Get bookingCurrency</span></span>](../api/bookingcurrency-get.md) | [<span data-ttu-id="610a9-116">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="610a9-116">bookingCurrency</span></span>](bookingcurrency.md) |<span data-ttu-id="610a9-117">Получение свойств объекта **bookingCurrency** .</span><span class="sxs-lookup"><span data-stu-id="610a9-117">Get the properties of a **bookingCurrency** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="610a9-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="610a9-118">Properties</span></span>
| <span data-ttu-id="610a9-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="610a9-119">Property</span></span>     | <span data-ttu-id="610a9-120">Тип</span><span class="sxs-lookup"><span data-stu-id="610a9-120">Type</span></span>   |<span data-ttu-id="610a9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="610a9-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="610a9-122">id</span><span class="sxs-lookup"><span data-stu-id="610a9-122">id</span></span>|<span data-ttu-id="610a9-123">String</span><span class="sxs-lookup"><span data-stu-id="610a9-123">String</span></span>| <span data-ttu-id="610a9-124">Код 3-символ валюты, на основании [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span><span class="sxs-lookup"><span data-stu-id="610a9-124">A 3-character currency code, based on [ISO 4217](https://www.iso.org/iso-4217-currency-codes.html).</span></span> <span data-ttu-id="610a9-125">К примеру код валюты доллара США — долларов США, а для Австралии доллар — AUD.</span><span class="sxs-lookup"><span data-stu-id="610a9-125">For example, the currency code for the US dollar is USD, and for the Australian dollar is AUD.</span></span> <span data-ttu-id="610a9-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="610a9-126">Read-only.</span></span>|
|<span data-ttu-id="610a9-127">символ</span><span class="sxs-lookup"><span data-stu-id="610a9-127">symbol</span></span>|<span data-ttu-id="610a9-128">String</span><span class="sxs-lookup"><span data-stu-id="610a9-128">String</span></span>| <span data-ttu-id="610a9-129">Символ валюты.</span><span class="sxs-lookup"><span data-stu-id="610a9-129">The currency symbol.</span></span> <span data-ttu-id="610a9-130">Например символ валюты доллара США, а также для Австралии доллар — $.</span><span class="sxs-lookup"><span data-stu-id="610a9-130">For example, the currency symbol for the US dollar and for the Australian dollar is $.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="610a9-131">Связи</span><span class="sxs-lookup"><span data-stu-id="610a9-131">Relationships</span></span>
<span data-ttu-id="610a9-132">Нет</span><span class="sxs-lookup"><span data-stu-id="610a9-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="610a9-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="610a9-133">JSON representation</span></span>

<span data-ttu-id="610a9-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="610a9-134">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingCurrency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->