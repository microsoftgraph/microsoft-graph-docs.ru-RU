---
title: Тип ресурса attendee
description: Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.
localization_priority: Normal
ms.openlocfilehash: 95881d0e2f3dfe51b975e60ba6f8d32cda5e222c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859327"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="25798-104">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="25798-104">attendee resource type</span></span>

> <span data-ttu-id="25798-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="25798-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25798-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25798-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25798-107">Участник события.</span><span class="sxs-lookup"><span data-stu-id="25798-107">An event attendee.</span></span> <span data-ttu-id="25798-108">Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.</span><span class="sxs-lookup"><span data-stu-id="25798-108">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="25798-109">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="25798-109">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="25798-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="25798-110">Properties</span></span>
| <span data-ttu-id="25798-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="25798-111">Property</span></span>     | <span data-ttu-id="25798-112">Тип</span><span class="sxs-lookup"><span data-stu-id="25798-112">Type</span></span>   |<span data-ttu-id="25798-113">Описание</span><span class="sxs-lookup"><span data-stu-id="25798-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25798-114">status</span><span class="sxs-lookup"><span data-stu-id="25798-114">status</span></span>|[<span data-ttu-id="25798-115">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="25798-115">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="25798-116">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="25798-116">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="25798-117">type</span><span class="sxs-lookup"><span data-stu-id="25798-117">type</span></span>|<span data-ttu-id="25798-118">String</span><span class="sxs-lookup"><span data-stu-id="25798-118">String</span></span>|<span data-ttu-id="25798-119">Тип участника: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="25798-119">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="25798-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="25798-120">emailAddress</span></span>|[<span data-ttu-id="25798-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="25798-121">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="25798-122">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="25798-122">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25798-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25798-123">JSON representation</span></span>

<span data-ttu-id="25798-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25798-124">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
