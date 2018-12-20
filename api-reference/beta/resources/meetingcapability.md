---
title: Тип ресурса meetingCapability
description: Содержит возможности собрания
author: VinodRavichandran
ms.openlocfilehash: 1a6f172922c0efbc9ad93e32141e364e2d0fc711
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380249"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="00f18-103">Тип ресурса meetingCapability</span><span class="sxs-lookup"><span data-stu-id="00f18-103">meetingCapability resource type</span></span>

> <span data-ttu-id="00f18-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00f18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00f18-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f18-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00f18-106">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="00f18-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="00f18-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="00f18-107">Properties</span></span>

| <span data-ttu-id="00f18-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="00f18-108">Property</span></span>                          | <span data-ttu-id="00f18-109">Тип</span><span class="sxs-lookup"><span data-stu-id="00f18-109">Type</span></span>    | <span data-ttu-id="00f18-110">Описание</span><span class="sxs-lookup"><span data-stu-id="00f18-110">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="00f18-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="00f18-111">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="00f18-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="00f18-112">Boolean</span></span> | <span data-ttu-id="00f18-113">Указывает, может ли анонимные пользователи исходящие звонки на собрании.</span><span class="sxs-lookup"><span data-stu-id="00f18-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="00f18-114">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="00f18-114">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="00f18-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="00f18-115">Boolean</span></span> | <span data-ttu-id="00f18-116">Указывает, разрешены ли анонимные пользователи начало собрания.</span><span class="sxs-lookup"><span data-stu-id="00f18-116">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="00f18-117">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="00f18-117">autoAdmittedUsers</span></span>                 | <span data-ttu-id="00f18-118">String</span><span class="sxs-lookup"><span data-stu-id="00f18-118">String</span></span>  | <span data-ttu-id="00f18-119">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="00f18-119">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="00f18-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00f18-120">JSON representation</span></span>

<span data-ttu-id="00f18-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00f18-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
