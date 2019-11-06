---
title: Тип ресурса Митингкапабилити
description: Содержит возможности собрания
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab0173f5519960f58c85d4bdd769e5ffb2a952c6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006650"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="6710a-103">Тип ресурса Митингкапабилити</span><span class="sxs-lookup"><span data-stu-id="6710a-103">meetingCapability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6710a-104">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="6710a-104">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="6710a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6710a-105">Properties</span></span>

| <span data-ttu-id="6710a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6710a-106">Property</span></span>                          | <span data-ttu-id="6710a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6710a-107">Type</span></span>    | <span data-ttu-id="6710a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6710a-108">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="6710a-109">аллованонимаусусерстодиалаут</span><span class="sxs-lookup"><span data-stu-id="6710a-109">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="6710a-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="6710a-110">Boolean</span></span> | <span data-ttu-id="6710a-111">Указывает, разрешено ли исходящие вызовы анонимных пользователей на собрании.</span><span class="sxs-lookup"><span data-stu-id="6710a-111">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="6710a-112">аллованонимаусусерстостартмитинг</span><span class="sxs-lookup"><span data-stu-id="6710a-112">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="6710a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6710a-113">Boolean</span></span> | <span data-ttu-id="6710a-114">Указывает, разрешено ли анонимным пользователям начинать собрание.</span><span class="sxs-lookup"><span data-stu-id="6710a-114">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="6710a-115">аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="6710a-115">autoAdmittedUsers</span></span>                 | <span data-ttu-id="6710a-116">String</span><span class="sxs-lookup"><span data-stu-id="6710a-116">String</span></span>  | <span data-ttu-id="6710a-117">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="6710a-117">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="6710a-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6710a-118">JSON representation</span></span>

<span data-ttu-id="6710a-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6710a-119">The following is a JSON representation of the resource.</span></span>

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
