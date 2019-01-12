---
title: Тип ресурса chatInfo
description: Сведения о сообщении в группах Майкрософт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 840073d6882d6665be60e7386eaafe3168b70dbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940752"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="0ff82-103">Тип ресурса chatInfo</span><span class="sxs-lookup"><span data-stu-id="0ff82-103">chatInfo resource type</span></span>

> <span data-ttu-id="0ff82-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ff82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ff82-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ff82-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ff82-106">Сведения о сообщении в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0ff82-106">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="0ff82-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ff82-107">Properties</span></span>

| <span data-ttu-id="0ff82-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ff82-108">Property</span></span>            | <span data-ttu-id="0ff82-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0ff82-109">Type</span></span>    | <span data-ttu-id="0ff82-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0ff82-110">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="0ff82-111">Код сообщения</span><span class="sxs-lookup"><span data-stu-id="0ff82-111">messageId</span></span>           | <span data-ttu-id="0ff82-112">Строка</span><span class="sxs-lookup"><span data-stu-id="0ff82-112">String</span></span>  | <span data-ttu-id="0ff82-113">Уникальный идентификатор для сообщения в канале группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0ff82-113">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="0ff82-114">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="0ff82-114">replyChainMessageId</span></span> | <span data-ttu-id="0ff82-115">Строка</span><span class="sxs-lookup"><span data-stu-id="0ff82-115">String</span></span>  | <span data-ttu-id="0ff82-116">Идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="0ff82-116">The ID of the reply message.</span></span> |
| <span data-ttu-id="0ff82-117">threadId</span><span class="sxs-lookup"><span data-stu-id="0ff82-117">threadId</span></span>            | <span data-ttu-id="0ff82-118">Строка</span><span class="sxs-lookup"><span data-stu-id="0ff82-118">String</span></span>  | <span data-ttu-id="0ff82-119">Уникальный идентификатор потока в группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="0ff82-119">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ff82-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ff82-120">JSON representation</span></span>

<span data-ttu-id="0ff82-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ff82-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
