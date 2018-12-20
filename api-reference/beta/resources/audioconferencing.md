---
title: Тип ресурса audioConferencing
description: Представляет телефона данные для доступа к onlineMeeting.
author: VinodRavichandran
ms.openlocfilehash: 4e2ee26e6f9a86d50efcb21cd95b84b207488ef1
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380228"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="93484-103">Тип ресурса audioConferencing</span><span class="sxs-lookup"><span data-stu-id="93484-103">audioConferencing resource type</span></span>

> <span data-ttu-id="93484-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="93484-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93484-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93484-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93484-106">Представляет телефона данные для доступа к [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="93484-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="93484-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="93484-107">Properties</span></span>

| <span data-ttu-id="93484-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="93484-108">Property</span></span>            | <span data-ttu-id="93484-109">Тип</span><span class="sxs-lookup"><span data-stu-id="93484-109">Type</span></span>    | <span data-ttu-id="93484-110">Описание</span><span class="sxs-lookup"><span data-stu-id="93484-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="93484-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="93484-111">dialinUrl</span></span>           | <span data-ttu-id="93484-112">String</span><span class="sxs-lookup"><span data-stu-id="93484-112">String</span></span>  | <span data-ttu-id="93484-113">URL-адрес, доступном веб-страницу, которая содержит данные для подключения.</span><span class="sxs-lookup"><span data-stu-id="93484-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="93484-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="93484-114">leaderPasscode</span></span>      | <span data-ttu-id="93484-115">String</span><span class="sxs-lookup"><span data-stu-id="93484-115">String</span></span>  | <span data-ttu-id="93484-116">Ведущий сотрудник, пароль для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="93484-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="93484-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="93484-117">participantPasscode</span></span> | <span data-ttu-id="93484-118">String</span><span class="sxs-lookup"><span data-stu-id="93484-118">String</span></span>  | <span data-ttu-id="93484-119">Участников пароль, необходимый для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="93484-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="93484-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="93484-120">tollFreeNumber</span></span>      | <span data-ttu-id="93484-121">String</span><span class="sxs-lookup"><span data-stu-id="93484-121">String</span></span>  | <span data-ttu-id="93484-122">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="93484-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="93484-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="93484-123">tollNumber</span></span>          | <span data-ttu-id="93484-124">String</span><span class="sxs-lookup"><span data-stu-id="93484-124">String</span></span>  | <span data-ttu-id="93484-125">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="93484-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="93484-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93484-126">JSON representation</span></span>

<span data-ttu-id="93484-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93484-127">The following is a JSON representation of the resource.</span></span>

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
