---
title: Тип ресурса attendee
description: Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 435a9b3badf20ddb79affd4e40e5ca8b66ff34c8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974294"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="0c8cd-104">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="0c8cd-104">attendee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c8cd-105">Участник события.</span><span class="sxs-lookup"><span data-stu-id="0c8cd-105">An event attendee.</span></span> <span data-ttu-id="0c8cd-106">Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.</span><span class="sxs-lookup"><span data-stu-id="0c8cd-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="0c8cd-107">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="0c8cd-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0c8cd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c8cd-108">Properties</span></span>
| <span data-ttu-id="0c8cd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c8cd-109">Property</span></span>     | <span data-ttu-id="0c8cd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0c8cd-110">Type</span></span>   |<span data-ttu-id="0c8cd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c8cd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c8cd-112">status</span><span class="sxs-lookup"><span data-stu-id="0c8cd-112">status</span></span>|[<span data-ttu-id="0c8cd-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="0c8cd-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="0c8cd-114">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="0c8cd-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="0c8cd-115">type</span><span class="sxs-lookup"><span data-stu-id="0c8cd-115">type</span></span>|<span data-ttu-id="0c8cd-116">String</span><span class="sxs-lookup"><span data-stu-id="0c8cd-116">String</span></span>|<span data-ttu-id="0c8cd-117">Тип участника: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="0c8cd-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="0c8cd-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0c8cd-118">emailAddress</span></span>|[<span data-ttu-id="0c8cd-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0c8cd-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="0c8cd-120">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="0c8cd-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c8cd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c8cd-121">JSON representation</span></span>

<span data-ttu-id="0c8cd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c8cd-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
