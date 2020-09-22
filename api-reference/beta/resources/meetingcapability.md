---
title: Тип ресурса Митингкапабилити
description: Содержит возможности собрания
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 29da5c8d4796e393bfead08979aca8e58a95024d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971687"
---
# <a name="meetingcapability-resource-type"></a><span data-ttu-id="42697-103">Тип ресурса Митингкапабилити</span><span class="sxs-lookup"><span data-stu-id="42697-103">meetingCapability resource type</span></span>

<span data-ttu-id="42697-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42697-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42697-105">Содержит возможности собрания</span><span class="sxs-lookup"><span data-stu-id="42697-105">Contains the capabilities of a meeting</span></span>

## <a name="properties"></a><span data-ttu-id="42697-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="42697-106">Properties</span></span>

| <span data-ttu-id="42697-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="42697-107">Property</span></span>                          | <span data-ttu-id="42697-108">Тип</span><span class="sxs-lookup"><span data-stu-id="42697-108">Type</span></span>    | <span data-ttu-id="42697-109">Описание</span><span class="sxs-lookup"><span data-stu-id="42697-109">Description</span></span>                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| <span data-ttu-id="42697-110">аллованонимаусусерстодиалаут</span><span class="sxs-lookup"><span data-stu-id="42697-110">allowAnonymousUsersToDialOut</span></span>      | <span data-ttu-id="42697-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="42697-111">Boolean</span></span> | <span data-ttu-id="42697-112">Указывает, разрешено ли исходящие вызовы анонимных пользователей на собрании.</span><span class="sxs-lookup"><span data-stu-id="42697-112">Indicates whether anonymous users dialout is allowed in a meeting.</span></span> |
| <span data-ttu-id="42697-113">аллованонимаусусерстостартмитинг</span><span class="sxs-lookup"><span data-stu-id="42697-113">allowAnonymousUsersToStartMeeting</span></span> | <span data-ttu-id="42697-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="42697-114">Boolean</span></span> | <span data-ttu-id="42697-115">Указывает, разрешено ли анонимным пользователям начинать собрание.</span><span class="sxs-lookup"><span data-stu-id="42697-115">Indicates whether anonymous users are allowed to start a meeting.</span></span>  |
| <span data-ttu-id="42697-116">аутоадмиттедусерс</span><span class="sxs-lookup"><span data-stu-id="42697-116">autoAdmittedUsers</span></span>                 | <span data-ttu-id="42697-117">String</span><span class="sxs-lookup"><span data-stu-id="42697-117">String</span></span>  | <span data-ttu-id="42697-118">Возможные значения: `everyoneInCompany`, `everyone`.</span><span class="sxs-lookup"><span data-stu-id="42697-118">Possible values are: `everyoneInCompany`, `everyone`.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="42697-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42697-119">JSON representation</span></span>

<span data-ttu-id="42697-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42697-120">The following is a JSON representation of the resource.</span></span>

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


