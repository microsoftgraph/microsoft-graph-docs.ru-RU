---
title: Тип ресурса Митингкапабилити
description: Содержит возможности собрания
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b891a9e6d0eb90a527c79528e9fd595c2f8ca5b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913627"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="a8fe1-103">Тип ресурса Митингкапабилити</span><span class="sxs-lookup"><span data-stu-id="a8fe1-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8fe1-104">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="a8fe1-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="a8fe1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8fe1-105">Properties</span></span>

| <span data-ttu-id="a8fe1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8fe1-106">Property</span></span>                          | <span data-ttu-id="a8fe1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a8fe1-107">Type</span></span>    | <span data-ttu-id="a8fe1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a8fe1-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="a8fe1-109">аллованонимаусусерстодиалаут</span><span class="sxs-lookup"><span data-stu-id="a8fe1-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="a8fe1-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8fe1-110">Boolean</span></span> | <span data-ttu-id="a8fe1-111">Указывает, разрешено ли исходящие вызовы анонимных пользователей на собрании.</span><span class="sxs-lookup"><span data-stu-id="a8fe1-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="a8fe1-112">аллованонимаусусерстостартмитинг</span><span class="sxs-lookup"><span data-stu-id="a8fe1-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="a8fe1-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8fe1-113">Boolean</span></span> | <span data-ttu-id="a8fe1-114">Указывает, разрешено ли анонимным пользователям начинать собрание.</span><span class="sxs-lookup"><span data-stu-id="a8fe1-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="a8fe1-115">аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="a8fe1-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="a8fe1-116">String</span><span class="sxs-lookup"><span data-stu-id="a8fe1-116">String</span></span>  | <span data-ttu-id="a8fe1-117">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="a8fe1-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="a8fe1-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8fe1-118">JSON representation</span></span>

<span data-ttu-id="a8fe1-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8fe1-119">The following is a JSON representation of the resource.</span></span>

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
