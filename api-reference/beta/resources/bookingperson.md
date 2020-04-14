---
title: Тип ресурса Букингперсон
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d5ebbd7c4abaf34b31ac3f3d8e75defd6c939ec0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453677"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="a178d-104">Тип ресурса Букингперсон</span><span class="sxs-lookup"><span data-stu-id="a178d-104">bookingPerson resource type</span></span>

<span data-ttu-id="a178d-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a178d-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="a178d-106">Это базовый тип для человека в Microsoft Books бизнеса, который может быть [букингкустомер](bookingcustomer.md) или [букингстаффмембер](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="a178d-106">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a178d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a178d-107">Properties</span></span>
| <span data-ttu-id="a178d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a178d-108">Property</span></span>     | <span data-ttu-id="a178d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a178d-109">Type</span></span>   |<span data-ttu-id="a178d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a178d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a178d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a178d-111">displayName</span></span>|<span data-ttu-id="a178d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="a178d-112">String</span></span>|<span data-ttu-id="a178d-113">Имя производной сущности, которая взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="a178d-113">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="a178d-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a178d-114">emailAddress</span></span>|<span data-ttu-id="a178d-115">String</span><span class="sxs-lookup"><span data-stu-id="a178d-115">String</span></span>|<span data-ttu-id="a178d-116">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="a178d-116">The email address of the person.</span></span>|
|<span data-ttu-id="a178d-117">id</span><span class="sxs-lookup"><span data-stu-id="a178d-117">id</span></span>|<span data-ttu-id="a178d-118">String</span><span class="sxs-lookup"><span data-stu-id="a178d-118">String</span></span>| <span data-ttu-id="a178d-119">Идентификатор производной сущности.</span><span class="sxs-lookup"><span data-stu-id="a178d-119">The ID for the derived entity.</span></span> <span data-ttu-id="a178d-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a178d-120">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a178d-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="a178d-121">Relationships</span></span>
<span data-ttu-id="a178d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a178d-122">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a178d-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a178d-123">JSON representation</span></span>

<span data-ttu-id="a178d-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a178d-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingPerson"
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
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
