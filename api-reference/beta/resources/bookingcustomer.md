---
title: Тип ресурса bookingCustomer
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522219"
---
# <a name="bookingcustomer-resource-type"></a><span data-ttu-id="8a535-104">Тип ресурса bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8a535-104">bookingCustomer resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="8a535-105">Представляет клиента [bookingBsiness](bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="8a535-105">Represents a customer of a [bookingBsiness](bookingbusiness.md).</span></span>


## <a name="methods"></a><span data-ttu-id="8a535-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8a535-106">Methods</span></span>

| <span data-ttu-id="8a535-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8a535-107">Method</span></span>           | <span data-ttu-id="8a535-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a535-108">Return Type</span></span>    |<span data-ttu-id="8a535-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8a535-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a535-110">Список клиентов</span><span class="sxs-lookup"><span data-stu-id="8a535-110">List customers</span></span>](../api/bookingbusiness-list-customers.md) | <span data-ttu-id="8a535-111">[bookingCustomer](bookingcustomer.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8a535-111">[bookingCustomer](bookingcustomer.md) collection</span></span> | <span data-ttu-id="8a535-112">Получите список объектов **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8a535-112">Get a list of **bookingCustomer** objects.</span></span> |
|[<span data-ttu-id="8a535-113">Создание bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8a535-113">Create bookingCustomer</span></span>](../api/bookingbusiness-post-customers.md) | [<span data-ttu-id="8a535-114">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8a535-114">bookingCustomer</span></span>](bookingcustomer.md) | <span data-ttu-id="8a535-115">Создание нового объекта **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8a535-115">Create a new **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="8a535-116">Получение bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8a535-116">Get bookingCustomer</span></span>](../api/bookingcustomer-get.md) | [<span data-ttu-id="8a535-117">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8a535-117">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="8a535-118">Чтение свойства и связи объекта **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8a535-118">Read the properties and relationships of a **bookingCustomer** object.</span></span>|
|[<span data-ttu-id="8a535-119">Update</span><span class="sxs-lookup"><span data-stu-id="8a535-119">Update</span></span>](../api/bookingcustomer-update.md) | [<span data-ttu-id="8a535-120">bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8a535-120">bookingCustomer</span></span>](bookingcustomer.md) |<span data-ttu-id="8a535-121">Обновление объекта **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8a535-121">Update a **bookingCustomer** object.</span></span> |
|[<span data-ttu-id="8a535-122">Delete</span><span class="sxs-lookup"><span data-stu-id="8a535-122">Delete</span></span>](../api/bookingcustomer-delete.md) | <span data-ttu-id="8a535-123">Нет</span><span class="sxs-lookup"><span data-stu-id="8a535-123">None</span></span> |<span data-ttu-id="8a535-124">Удалите объект **bookingCustomer** .</span><span class="sxs-lookup"><span data-stu-id="8a535-124">Delete a **bookingCustomer** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a535-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a535-125">Properties</span></span>
| <span data-ttu-id="8a535-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a535-126">Property</span></span>     | <span data-ttu-id="8a535-127">Тип</span><span class="sxs-lookup"><span data-stu-id="8a535-127">Type</span></span>   |<span data-ttu-id="8a535-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8a535-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a535-129">displayName</span><span class="sxs-lookup"><span data-stu-id="8a535-129">displayName</span></span>|<span data-ttu-id="8a535-130">String</span><span class="sxs-lookup"><span data-stu-id="8a535-130">String</span></span>|<span data-ttu-id="8a535-131">Имя клиента.</span><span class="sxs-lookup"><span data-stu-id="8a535-131">The name of the customer.</span></span>|
|<span data-ttu-id="8a535-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8a535-132">emailAddress</span></span>|<span data-ttu-id="8a535-133">String</span><span class="sxs-lookup"><span data-stu-id="8a535-133">String</span></span>|<span data-ttu-id="8a535-134">SMTP-адрес клиента.</span><span class="sxs-lookup"><span data-stu-id="8a535-134">The SMTP address of the customer.</span></span>|
|<span data-ttu-id="8a535-135">id</span><span class="sxs-lookup"><span data-stu-id="8a535-135">id</span></span>|<span data-ttu-id="8a535-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8a535-136">String</span></span>| <span data-ttu-id="8a535-137">Идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="8a535-137">The ID of the customer.</span></span> <span data-ttu-id="8a535-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a535-138">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a535-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="8a535-139">Relationships</span></span>
<span data-ttu-id="8a535-140">Нет</span><span class="sxs-lookup"><span data-stu-id="8a535-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8a535-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a535-141">JSON representation</span></span>

<span data-ttu-id="8a535-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a535-142">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcustomer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
