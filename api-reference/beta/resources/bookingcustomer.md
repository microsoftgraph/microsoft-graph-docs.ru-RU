---
title: Тип ресурса Букингкустомер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d996c5e06c5c12e3a5115253bb73ed4a7a450258
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645221"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="e0771-104">Тип ресурса Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="e0771-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="e0771-105">Представляет клиента объекта [букингбусинесс](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="e0771-105">Represents a customer of a [bookingBusiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="e0771-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e0771-106">Methods</span></span>

| <span data-ttu-id="e0771-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e0771-107">Method</span></span>           | <span data-ttu-id="e0771-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e0771-108">Return Type</span></span>    |<span data-ttu-id="e0771-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e0771-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0771-110">Перечисление клиентов</span><span class="sxs-lookup"><span data-stu-id="e0771-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="e0771-111">Коллекция [букингкустомер](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="e0771-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="e0771-112">Получение списка объектов **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="e0771-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="e0771-113">Создание Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="e0771-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="e0771-114">Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="e0771-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="e0771-115">Создание нового объекта **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="e0771-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="e0771-116">Получение Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="e0771-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="e0771-117">Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="e0771-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="e0771-118">Чтение свойств и связей объекта **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="e0771-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|<span data-ttu-id="e0771-119">[обновление](../api/bookingcustomer-update.md);</span><span class="sxs-lookup"><span data-stu-id="e0771-119">[Update](../api/bookingcustomer-update.md)</span></span> | [<span data-ttu-id="e0771-120">Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="e0771-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="e0771-121">Обновление объекта **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="e0771-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="e0771-122">Удаление</span><span class="sxs-lookup"><span data-stu-id="e0771-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="e0771-123">Нет</span><span class="sxs-lookup"><span data-stu-id="e0771-123">None</span></span> |<span data-ttu-id="e0771-124">Удаление объекта **букингкустомер** .</span><span class="sxs-lookup"><span data-stu-id="e0771-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e0771-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0771-125">Properties</span></span>
| <span data-ttu-id="e0771-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0771-126">Property</span></span>     | <span data-ttu-id="e0771-127">Тип</span><span class="sxs-lookup"><span data-stu-id="e0771-127">Type</span></span>   |<span data-ttu-id="e0771-128">Описание</span><span class="sxs-lookup"><span data-stu-id="e0771-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0771-129">displayName</span><span class="sxs-lookup"><span data-stu-id="e0771-129">displayName</span></span>|<span data-ttu-id="e0771-130">Строка</span><span class="sxs-lookup"><span data-stu-id="e0771-130">String</span></span>|<span data-ttu-id="e0771-131">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="e0771-131">The name of the customer.</span></span>|
|<span data-ttu-id="e0771-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e0771-132">emailAddress</span></span>|<span data-ttu-id="e0771-133">String</span><span class="sxs-lookup"><span data-stu-id="e0771-133">String</span></span>|<span data-ttu-id="e0771-134">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="e0771-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="e0771-135">id</span><span class="sxs-lookup"><span data-stu-id="e0771-135">id</span></span>|<span data-ttu-id="e0771-136">String</span><span class="sxs-lookup"><span data-stu-id="e0771-136">String</span></span>| <span data-ttu-id="e0771-137">Идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="e0771-137">The ID of the customer.</span></span> <span data-ttu-id="e0771-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e0771-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0771-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="e0771-139">Relationships</span></span>
<span data-ttu-id="e0771-140">Нет</span><span class="sxs-lookup"><span data-stu-id="e0771-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e0771-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0771-141">JSON representation</span></span>

<span data-ttu-id="e0771-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0771-142">The following is a JSON representation of the resource.</span></span>

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
