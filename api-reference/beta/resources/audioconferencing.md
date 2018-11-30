---
title: Тип ресурса audioConferencing
description: Представляет телефона данные для доступа к onlineMeeting.
ms.openlocfilehash: dd23c6ade282e081482a8c079491644c663b4054
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077136"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="5e2e6-103">Тип ресурса audioConferencing</span><span class="sxs-lookup"><span data-stu-id="5e2e6-103">audioConferencing resource type</span></span>

> <span data-ttu-id="5e2e6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e2e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e2e6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e2e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e2e6-106">Представляет телефона данные для доступа к [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="5e2e6-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5e2e6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e2e6-107">Properties</span></span>

| <span data-ttu-id="5e2e6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e2e6-108">Property</span></span>            | <span data-ttu-id="5e2e6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5e2e6-109">Type</span></span>    | <span data-ttu-id="5e2e6-110">Description</span><span class="sxs-lookup"><span data-stu-id="5e2e6-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="5e2e6-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="5e2e6-111">dialinUrl</span></span>           | <span data-ttu-id="5e2e6-112">String</span><span class="sxs-lookup"><span data-stu-id="5e2e6-112">String</span></span>  | <span data-ttu-id="5e2e6-113">URL-адрес, доступном веб-страницу, которая содержит данные для подключения.</span><span class="sxs-lookup"><span data-stu-id="5e2e6-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="5e2e6-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="5e2e6-114">leaderPasscode</span></span>      | <span data-ttu-id="5e2e6-115">String</span><span class="sxs-lookup"><span data-stu-id="5e2e6-115">String</span></span>  | <span data-ttu-id="5e2e6-116">Ведущий сотрудник, пароль для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="5e2e6-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="5e2e6-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="5e2e6-117">participantPasscode</span></span> | <span data-ttu-id="5e2e6-118">String</span><span class="sxs-lookup"><span data-stu-id="5e2e6-118">String</span></span>  | <span data-ttu-id="5e2e6-119">Участников пароль, необходимый для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="5e2e6-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="5e2e6-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="5e2e6-120">tollFreeNumber</span></span>      | <span data-ttu-id="5e2e6-121">String</span><span class="sxs-lookup"><span data-stu-id="5e2e6-121">String</span></span>  | <span data-ttu-id="5e2e6-122">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="5e2e6-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="5e2e6-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="5e2e6-123">tollNumber</span></span>          | <span data-ttu-id="5e2e6-124">String</span><span class="sxs-lookup"><span data-stu-id="5e2e6-124">String</span></span>  | <span data-ttu-id="5e2e6-125">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="5e2e6-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="5e2e6-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e2e6-126">JSON representation</span></span>

<span data-ttu-id="5e2e6-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e2e6-127">The following is a JSON representation of the resource.</span></span>

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
