---
title: Тип ресурса Чатинфо
description: Содержит сведения, связанные с собраниями Microsoft Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5801ad39c3e977740825f14da18568a488e77695
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870360"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="dbffc-103">Тип ресурса Чатинфо</span><span class="sxs-lookup"><span data-stu-id="dbffc-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbffc-104">Содержит сведения, связанные с собраниями Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dbffc-104">Contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="dbffc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbffc-105">Properties</span></span>

| <span data-ttu-id="dbffc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbffc-106">Property</span></span>            | <span data-ttu-id="dbffc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="dbffc-107">Type</span></span>    | <span data-ttu-id="dbffc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="dbffc-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="dbffc-109">messageId</span><span class="sxs-lookup"><span data-stu-id="dbffc-109">messageId</span></span>           | <span data-ttu-id="dbffc-110">String</span><span class="sxs-lookup"><span data-stu-id="dbffc-110">String</span></span>  | <span data-ttu-id="dbffc-111">Уникальный идентификатор сообщения в канале Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dbffc-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="dbffc-112">репличаинмессажеид</span><span class="sxs-lookup"><span data-stu-id="dbffc-112">replyChainMessageId</span></span> | <span data-ttu-id="dbffc-113">String</span><span class="sxs-lookup"><span data-stu-id="dbffc-113">String</span></span>  | <span data-ttu-id="dbffc-114">Идентификатор ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="dbffc-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="dbffc-115">Tидентификатор</span><span class="sxs-lookup"><span data-stu-id="dbffc-115">threadId</span></span>            | <span data-ttu-id="dbffc-116">String</span><span class="sxs-lookup"><span data-stu-id="dbffc-116">String</span></span>  | <span data-ttu-id="dbffc-117">Уникальный идентификатор потока в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="dbffc-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dbffc-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbffc-118">JSON representation</span></span>

<span data-ttu-id="dbffc-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dbffc-119">The following is a JSON representation of the resource.</span></span>

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
