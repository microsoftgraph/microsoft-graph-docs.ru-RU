---
title: Тип ресурса organizerMeetingInfo
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 00a7978c44c82ddd6b34802f29188a554e7e0b4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078680"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="5fe33-103">Тип ресурса organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="5fe33-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="5fe33-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5fe33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fe33-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fe33-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="5fe33-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fe33-106">Properties</span></span>

| <span data-ttu-id="5fe33-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fe33-107">Property</span></span>                     | <span data-ttu-id="5fe33-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5fe33-108">Type</span></span>                          | <span data-ttu-id="5fe33-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5fe33-109">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="5fe33-110">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="5fe33-110">allowConversationWithoutHost</span></span> | <span data-ttu-id="5fe33-111">Логический</span><span class="sxs-lookup"><span data-stu-id="5fe33-111">Boolean</span></span>                       | <span data-ttu-id="5fe33-112">Указывает, если беседы можно продолжить после покидает узла беседы.</span><span class="sxs-lookup"><span data-stu-id="5fe33-112">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="5fe33-113">organizer</span><span class="sxs-lookup"><span data-stu-id="5fe33-113">organizer</span></span>                    | [<span data-ttu-id="5fe33-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="5fe33-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="5fe33-115">Организатор identity Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5fe33-115">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5fe33-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fe33-116">JSON representation</span></span>

<span data-ttu-id="5fe33-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fe33-117">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="5fe33-118">Пример</span><span class="sxs-lookup"><span data-stu-id="5fe33-118">Example</span></span>

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
