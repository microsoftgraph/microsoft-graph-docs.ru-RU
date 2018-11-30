---
title: Тип ресурса meetingCapability
description: Содержит возможности собрания
ms.openlocfilehash: 438193d08ab5542f07d4cbf61704520d81433e50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078084"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="4c108-103">Тип ресурса meetingCapability</span><span class="sxs-lookup"><span data-stu-id="4c108-103">meetingCapability resource type</span></span>

> <span data-ttu-id="4c108-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c108-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c108-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c108-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c108-106">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="4c108-106">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="4c108-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c108-107">Properties</span></span>

| <span data-ttu-id="4c108-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c108-108">Property</span></span>       | <span data-ttu-id="4c108-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4c108-109">Type</span></span>    | <span data-ttu-id="4c108-110">Description</span><span class="sxs-lookup"><span data-stu-id="4c108-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c108-111">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="4c108-111">allowAnonymousUsersToDialOut</span></span> | <span data-ttu-id="4c108-112">Логический</span><span class="sxs-lookup"><span data-stu-id="4c108-112">Boolean</span></span> | <span data-ttu-id="4c108-113">Указывает, может ли анонимные пользователи исходящие звонки на собрании.</span><span class="sxs-lookup"><span data-stu-id="4c108-113">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="4c108-114">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="4c108-114">autoAdmittedUsers</span></span> | <span data-ttu-id="4c108-115">String</span><span class="sxs-lookup"><span data-stu-id="4c108-115">String</span></span> | <span data-ttu-id="4c108-116">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="4c108-116">Possible values are: `everyoneInCompany`, `everyone`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c108-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c108-117">JSON representation</span></span>

<span data-ttu-id="4c108-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c108-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
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
