---
title: Тип ресурса audioConferencing
description: Представляет телефона данные для доступа к onlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9bd8343f29a797a24044f02aa2a00bd098c35007
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843626"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="c97a4-103">Тип ресурса audioConferencing</span><span class="sxs-lookup"><span data-stu-id="c97a4-103">audioConferencing resource type</span></span>

> <span data-ttu-id="c97a4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c97a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c97a4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c97a4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c97a4-106">Представляет телефона данные для доступа к [onlineMeeting](onlinemeeting.md).</span><span class="sxs-lookup"><span data-stu-id="c97a4-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c97a4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c97a4-107">Properties</span></span>

| <span data-ttu-id="c97a4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c97a4-108">Property</span></span>            | <span data-ttu-id="c97a4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c97a4-109">Type</span></span>    | <span data-ttu-id="c97a4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c97a4-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="c97a4-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="c97a4-111">dialinUrl</span></span>           | <span data-ttu-id="c97a4-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c97a4-112">String</span></span>  | <span data-ttu-id="c97a4-113">URL-адрес, доступном веб-страницу, которая содержит данные для подключения.</span><span class="sxs-lookup"><span data-stu-id="c97a4-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="c97a4-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="c97a4-114">leaderPasscode</span></span>      | <span data-ttu-id="c97a4-115">Строка</span><span class="sxs-lookup"><span data-stu-id="c97a4-115">String</span></span>  | <span data-ttu-id="c97a4-116">Ведущий сотрудник, пароль для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="c97a4-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="c97a4-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="c97a4-117">participantPasscode</span></span> | <span data-ttu-id="c97a4-118">Строка</span><span class="sxs-lookup"><span data-stu-id="c97a4-118">String</span></span>  | <span data-ttu-id="c97a4-119">Участников пароль, необходимый для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="c97a4-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="c97a4-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="c97a4-120">tollFreeNumber</span></span>      | <span data-ttu-id="c97a4-121">Строка</span><span class="sxs-lookup"><span data-stu-id="c97a4-121">String</span></span>  | <span data-ttu-id="c97a4-122">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="c97a4-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="c97a4-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="c97a4-123">tollNumber</span></span>          | <span data-ttu-id="c97a4-124">Строка</span><span class="sxs-lookup"><span data-stu-id="c97a4-124">String</span></span>  | <span data-ttu-id="c97a4-125">Бесплатный номер для подключения к поставщику конференции звук.</span><span class="sxs-lookup"><span data-stu-id="c97a4-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="c97a4-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c97a4-126">JSON representation</span></span>

<span data-ttu-id="c97a4-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c97a4-127">The following is a JSON representation of the resource.</span></span>

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
