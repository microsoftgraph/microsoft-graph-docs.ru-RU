---
title: Тип ресурса meetingCapability
description: Содержит возможности собрания
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 342d264c1f4c670d159c15558c78cc896d4a9487
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931365"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="a7fe0-103">Тип ресурса meetingCapability</span><span class="sxs-lookup"><span data-stu-id="a7fe0-103">meetingCapability resource type</span></span>

> <span data-ttu-id="a7fe0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a7fe0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7fe0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7fe0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7fe0-106">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="a7fe0-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="a7fe0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7fe0-107">Properties</span></span>

| <span data-ttu-id="a7fe0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7fe0-108">Property</span></span>                          | <span data-ttu-id="a7fe0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a7fe0-109">Type</span></span>    | <span data-ttu-id="a7fe0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a7fe0-110">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="a7fe0-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="a7fe0-111">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="a7fe0-112">Логический</span><span class="sxs-lookup"><span data-stu-id="a7fe0-112">Boolean</span></span> | <span data-ttu-id="a7fe0-113">Указывает, может ли анонимные пользователи исходящие звонки на собрании.</span><span class="sxs-lookup"><span data-stu-id="a7fe0-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="a7fe0-114">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="a7fe0-114">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="a7fe0-115">Логический</span><span class="sxs-lookup"><span data-stu-id="a7fe0-115">Boolean</span></span> | <span data-ttu-id="a7fe0-116">Указывает, разрешены ли анонимные пользователи начало собрания.</span><span class="sxs-lookup"><span data-stu-id="a7fe0-116">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="a7fe0-117">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="a7fe0-117">autoAdmittedUsers</span></span>                 | <span data-ttu-id="a7fe0-118">String</span><span class="sxs-lookup"><span data-stu-id="a7fe0-118">String</span></span>  | <span data-ttu-id="a7fe0-119">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="a7fe0-119">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="a7fe0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7fe0-120">JSON representation</span></span>

<span data-ttu-id="a7fe0-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7fe0-121">The following is a JSON representation of the resource.</span></span>

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
