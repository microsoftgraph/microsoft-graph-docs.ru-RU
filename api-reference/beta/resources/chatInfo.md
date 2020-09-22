---
title: Тип ресурса Чатинфо
description: Содержит сведения, связанные с собраниями Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e17f949b46626096238745b23b5332ffa69acf3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064355"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="a448a-103">Тип ресурса Чатинфо</span><span class="sxs-lookup"><span data-stu-id="a448a-103">chatInfo resource type</span></span>

<span data-ttu-id="a448a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a448a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a448a-105">Содержит сведения, связанные с собраниями Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a448a-105">Contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="a448a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a448a-106">Properties</span></span>

| <span data-ttu-id="a448a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a448a-107">Property</span></span>            | <span data-ttu-id="a448a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a448a-108">Type</span></span>    | <span data-ttu-id="a448a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a448a-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="a448a-110">messageId</span><span class="sxs-lookup"><span data-stu-id="a448a-110">messageId</span></span>           | <span data-ttu-id="a448a-111">String</span><span class="sxs-lookup"><span data-stu-id="a448a-111">String</span></span>  | <span data-ttu-id="a448a-112">Уникальный идентификатор сообщения в канале Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a448a-112">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="a448a-113">репличаинмессажеид</span><span class="sxs-lookup"><span data-stu-id="a448a-113">replyChainMessageId</span></span> | <span data-ttu-id="a448a-114">String</span><span class="sxs-lookup"><span data-stu-id="a448a-114">String</span></span>  | <span data-ttu-id="a448a-115">Идентификатор ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="a448a-115">The ID of the reply message.</span></span> |
| <span data-ttu-id="a448a-116">Tидентификатор</span><span class="sxs-lookup"><span data-stu-id="a448a-116">threadId</span></span>            | <span data-ttu-id="a448a-117">String</span><span class="sxs-lookup"><span data-stu-id="a448a-117">String</span></span>  | <span data-ttu-id="a448a-118">Уникальный идентификатор потока в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a448a-118">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a448a-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a448a-119">JSON representation</span></span>

<span data-ttu-id="a448a-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a448a-120">The following is a JSON representation of the resource.</span></span>

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


