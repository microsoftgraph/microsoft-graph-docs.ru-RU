---
title: Тип ресурса bookingNamedEntity
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: fa307d0ee07b43a44210fc6ceaf4c74a29999caa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860503"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="5c3c2-104">Тип ресурса bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="5c3c2-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="5c3c2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5c3c2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c3c2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c3c2-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="5c3c2-107">Это базовый тип для резервирования Microsoft сущностей, которые обеспечивают отображаемое имя, например, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="5c3c2-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5c3c2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c3c2-108">Properties</span></span>
| <span data-ttu-id="5c3c2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c3c2-109">Property</span></span>     | <span data-ttu-id="5c3c2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5c3c2-110">Type</span></span>   |<span data-ttu-id="5c3c2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5c3c2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c3c2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5c3c2-112">displayName</span></span>|<span data-ttu-id="5c3c2-113">Строка</span><span class="sxs-lookup"><span data-stu-id="5c3c2-113">String</span></span>|<span data-ttu-id="5c3c2-114">Имя для производные сущности, который взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="5c3c2-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="5c3c2-115">id</span><span class="sxs-lookup"><span data-stu-id="5c3c2-115">id</span></span>|<span data-ttu-id="5c3c2-116">Строка</span><span class="sxs-lookup"><span data-stu-id="5c3c2-116">String</span></span>| <span data-ttu-id="5c3c2-117">Идентификатор производные сущности.</span><span class="sxs-lookup"><span data-stu-id="5c3c2-117">The ID for the derived entity.</span></span> <span data-ttu-id="5c3c2-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c3c2-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c3c2-119">Связи</span><span class="sxs-lookup"><span data-stu-id="5c3c2-119">Relationships</span></span>
<span data-ttu-id="5c3c2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5c3c2-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5c3c2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c3c2-121">JSON representation</span></span>

<span data-ttu-id="5c3c2-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c3c2-122">The following is a JSON representation of the resource.</span></span>

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
