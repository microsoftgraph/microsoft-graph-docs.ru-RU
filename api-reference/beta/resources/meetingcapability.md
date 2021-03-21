---
title: Тип ресурса meetingCapability
description: Содержит возможности собрания
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d8e1d3985f95ecc28bd986218d7ff668f65b1db8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960407"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="a1add-103">Тип ресурса meetingCapability</span><span class="sxs-lookup"><span data-stu-id="a1add-103">meetingCapability resource type</span></span>

<span data-ttu-id="a1add-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1add-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1add-105">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="a1add-105">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="a1add-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1add-106">Properties</span></span>

| <span data-ttu-id="a1add-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1add-107">Property</span></span>                          | <span data-ttu-id="a1add-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a1add-108">Type</span></span>    | <span data-ttu-id="a1add-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a1add-109">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="a1add-110">allowAnonymousUsersToDialOut</span><span class="sxs-lookup"><span data-stu-id="a1add-110">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="a1add-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1add-111">Boolean</span></span> | <span data-ttu-id="a1add-112">Указывает, разрешен ли анонимный диалог пользователей на собрании.</span><span class="sxs-lookup"><span data-stu-id="a1add-112">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="a1add-113">allowAnonymousUsersToStartMeeting</span><span class="sxs-lookup"><span data-stu-id="a1add-113">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="a1add-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1add-114">Boolean</span></span> | <span data-ttu-id="a1add-115">Указывает, разрешено ли анонимным пользователям начинать собрание.</span><span class="sxs-lookup"><span data-stu-id="a1add-115">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="a1add-116">autoAdmittedUsers</span><span class="sxs-lookup"><span data-stu-id="a1add-116">autoAdmittedUsers</span></span>                 | <span data-ttu-id="a1add-117">autoAdmittedUsersType</span><span class="sxs-lookup"><span data-stu-id="a1add-117">autoAdmittedUsersType</span></span>  | <span data-ttu-id="a1add-118">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="a1add-118">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="a1add-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1add-119">JSON representation</span></span>

<span data-ttu-id="a1add-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1add-120">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


