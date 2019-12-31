---
title: Тип ресурса Чатинфо
description: Содержит сведения, связанные с собраниями Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cb3806cf28e5557d7b5e4bf0296083e3c595047c
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913151"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="acc18-103">Тип ресурса Чатинфо</span><span class="sxs-lookup"><span data-stu-id="acc18-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acc18-104">Содержит сведения, связанные с собраниями Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="acc18-104">Contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="acc18-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="acc18-105">Properties</span></span>

| <span data-ttu-id="acc18-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="acc18-106">Property</span></span>            | <span data-ttu-id="acc18-107">Тип</span><span class="sxs-lookup"><span data-stu-id="acc18-107">Type</span></span>    | <span data-ttu-id="acc18-108">Описание</span><span class="sxs-lookup"><span data-stu-id="acc18-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="acc18-109">messageId</span><span class="sxs-lookup"><span data-stu-id="acc18-109">messageId</span></span>           | <span data-ttu-id="acc18-110">String</span><span class="sxs-lookup"><span data-stu-id="acc18-110">String</span></span>  | <span data-ttu-id="acc18-111">Уникальный идентификатор сообщения в канале Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="acc18-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="acc18-112">репличаинмессажеид</span><span class="sxs-lookup"><span data-stu-id="acc18-112">replyChainMessageId</span></span> | <span data-ttu-id="acc18-113">String</span><span class="sxs-lookup"><span data-stu-id="acc18-113">String</span></span>  | <span data-ttu-id="acc18-114">Идентификатор ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="acc18-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="acc18-115">Tидентификатор</span><span class="sxs-lookup"><span data-stu-id="acc18-115">threadId</span></span>            | <span data-ttu-id="acc18-116">String</span><span class="sxs-lookup"><span data-stu-id="acc18-116">String</span></span>  | <span data-ttu-id="acc18-117">Уникальный идентификатор потока в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="acc18-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="acc18-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="acc18-118">JSON representation</span></span>

<span data-ttu-id="acc18-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acc18-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
