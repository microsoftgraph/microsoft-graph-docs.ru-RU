---
title: Тип ресурса attendee
description: Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1cadb1ca6d2ab1168c3c7f9ff2b182b57112bfb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532092"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="63b5c-104">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="63b5c-104">attendee resource type</span></span>

<span data-ttu-id="63b5c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63b5c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63b5c-106">Участник события.</span><span class="sxs-lookup"><span data-stu-id="63b5c-106">An event attendee.</span></span> <span data-ttu-id="63b5c-107">Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.</span><span class="sxs-lookup"><span data-stu-id="63b5c-107">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="63b5c-108">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="63b5c-108">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="63b5c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="63b5c-109">Properties</span></span>
| <span data-ttu-id="63b5c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="63b5c-110">Property</span></span>     | <span data-ttu-id="63b5c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="63b5c-111">Type</span></span>   |<span data-ttu-id="63b5c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="63b5c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63b5c-113">status</span><span class="sxs-lookup"><span data-stu-id="63b5c-113">status</span></span>|[<span data-ttu-id="63b5c-114">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="63b5c-114">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="63b5c-115">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="63b5c-115">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="63b5c-116">type</span><span class="sxs-lookup"><span data-stu-id="63b5c-116">type</span></span>|<span data-ttu-id="63b5c-117">String</span><span class="sxs-lookup"><span data-stu-id="63b5c-117">String</span></span>|<span data-ttu-id="63b5c-118">Тип участника: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="63b5c-118">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="63b5c-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="63b5c-119">emailAddress</span></span>|[<span data-ttu-id="63b5c-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="63b5c-120">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="63b5c-121">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="63b5c-121">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63b5c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63b5c-122">JSON representation</span></span>

<span data-ttu-id="63b5c-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63b5c-123">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
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
