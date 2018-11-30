---
title: Тип ресурса bookingNamedEntity
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 1d82fcf6fcf7ffad6e60baea3f3e1118ec60345d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075278"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="b8240-104">Тип ресурса bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="b8240-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="b8240-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b8240-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8240-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8240-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="b8240-107">Это базовый тип для резервирования Microsoft сущностей, которые обеспечивают отображаемое имя, например, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="b8240-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b8240-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8240-108">Properties</span></span>
| <span data-ttu-id="b8240-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8240-109">Property</span></span>     | <span data-ttu-id="b8240-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b8240-110">Type</span></span>   |<span data-ttu-id="b8240-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b8240-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8240-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b8240-112">displayName</span></span>|<span data-ttu-id="b8240-113">String</span><span class="sxs-lookup"><span data-stu-id="b8240-113">String</span></span>|<span data-ttu-id="b8240-114">Имя для производные сущности, который взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="b8240-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="b8240-115">id</span><span class="sxs-lookup"><span data-stu-id="b8240-115">id</span></span>|<span data-ttu-id="b8240-116">String</span><span class="sxs-lookup"><span data-stu-id="b8240-116">String</span></span>| <span data-ttu-id="b8240-117">Идентификатор производные сущности.</span><span class="sxs-lookup"><span data-stu-id="b8240-117">The ID for the derived entity.</span></span> <span data-ttu-id="b8240-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b8240-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8240-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b8240-119">Relationships</span></span>
<span data-ttu-id="b8240-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b8240-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b8240-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8240-121">JSON representation</span></span>

<span data-ttu-id="b8240-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8240-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingNamedEntity"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingNamedEntity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->