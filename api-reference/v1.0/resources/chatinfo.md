---
title: Тип ресурса Чатинфо
description: Сведения о сообщении в Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b69905a0e1d8937c582df3373a4e981f8d8405ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533081"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="884c3-103">Тип ресурса Чатинфо</span><span class="sxs-lookup"><span data-stu-id="884c3-103">chatInfo resource type</span></span>

<span data-ttu-id="884c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="884c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="884c3-105">Содержит сведения, связанные с собраниями Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="884c3-105">This contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="884c3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="884c3-106">Properties</span></span>

| <span data-ttu-id="884c3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="884c3-107">Property</span></span>            | <span data-ttu-id="884c3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="884c3-108">Type</span></span>    | <span data-ttu-id="884c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="884c3-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="884c3-110">messageId</span><span class="sxs-lookup"><span data-stu-id="884c3-110">messageId</span></span>           | <span data-ttu-id="884c3-111">Строка</span><span class="sxs-lookup"><span data-stu-id="884c3-111">String</span></span>  | <span data-ttu-id="884c3-112">Уникальный идентификатор сообщения в канале Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="884c3-112">The unique identifier of a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="884c3-113">репличаинмессажеид</span><span class="sxs-lookup"><span data-stu-id="884c3-113">replyChainMessageId</span></span> | <span data-ttu-id="884c3-114">Строка</span><span class="sxs-lookup"><span data-stu-id="884c3-114">String</span></span>  | <span data-ttu-id="884c3-115">Идентификатор ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="884c3-115">The ID of the reply message.</span></span> |
| <span data-ttu-id="884c3-116">Tидентификатор</span><span class="sxs-lookup"><span data-stu-id="884c3-116">threadId</span></span>            | <span data-ttu-id="884c3-117">Строка</span><span class="sxs-lookup"><span data-stu-id="884c3-117">String</span></span>  | <span data-ttu-id="884c3-118">Уникальный идентификатор потока в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="884c3-118">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="884c3-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="884c3-119">JSON representation</span></span>

<span data-ttu-id="884c3-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="884c3-120">The following is a JSON representation of the resource.</span></span>

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
