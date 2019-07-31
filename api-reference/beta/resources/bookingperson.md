---
title: Тип ресурса Букингперсон
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3c8db7aca957878247193207e00e969d8ddfc98e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974168"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="0cde3-104">Тип ресурса Букингперсон</span><span class="sxs-lookup"><span data-stu-id="0cde3-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="0cde3-105">Это базовый тип для человека в Microsoft Books бизнеса, который может быть [букингкустомер](bookingcustomer.md) или [букингстаффмембер](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="0cde3-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0cde3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cde3-106">Properties</span></span>
| <span data-ttu-id="0cde3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cde3-107">Property</span></span>     | <span data-ttu-id="0cde3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0cde3-108">Type</span></span>   |<span data-ttu-id="0cde3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0cde3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cde3-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0cde3-110">displayName</span></span>|<span data-ttu-id="0cde3-111">Строка</span><span class="sxs-lookup"><span data-stu-id="0cde3-111">String</span></span>|<span data-ttu-id="0cde3-112">Имя производной сущности, которая взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="0cde3-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="0cde3-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0cde3-113">emailAddress</span></span>|<span data-ttu-id="0cde3-114">String</span><span class="sxs-lookup"><span data-stu-id="0cde3-114">String</span></span>|<span data-ttu-id="0cde3-115">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="0cde3-115">The email address of the person.</span></span>|
|<span data-ttu-id="0cde3-116">id</span><span class="sxs-lookup"><span data-stu-id="0cde3-116">id</span></span>|<span data-ttu-id="0cde3-117">String</span><span class="sxs-lookup"><span data-stu-id="0cde3-117">String</span></span>| <span data-ttu-id="0cde3-118">Идентификатор производной сущности.</span><span class="sxs-lookup"><span data-stu-id="0cde3-118">The ID for the derived entity.</span></span> <span data-ttu-id="0cde3-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0cde3-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cde3-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="0cde3-120">Relationships</span></span>
<span data-ttu-id="0cde3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0cde3-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0cde3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0cde3-122">JSON representation</span></span>

<span data-ttu-id="0cde3-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0cde3-123">The following is a JSON representation of the resource.</span></span>

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
