---
title: Тип ресурса organizerMeetingInfo
description: Сведения о собрании, содержащий организатора собрания.
author: VinodRavichandran
ms.openlocfilehash: 296b20125908caf73221c2a8380e91931deb7e61
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380214"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="2f7f3-103">Тип ресурса organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="2f7f3-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="2f7f3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f7f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f7f3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f7f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f7f3-106">Сведения о собрании, содержащий организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="2f7f3-106">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="2f7f3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f7f3-107">Properties</span></span>

| <span data-ttu-id="2f7f3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f7f3-108">Property</span></span>                     | <span data-ttu-id="2f7f3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2f7f3-109">Type</span></span>                          | <span data-ttu-id="2f7f3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2f7f3-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="2f7f3-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="2f7f3-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="2f7f3-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f7f3-112">Boolean</span></span>                       | <span data-ttu-id="2f7f3-113">Указывает, если беседы можно продолжить после покидает узла беседы.</span><span class="sxs-lookup"><span data-stu-id="2f7f3-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="2f7f3-114">organizer</span><span class="sxs-lookup"><span data-stu-id="2f7f3-114">organizer</span></span>                    | [<span data-ttu-id="2f7f3-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="2f7f3-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="2f7f3-116">Организатор identity Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2f7f3-116">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="2f7f3-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f7f3-117">JSON representation</span></span>

<span data-ttu-id="2f7f3-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f7f3-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="2f7f3-119">Пример</span><span class="sxs-lookup"><span data-stu-id="2f7f3-119">Example</span></span>

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
