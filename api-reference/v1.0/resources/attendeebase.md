---
title: Тип ресурсов attendeeBase
description: Тип участника.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 154584a91fc8844e2745d5198773157c4dfe26d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033112"
---
# <a name="attendeebase-resource-type"></a><span data-ttu-id="0c154-103">Тип ресурсов attendeeBase</span><span class="sxs-lookup"><span data-stu-id="0c154-103">attendeeBase resource type</span></span>

<span data-ttu-id="0c154-104">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="0c154-104">The type of attendee.</span></span>

<span data-ttu-id="0c154-105">Тип, производный от [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="0c154-105">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c154-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c154-106">JSON representation</span></span>

<span data-ttu-id="0c154-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="0c154-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="0c154-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c154-108">Properties</span></span>
| <span data-ttu-id="0c154-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c154-109">Property</span></span>     | <span data-ttu-id="0c154-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0c154-110">Type</span></span>   |<span data-ttu-id="0c154-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c154-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c154-112">type</span><span class="sxs-lookup"><span data-stu-id="0c154-112">type</span></span>|<span data-ttu-id="0c154-113">attendeeType</span><span class="sxs-lookup"><span data-stu-id="0c154-113">attendeeType</span></span>| <span data-ttu-id="0c154-114">Тип участника.</span><span class="sxs-lookup"><span data-stu-id="0c154-114">The type of attendee.</span></span> <span data-ttu-id="0c154-115">Допустимые значения: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="0c154-115">The possible values are: `required`, `optional`, `resource`.</span></span> <span data-ttu-id="0c154-116">Если участник является пользователем, то [findMeetingTimes](../api/user-findmeetingtimes.md) всегда определяет тип этого пользователя как `Required`.</span><span class="sxs-lookup"><span data-stu-id="0c154-116">Currently if the attendee is a person, [findMeetingTimes](../api/user-findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="0c154-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0c154-117">emailAddress</span></span>|[<span data-ttu-id="0c154-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0c154-118">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="0c154-119">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="0c154-119">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
