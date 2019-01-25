---
title: Тип ресурса audioConferencing
description: Представляет телефона данные для доступа к onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb822f2049d84f9a2460370f05d5dfc85c347f15
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522177"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="dcb53-103">Тип ресурса audioConferencing</span><span class="sxs-lookup"><span data-stu-id="dcb53-103">audioConferencing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcb53-104">Представляет телефона данные для доступа к [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="dcb53-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dcb53-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dcb53-105">Properties</span></span>

| <span data-ttu-id="dcb53-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dcb53-106">Property</span></span>            | <span data-ttu-id="dcb53-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dcb53-107">Type</span></span>    | <span data-ttu-id="dcb53-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dcb53-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="dcb53-109">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="dcb53-109">dialinUrl</span></span>           | <span data-ttu-id="dcb53-110">String</span><span class="sxs-lookup"><span data-stu-id="dcb53-110">String</span></span>  | <span data-ttu-id="dcb53-111">URL-адрес, доступном веб-страницу, которая содержит данные для подключения.</span><span class="sxs-lookup"><span data-stu-id="dcb53-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="dcb53-112">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="dcb53-112">leaderPasscode</span></span>      | <span data-ttu-id="dcb53-113">String</span><span class="sxs-lookup"><span data-stu-id="dcb53-113">String</span></span>  | <span data-ttu-id="dcb53-114">Ведущий сотрудник, пароль для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="dcb53-114">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="dcb53-115">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="dcb53-115">participantPasscode</span></span> | <span data-ttu-id="dcb53-116">String</span><span class="sxs-lookup"><span data-stu-id="dcb53-116">String</span></span>  | <span data-ttu-id="dcb53-117">Участников пароль, необходимый для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="dcb53-117">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="dcb53-118">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="dcb53-118">tollFreeNumber</span></span>      | <span data-ttu-id="dcb53-119">String</span><span class="sxs-lookup"><span data-stu-id="dcb53-119">String</span></span>  | <span data-ttu-id="dcb53-120">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="dcb53-120">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="dcb53-121">tollNumber</span><span class="sxs-lookup"><span data-stu-id="dcb53-121">tollNumber</span></span>          | <span data-ttu-id="dcb53-122">String</span><span class="sxs-lookup"><span data-stu-id="dcb53-122">String</span></span>  | <span data-ttu-id="dcb53-123">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="dcb53-123">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="dcb53-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dcb53-124">JSON representation</span></span>

<span data-ttu-id="dcb53-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dcb53-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioconferencing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
