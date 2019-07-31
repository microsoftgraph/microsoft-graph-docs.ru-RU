---
title: Тип ресурса Митингкапабилити
description: Содержит возможности собрания
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1de406cf0614a4cbb64749cef763a97a3723eb48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966868"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="2cf7b-103">Тип ресурса Митингкапабилити</span><span class="sxs-lookup"><span data-stu-id="2cf7b-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cf7b-104">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="2cf7b-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="2cf7b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2cf7b-105">Properties</span></span>

| <span data-ttu-id="2cf7b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cf7b-106">Property</span></span>                          | <span data-ttu-id="2cf7b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2cf7b-107">Type</span></span>    | <span data-ttu-id="2cf7b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2cf7b-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="2cf7b-109">Аллованонимаусусерстодиалаут</span><span class="sxs-lookup"><span data-stu-id="2cf7b-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="2cf7b-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cf7b-110">Boolean</span></span> | <span data-ttu-id="2cf7b-111">Указывает, разрешено ли исходящие вызовы анонимных пользователей на собрании.</span><span class="sxs-lookup"><span data-stu-id="2cf7b-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="2cf7b-112">Аллованонимаусусерстостартмитинг</span><span class="sxs-lookup"><span data-stu-id="2cf7b-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="2cf7b-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cf7b-113">Boolean</span></span> | <span data-ttu-id="2cf7b-114">Указывает, разрешено ли анонимным пользователям начинать собрание.</span><span class="sxs-lookup"><span data-stu-id="2cf7b-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="2cf7b-115">Аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="2cf7b-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="2cf7b-116">String</span><span class="sxs-lookup"><span data-stu-id="2cf7b-116">String</span></span>  | <span data-ttu-id="2cf7b-117">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="2cf7b-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="2cf7b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2cf7b-118">JSON representation</span></span>

<span data-ttu-id="2cf7b-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cf7b-119">The following is a JSON representation of the resource.</span></span>

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
