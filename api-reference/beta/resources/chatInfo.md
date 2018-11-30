---
title: Тип ресурса chatInfo
description: Сведения о сообщении в группах Майкрософт.
ms.openlocfilehash: d7e90cf2cdf5180f6483675d919b4e635a1cd5fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074812"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="74a76-103">Тип ресурса chatInfo</span><span class="sxs-lookup"><span data-stu-id="74a76-103">chatInfo resource type</span></span>

> <span data-ttu-id="74a76-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74a76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74a76-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74a76-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74a76-106">Сведения о сообщении в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="74a76-106">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="74a76-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="74a76-107">Properties</span></span>

| <span data-ttu-id="74a76-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="74a76-108">Property</span></span>            | <span data-ttu-id="74a76-109">Тип</span><span class="sxs-lookup"><span data-stu-id="74a76-109">Type</span></span>    | <span data-ttu-id="74a76-110">Description</span><span class="sxs-lookup"><span data-stu-id="74a76-110">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="74a76-111">Код сообщения</span><span class="sxs-lookup"><span data-stu-id="74a76-111">messageId</span></span>           | <span data-ttu-id="74a76-112">String</span><span class="sxs-lookup"><span data-stu-id="74a76-112">String</span></span>  | <span data-ttu-id="74a76-113">Уникальный идентификатор для сообщения в канале группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="74a76-113">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="74a76-114">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="74a76-114">replyChainMessageId</span></span> | <span data-ttu-id="74a76-115">String</span><span class="sxs-lookup"><span data-stu-id="74a76-115">String</span></span>  | <span data-ttu-id="74a76-116">Идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="74a76-116">The ID of the reply message.</span></span> |
| <span data-ttu-id="74a76-117">threadId</span><span class="sxs-lookup"><span data-stu-id="74a76-117">threadId</span></span>            | <span data-ttu-id="74a76-118">String</span><span class="sxs-lookup"><span data-stu-id="74a76-118">String</span></span>  | <span data-ttu-id="74a76-119">Уникальный идентификатор потока в группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="74a76-119">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="74a76-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74a76-120">JSON representation</span></span>

<span data-ttu-id="74a76-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74a76-121">The following is a JSON representation of the resource.</span></span>

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
