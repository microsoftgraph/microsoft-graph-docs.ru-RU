---
title: Тип ресурса audioConferencing
description: Представляет телефона данные для доступа к onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd65b094a17ad3fa470471c3ed6dd3908367e578
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977509"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="e4ef7-103">Тип ресурса audioConferencing</span><span class="sxs-lookup"><span data-stu-id="e4ef7-103">audioConferencing resource type</span></span>

> <span data-ttu-id="e4ef7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e4ef7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4ef7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ef7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e4ef7-106">Представляет телефона данные для доступа к [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="e4ef7-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e4ef7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4ef7-107">Properties</span></span>

| <span data-ttu-id="e4ef7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4ef7-108">Property</span></span>            | <span data-ttu-id="e4ef7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e4ef7-109">Type</span></span>    | <span data-ttu-id="e4ef7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e4ef7-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="e4ef7-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="e4ef7-111">dialinUrl</span></span>           | <span data-ttu-id="e4ef7-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e4ef7-112">String</span></span>  | <span data-ttu-id="e4ef7-113">URL-адрес, доступном веб-страницу, которая содержит данные для подключения.</span><span class="sxs-lookup"><span data-stu-id="e4ef7-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="e4ef7-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="e4ef7-114">leaderPasscode</span></span>      | <span data-ttu-id="e4ef7-115">Строка</span><span class="sxs-lookup"><span data-stu-id="e4ef7-115">String</span></span>  | <span data-ttu-id="e4ef7-116">Ведущий сотрудник, пароль для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="e4ef7-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="e4ef7-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="e4ef7-117">participantPasscode</span></span> | <span data-ttu-id="e4ef7-118">Строка</span><span class="sxs-lookup"><span data-stu-id="e4ef7-118">String</span></span>  | <span data-ttu-id="e4ef7-119">Участников пароль, необходимый для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="e4ef7-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="e4ef7-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="e4ef7-120">tollFreeNumber</span></span>      | <span data-ttu-id="e4ef7-121">Строка</span><span class="sxs-lookup"><span data-stu-id="e4ef7-121">String</span></span>  | <span data-ttu-id="e4ef7-122">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="e4ef7-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="e4ef7-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="e4ef7-123">tollNumber</span></span>          | <span data-ttu-id="e4ef7-124">Строка</span><span class="sxs-lookup"><span data-stu-id="e4ef7-124">String</span></span>  | <span data-ttu-id="e4ef7-125">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="e4ef7-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="e4ef7-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4ef7-126">JSON representation</span></span>

<span data-ttu-id="e4ef7-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4ef7-127">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
