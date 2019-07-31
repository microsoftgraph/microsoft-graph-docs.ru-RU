---
title: Тип ресурса Букингкустомер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 864635014b3e215dabd11896922ca9e73a5e8cb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974173"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="fd595-104">Тип ресурса Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="fd595-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="fd595-105">Представляет клиента объекта [букингбусинесс](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="fd595-105">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="fd595-106">Методы</span><span class="sxs-lookup"><span data-stu-id="fd595-106">Methods</span></span>

| <span data-ttu-id="fd595-107">Метод</span><span class="sxs-lookup"><span data-stu-id="fd595-107">Method</span></span>           | <span data-ttu-id="fd595-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fd595-108">Return Type</span></span>    |<span data-ttu-id="fd595-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fd595-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd595-110">Перечисление клиентов</span><span class="sxs-lookup"><span data-stu-id="fd595-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="fd595-111">Коллекция [букингкустомер](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="fd595-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="fd595-112">Получение списка объектов **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="fd595-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="fd595-113">Создание Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="fd595-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="fd595-114">Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="fd595-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="fd595-115">Создание нового объекта **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="fd595-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="fd595-116">Получение Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="fd595-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="fd595-117">Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="fd595-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="fd595-118">Чтение свойств и связей объекта **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="fd595-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|<span data-ttu-id="fd595-119">[обновление](../api/bookingcustomer-update.md);</span><span class="sxs-lookup"><span data-stu-id="fd595-119">[Update](../api/bookingcustomer-update.md)</span></span> | [<span data-ttu-id="fd595-120">Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="fd595-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="fd595-121">Обновление объекта **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="fd595-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="fd595-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="fd595-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="fd595-123">Нет</span><span class="sxs-lookup"><span data-stu-id="fd595-123">None</span></span> |<span data-ttu-id="fd595-124">Удаление объекта **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="fd595-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fd595-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd595-125">Properties</span></span>
| <span data-ttu-id="fd595-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd595-126">Property</span></span>     | <span data-ttu-id="fd595-127">Тип</span><span class="sxs-lookup"><span data-stu-id="fd595-127">Type</span></span>   |<span data-ttu-id="fd595-128">Описание</span><span class="sxs-lookup"><span data-stu-id="fd595-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd595-129">displayName</span><span class="sxs-lookup"><span data-stu-id="fd595-129">displayName</span></span>|<span data-ttu-id="fd595-130">Строка</span><span class="sxs-lookup"><span data-stu-id="fd595-130">String</span></span>|<span data-ttu-id="fd595-131">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="fd595-131">The name of the customer.</span></span>|
|<span data-ttu-id="fd595-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fd595-132">emailAddress</span></span>|<span data-ttu-id="fd595-133">String</span><span class="sxs-lookup"><span data-stu-id="fd595-133">String</span></span>|<span data-ttu-id="fd595-134">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="fd595-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="fd595-135">id</span><span class="sxs-lookup"><span data-stu-id="fd595-135">id</span></span>|<span data-ttu-id="fd595-136">String</span><span class="sxs-lookup"><span data-stu-id="fd595-136">String</span></span>| <span data-ttu-id="fd595-137">Идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="fd595-137">The ID of the customer.</span></span> <span data-ttu-id="fd595-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd595-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd595-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="fd595-139">Relationships</span></span>
<span data-ttu-id="fd595-140">Нет</span><span class="sxs-lookup"><span data-stu-id="fd595-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fd595-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd595-141">JSON representation</span></span>

<span data-ttu-id="fd595-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd595-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
