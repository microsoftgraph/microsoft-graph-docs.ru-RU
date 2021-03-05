---
title: Тип ресурсов attendeeAvailability
description: Доступность участника.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9c69925ee64dd3c39b7edb59a6416d0ddc5b533c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474465"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="eec65-103">Тип ресурсов attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="eec65-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="eec65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eec65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eec65-105">Доступность участника.</span><span class="sxs-lookup"><span data-stu-id="eec65-105">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eec65-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eec65-106">JSON representation</span></span>

<span data-ttu-id="eec65-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="eec65-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="eec65-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eec65-108">Properties</span></span>
| <span data-ttu-id="eec65-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eec65-109">Property</span></span>     | <span data-ttu-id="eec65-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eec65-110">Type</span></span>   |<span data-ttu-id="eec65-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eec65-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eec65-112">attendee</span><span class="sxs-lookup"><span data-stu-id="eec65-112">attendee</span></span>|[<span data-ttu-id="eec65-113">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="eec65-113">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="eec65-114">Адрес электронной почты и тип участника — будь то человек или ресурс, а также необходимые или необязательные, если это человек.</span><span class="sxs-lookup"><span data-stu-id="eec65-114">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="eec65-115">availability</span><span class="sxs-lookup"><span data-stu-id="eec65-115">availability</span></span>|<span data-ttu-id="eec65-116">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="eec65-116">freeBusyStatus</span></span>| <span data-ttu-id="eec65-117">Состояние занятости участника.</span><span class="sxs-lookup"><span data-stu-id="eec65-117">The availability status of the attendee.</span></span> <span data-ttu-id="eec65-118">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="eec65-118">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

