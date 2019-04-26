---
title: Тип ресурса Букингперсон
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b4f69fde11ce0717e7ac81bd2070d08cbb59a84a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338757"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="6d645-104">Тип ресурса Букингперсон</span><span class="sxs-lookup"><span data-stu-id="6d645-104">bookingPerson resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="6d645-105">Это базовый тип для человека в Microsoft Books бизнеса, который может быть [букингкустомер](bookingcustomer.md) или [букингстаффмембер](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="6d645-105">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6d645-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d645-106">Properties</span></span>
| <span data-ttu-id="6d645-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d645-107">Property</span></span>     | <span data-ttu-id="6d645-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6d645-108">Type</span></span>   |<span data-ttu-id="6d645-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6d645-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d645-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6d645-110">displayName</span></span>|<span data-ttu-id="6d645-111">Строка</span><span class="sxs-lookup"><span data-stu-id="6d645-111">String</span></span>|<span data-ttu-id="6d645-112">Имя производной сущности, которая взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="6d645-112">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="6d645-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6d645-113">emailAddress</span></span>|<span data-ttu-id="6d645-114">String</span><span class="sxs-lookup"><span data-stu-id="6d645-114">String</span></span>|<span data-ttu-id="6d645-115">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d645-115">The email address of the person.</span></span>|
|<span data-ttu-id="6d645-116">id</span><span class="sxs-lookup"><span data-stu-id="6d645-116">id</span></span>|<span data-ttu-id="6d645-117">String</span><span class="sxs-lookup"><span data-stu-id="6d645-117">String</span></span>| <span data-ttu-id="6d645-118">Идентификатор производной сущности.</span><span class="sxs-lookup"><span data-stu-id="6d645-118">The ID for the derived entity.</span></span> <span data-ttu-id="6d645-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6d645-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d645-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="6d645-120">Relationships</span></span>
<span data-ttu-id="6d645-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6d645-121">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6d645-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d645-122">JSON representation</span></span>

<span data-ttu-id="6d645-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d645-123">The following is a JSON representation of the resource.</span></span>

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
