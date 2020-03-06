---
title: Тип ресурсов attendeeAvailability
description: Доступность участника.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bbc4a765ae8b61154bbbd304b131038f52b131ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532076"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="edf0c-103">Тип ресурсов attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="edf0c-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="edf0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edf0c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="edf0c-105">Доступность участника.</span><span class="sxs-lookup"><span data-stu-id="edf0c-105">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="edf0c-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="edf0c-106">JSON representation</span></span>

<span data-ttu-id="edf0c-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="edf0c-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="edf0c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="edf0c-108">Properties</span></span>
| <span data-ttu-id="edf0c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="edf0c-109">Property</span></span>     | <span data-ttu-id="edf0c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="edf0c-110">Type</span></span>   |<span data-ttu-id="edf0c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="edf0c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edf0c-112">attendee</span><span class="sxs-lookup"><span data-stu-id="edf0c-112">attendee</span></span>|[<span data-ttu-id="edf0c-113">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="edf0c-113">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="edf0c-114">Адрес электронной почты и тип участника — является ли это пользователь или ресурс, а также является ли он обязательным, если это человек.</span><span class="sxs-lookup"><span data-stu-id="edf0c-114">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="edf0c-115">availability</span><span class="sxs-lookup"><span data-stu-id="edf0c-115">availability</span></span>|<span data-ttu-id="edf0c-116">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="edf0c-116">freeBusyStatus</span></span>| <span data-ttu-id="edf0c-117">Состояние занятости участника.</span><span class="sxs-lookup"><span data-stu-id="edf0c-117">The availability status of the attendee.</span></span> <span data-ttu-id="edf0c-118">Допустимые значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="edf0c-118">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
