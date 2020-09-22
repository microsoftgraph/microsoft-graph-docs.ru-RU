---
title: Тип ресурса Чатинфо
description: Сведения о сообщении в Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ee55fc2f9321a5b16c3a24ec330f5966472f4f9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059175"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="0f75d-103">Тип ресурса Чатинфо</span><span class="sxs-lookup"><span data-stu-id="0f75d-103">chatInfo resource type</span></span>

<span data-ttu-id="0f75d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f75d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f75d-105">Содержит сведения, связанные с собраниями Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0f75d-105">This contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="0f75d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f75d-106">Properties</span></span>

| <span data-ttu-id="0f75d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f75d-107">Property</span></span>            | <span data-ttu-id="0f75d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0f75d-108">Type</span></span>    | <span data-ttu-id="0f75d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f75d-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="0f75d-110">messageId</span><span class="sxs-lookup"><span data-stu-id="0f75d-110">messageId</span></span>           | <span data-ttu-id="0f75d-111">String</span><span class="sxs-lookup"><span data-stu-id="0f75d-111">String</span></span>  | <span data-ttu-id="0f75d-112">Уникальный идентификатор сообщения в канале Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0f75d-112">The unique identifier of a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="0f75d-113">репличаинмессажеид</span><span class="sxs-lookup"><span data-stu-id="0f75d-113">replyChainMessageId</span></span> | <span data-ttu-id="0f75d-114">String</span><span class="sxs-lookup"><span data-stu-id="0f75d-114">String</span></span>  | <span data-ttu-id="0f75d-115">Идентификатор ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="0f75d-115">The ID of the reply message.</span></span> |
| <span data-ttu-id="0f75d-116">Tидентификатор</span><span class="sxs-lookup"><span data-stu-id="0f75d-116">threadId</span></span>            | <span data-ttu-id="0f75d-117">String</span><span class="sxs-lookup"><span data-stu-id="0f75d-117">String</span></span>  | <span data-ttu-id="0f75d-118">Уникальный идентификатор потока в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="0f75d-118">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0f75d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f75d-119">JSON representation</span></span>

<span data-ttu-id="0f75d-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f75d-120">The following is a JSON representation of the resource.</span></span>

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

