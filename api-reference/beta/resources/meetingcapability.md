---
title: Тип ресурса meetingCapability
description: Содержит возможности собрания
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 3a7f291c81522d33bffbcce6e97a407f09234db5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825811"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="c026c-103">Тип ресурса meetingCapability</span><span class="sxs-lookup"><span data-stu-id="c026c-103">meetingCapability resource type</span></span>

> <span data-ttu-id="c026c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c026c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c026c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c026c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c026c-106">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="c026c-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="c026c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c026c-107">Properties</span></span>

| <span data-ttu-id="c026c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c026c-108">Property</span></span>                          | <span data-ttu-id="c026c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c026c-109">Type</span></span>    | <span data-ttu-id="c026c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c026c-110">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="c026c-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="c026c-111">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="c026c-112">Логический</span><span class="sxs-lookup"><span data-stu-id="c026c-112">Boolean</span></span> | <span data-ttu-id="c026c-113">Указывает, может ли анонимные пользователи исходящие звонки на собрании.</span><span class="sxs-lookup"><span data-stu-id="c026c-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="c026c-114">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="c026c-114">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="c026c-115">Логический</span><span class="sxs-lookup"><span data-stu-id="c026c-115">Boolean</span></span> | <span data-ttu-id="c026c-116">Указывает, разрешены ли анонимные пользователи начало собрания.</span><span class="sxs-lookup"><span data-stu-id="c026c-116">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="c026c-117">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="c026c-117">autoAdmittedUsers</span></span>                 | <span data-ttu-id="c026c-118">String</span><span class="sxs-lookup"><span data-stu-id="c026c-118">String</span></span>  | <span data-ttu-id="c026c-119">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="c026c-119">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="c026c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c026c-120">JSON representation</span></span>

<span data-ttu-id="c026c-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c026c-121">The following is a JSON representation of the resource.</span></span>

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
