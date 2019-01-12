---
title: Тип ресурса organizerMeetingInfo
description: Сведения о собрании, содержащий организатора собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 66a08b30741d488edf2d514568a17f292e588c23
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957706"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="210b1-103">Тип ресурса organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="210b1-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="210b1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="210b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="210b1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="210b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="210b1-106">Сведения о собрании, содержащий организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="210b1-106">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="210b1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="210b1-107">Properties</span></span>

| <span data-ttu-id="210b1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="210b1-108">Property</span></span>                     | <span data-ttu-id="210b1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="210b1-109">Type</span></span>                          | <span data-ttu-id="210b1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="210b1-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="210b1-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="210b1-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="210b1-112">Логический</span><span class="sxs-lookup"><span data-stu-id="210b1-112">Boolean</span></span>                       | <span data-ttu-id="210b1-113">Указывает, если беседы можно продолжить после покидает узла беседы.</span><span class="sxs-lookup"><span data-stu-id="210b1-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="210b1-114">organizer</span><span class="sxs-lookup"><span data-stu-id="210b1-114">organizer</span></span>                    | [<span data-ttu-id="210b1-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="210b1-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="210b1-116">Организатор identity Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="210b1-116">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="210b1-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="210b1-117">JSON representation</span></span>

<span data-ttu-id="210b1-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="210b1-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

## <a name="example"></a><span data-ttu-id="210b1-119">Пример</span><span class="sxs-lookup"><span data-stu-id="210b1-119">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": {
    "user": {
      "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
      "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
