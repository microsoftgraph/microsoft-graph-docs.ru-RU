---
title: Тип ресурса Чатинфо
description: Сведения о сообщении в Microsoft Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5a2c7b705078e49c7e3bd68056b698e05d3f83bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012977"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="d4d23-103">Тип ресурса Чатинфо</span><span class="sxs-lookup"><span data-stu-id="d4d23-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4d23-104">Сведения о сообщении в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d4d23-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="d4d23-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4d23-105">Properties</span></span>

| <span data-ttu-id="d4d23-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4d23-106">Property</span></span>            | <span data-ttu-id="d4d23-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d4d23-107">Type</span></span>    | <span data-ttu-id="d4d23-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d4d23-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="d4d23-109">messageId</span><span class="sxs-lookup"><span data-stu-id="d4d23-109">messageId</span></span>           | <span data-ttu-id="d4d23-110">String</span><span class="sxs-lookup"><span data-stu-id="d4d23-110">String</span></span>  | <span data-ttu-id="d4d23-111">Уникальный идентификатор сообщения в канале Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d4d23-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="d4d23-112">Репличаинмессажеид</span><span class="sxs-lookup"><span data-stu-id="d4d23-112">replyChainMessageId</span></span> | <span data-ttu-id="d4d23-113">String</span><span class="sxs-lookup"><span data-stu-id="d4d23-113">String</span></span>  | <span data-ttu-id="d4d23-114">Идентификатор ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="d4d23-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="d4d23-115">Tидентификатор</span><span class="sxs-lookup"><span data-stu-id="d4d23-115">threadId</span></span>            | <span data-ttu-id="d4d23-116">String</span><span class="sxs-lookup"><span data-stu-id="d4d23-116">String</span></span>  | <span data-ttu-id="d4d23-117">Уникальный идентификатор потока в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d4d23-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4d23-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4d23-118">JSON representation</span></span>

<span data-ttu-id="d4d23-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4d23-119">The following is a JSON representation of the resource.</span></span>

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
