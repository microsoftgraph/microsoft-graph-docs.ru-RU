---
title: Тип ресурса bookingPerson
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 606e0e0d1d851fac16b25310b278ca524124eb00
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845579"
---
# <a name="bookingperson-resource-type"></a><span data-ttu-id="eb6dd-104">Тип ресурса bookingPerson</span><span class="sxs-lookup"><span data-stu-id="eb6dd-104">bookingPerson resource type</span></span>

 > <span data-ttu-id="eb6dd-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eb6dd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb6dd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb6dd-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="eb6dd-107">Это базовый тип для пользователя в business резервирования Майкрософт, который может быть [bookingCustomer](bookingcustomer.md) или [bookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="eb6dd-107">This is a base type for a person in a Microsoft Bookings business, which can be a [bookingCustomer](bookingcustomer.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="eb6dd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb6dd-108">Properties</span></span>
| <span data-ttu-id="eb6dd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb6dd-109">Property</span></span>     | <span data-ttu-id="eb6dd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eb6dd-110">Type</span></span>   |<span data-ttu-id="eb6dd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eb6dd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb6dd-112">displayName</span><span class="sxs-lookup"><span data-stu-id="eb6dd-112">displayName</span></span>|<span data-ttu-id="eb6dd-113">Строка</span><span class="sxs-lookup"><span data-stu-id="eb6dd-113">String</span></span>|<span data-ttu-id="eb6dd-114">Имя для производные сущности, который взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="eb6dd-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="eb6dd-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="eb6dd-115">emailAddress</span></span>|<span data-ttu-id="eb6dd-116">String</span><span class="sxs-lookup"><span data-stu-id="eb6dd-116">String</span></span>|<span data-ttu-id="eb6dd-117">Адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="eb6dd-117">The email address of the person.</span></span>|
|<span data-ttu-id="eb6dd-118">id</span><span class="sxs-lookup"><span data-stu-id="eb6dd-118">id</span></span>|<span data-ttu-id="eb6dd-119">Строка</span><span class="sxs-lookup"><span data-stu-id="eb6dd-119">String</span></span>| <span data-ttu-id="eb6dd-120">Идентификатор производные сущности.</span><span class="sxs-lookup"><span data-stu-id="eb6dd-120">The ID for the derived entity.</span></span> <span data-ttu-id="eb6dd-121">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="eb6dd-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb6dd-122">Связи</span><span class="sxs-lookup"><span data-stu-id="eb6dd-122">Relationships</span></span>
<span data-ttu-id="eb6dd-123">Нет</span><span class="sxs-lookup"><span data-stu-id="eb6dd-123">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="eb6dd-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb6dd-124">JSON representation</span></span>

<span data-ttu-id="eb6dd-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb6dd-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingPerson resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
