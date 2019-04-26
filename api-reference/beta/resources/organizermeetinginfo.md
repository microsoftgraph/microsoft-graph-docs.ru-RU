---
title: Тип ресурса Организермитингинфо
description: Сведения о собрании, содержащие организатора собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3b7d21a313d8744f18c8b96549bc9470b587361c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568600"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="f6c81-103">Тип ресурса Организермитингинфо</span><span class="sxs-lookup"><span data-stu-id="f6c81-103">organizerMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6c81-104">Сведения о собрании, содержащие организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="f6c81-104">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="f6c81-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6c81-105">Properties</span></span>

| <span data-ttu-id="f6c81-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6c81-106">Property</span></span>                     | <span data-ttu-id="f6c81-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f6c81-107">Type</span></span>                          | <span data-ttu-id="f6c81-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f6c81-108">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="f6c81-109">Алловконверсатионвисаусост</span><span class="sxs-lookup"><span data-stu-id="f6c81-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="f6c81-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6c81-110">Boolean</span></span>                       | <span data-ttu-id="f6c81-111">Указывает, может ли беседа продолжиться после закрытия узла беседы.</span><span class="sxs-lookup"><span data-stu-id="f6c81-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="f6c81-112">organizer</span><span class="sxs-lookup"><span data-stu-id="f6c81-112">organizer</span></span>                    | [<span data-ttu-id="f6c81-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="f6c81-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="f6c81-114">Удостоверение Azure Active Directory для организатора.</span><span class="sxs-lookup"><span data-stu-id="f6c81-114">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f6c81-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6c81-115">JSON representation</span></span>

<span data-ttu-id="f6c81-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6c81-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.meetingInfo",
   "openType": true,
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "microsoft.graph.identitySet" }
}
```

## <a name="example"></a><span data-ttu-id="f6c81-117">Пример</span><span class="sxs-lookup"><span data-stu-id="f6c81-117">Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
