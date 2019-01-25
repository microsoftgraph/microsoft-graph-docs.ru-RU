---
title: Тип ресурса chatInfo
description: Сведения о сообщении в группах Майкрософт.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3c1414d10a262280bcf0d3a307fc0c71aed2fbde
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507665"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="2785b-103">Тип ресурса chatInfo</span><span class="sxs-lookup"><span data-stu-id="2785b-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2785b-104">Сведения о сообщении в группах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2785b-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="2785b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2785b-105">Properties</span></span>

| <span data-ttu-id="2785b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2785b-106">Property</span></span>            | <span data-ttu-id="2785b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2785b-107">Type</span></span>    | <span data-ttu-id="2785b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2785b-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="2785b-109">MessageId</span><span class="sxs-lookup"><span data-stu-id="2785b-109">messageId</span></span>           | <span data-ttu-id="2785b-110">String</span><span class="sxs-lookup"><span data-stu-id="2785b-110">String</span></span>  | <span data-ttu-id="2785b-111">Уникальный идентификатор для сообщения в канале группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2785b-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="2785b-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="2785b-112">replyChainMessageId</span></span> | <span data-ttu-id="2785b-113">String</span><span class="sxs-lookup"><span data-stu-id="2785b-113">String</span></span>  | <span data-ttu-id="2785b-114">Идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="2785b-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="2785b-115">threadId</span><span class="sxs-lookup"><span data-stu-id="2785b-115">threadId</span></span>            | <span data-ttu-id="2785b-116">String</span><span class="sxs-lookup"><span data-stu-id="2785b-116">String</span></span>  | <span data-ttu-id="2785b-117">Уникальный идентификатор потока в группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2785b-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2785b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2785b-118">JSON representation</span></span>

<span data-ttu-id="2785b-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2785b-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatInfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
