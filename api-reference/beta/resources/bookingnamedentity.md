---
title: Тип ресурса bookingNamedEntity
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: abd5c9e85357caa6ba6cbbd52d67550a463e36e9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985783"
---
# <a name="bookingnamedentity-resource-type"></a><span data-ttu-id="5eb6a-104">Тип ресурса bookingNamedEntity</span><span class="sxs-lookup"><span data-stu-id="5eb6a-104">bookingNamedEntity resource type</span></span>

 > <span data-ttu-id="5eb6a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5eb6a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5eb6a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5eb6a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="5eb6a-107">Это базовый тип для резервирования Microsoft сущностей, которые обеспечивают отображаемое имя, например, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span><span class="sxs-lookup"><span data-stu-id="5eb6a-107">This is a base type for Microsoft Bookings entities that provide a display name, for example, [bookingBusiness](bookingbusiness.md), [bookingPerson](bookingperson.md), [bookingService](bookingservice.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5eb6a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5eb6a-108">Properties</span></span>
| <span data-ttu-id="5eb6a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5eb6a-109">Property</span></span>     | <span data-ttu-id="5eb6a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5eb6a-110">Type</span></span>   |<span data-ttu-id="5eb6a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5eb6a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5eb6a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5eb6a-112">displayName</span></span>|<span data-ttu-id="5eb6a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="5eb6a-113">String</span></span>|<span data-ttu-id="5eb6a-114">Имя для производные сущности, который взаимодействует с клиентами.</span><span class="sxs-lookup"><span data-stu-id="5eb6a-114">A name for the derived entity, which interfaces with customers.</span></span>|
|<span data-ttu-id="5eb6a-115">id</span><span class="sxs-lookup"><span data-stu-id="5eb6a-115">id</span></span>|<span data-ttu-id="5eb6a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="5eb6a-116">String</span></span>| <span data-ttu-id="5eb6a-117">Идентификатор производные сущности.</span><span class="sxs-lookup"><span data-stu-id="5eb6a-117">The ID for the derived entity.</span></span> <span data-ttu-id="5eb6a-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5eb6a-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5eb6a-119">Связи</span><span class="sxs-lookup"><span data-stu-id="5eb6a-119">Relationships</span></span>
<span data-ttu-id="5eb6a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5eb6a-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5eb6a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5eb6a-121">JSON representation</span></span>

<span data-ttu-id="5eb6a-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5eb6a-122">The following is a JSON representation of the resource.</span></span>

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
