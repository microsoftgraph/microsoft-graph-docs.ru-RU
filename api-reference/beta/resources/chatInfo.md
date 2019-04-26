---
title: Тип ресурса Чатинфо
description: Сведения о сообщении в Microsoft Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 552844795d3ba7e8ad4c8a3c3a6dff3c18990bc2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339697"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="ea8cc-103">Тип ресурса Чатинфо</span><span class="sxs-lookup"><span data-stu-id="ea8cc-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea8cc-104">Сведения о сообщении в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="ea8cc-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea8cc-105">Properties</span></span>

| <span data-ttu-id="ea8cc-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea8cc-106">Property</span></span>            | <span data-ttu-id="ea8cc-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ea8cc-107">Type</span></span>    | <span data-ttu-id="ea8cc-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ea8cc-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="ea8cc-109">messageId</span><span class="sxs-lookup"><span data-stu-id="ea8cc-109">messageId</span></span>           | <span data-ttu-id="ea8cc-110">String</span><span class="sxs-lookup"><span data-stu-id="ea8cc-110">String</span></span>  | <span data-ttu-id="ea8cc-111">Уникальный идентификатор сообщения в канале Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="ea8cc-112">Репличаинмессажеид</span><span class="sxs-lookup"><span data-stu-id="ea8cc-112">replyChainMessageId</span></span> | <span data-ttu-id="ea8cc-113">String</span><span class="sxs-lookup"><span data-stu-id="ea8cc-113">String</span></span>  | <span data-ttu-id="ea8cc-114">Идентификатор ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="ea8cc-115">Tидентификатор</span><span class="sxs-lookup"><span data-stu-id="ea8cc-115">threadId</span></span>            | <span data-ttu-id="ea8cc-116">String</span><span class="sxs-lookup"><span data-stu-id="ea8cc-116">String</span></span>  | <span data-ttu-id="ea8cc-117">Уникальный идентификатор потока в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ea8cc-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea8cc-118">JSON representation</span></span>

<span data-ttu-id="ea8cc-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea8cc-119">The following is a JSON representation of the resource.</span></span>

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
