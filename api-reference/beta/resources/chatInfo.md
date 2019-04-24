---
title: Тип ресурса Чатинфо
description: Сведения о сообщении в Microsoft Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3c1414d10a262280bcf0d3a307fc0c71aed2fbde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461075"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="e8221-103">Тип ресурса Чатинфо</span><span class="sxs-lookup"><span data-stu-id="e8221-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8221-104">Сведения о сообщении в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e8221-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="e8221-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8221-105">Properties</span></span>

| <span data-ttu-id="e8221-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8221-106">Property</span></span>            | <span data-ttu-id="e8221-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e8221-107">Type</span></span>    | <span data-ttu-id="e8221-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e8221-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="e8221-109">messageId</span><span class="sxs-lookup"><span data-stu-id="e8221-109">messageId</span></span>           | <span data-ttu-id="e8221-110">String</span><span class="sxs-lookup"><span data-stu-id="e8221-110">String</span></span>  | <span data-ttu-id="e8221-111">Уникальный идентификатор сообщения в канале Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e8221-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="e8221-112">Репличаинмессажеид</span><span class="sxs-lookup"><span data-stu-id="e8221-112">replyChainMessageId</span></span> | <span data-ttu-id="e8221-113">String</span><span class="sxs-lookup"><span data-stu-id="e8221-113">String</span></span>  | <span data-ttu-id="e8221-114">Идентификатор ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="e8221-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="e8221-115">Tидентификатор</span><span class="sxs-lookup"><span data-stu-id="e8221-115">threadId</span></span>            | <span data-ttu-id="e8221-116">String</span><span class="sxs-lookup"><span data-stu-id="e8221-116">String</span></span>  | <span data-ttu-id="e8221-117">Уникальный идентификатор потока в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e8221-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e8221-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8221-118">JSON representation</span></span>

<span data-ttu-id="e8221-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8221-119">The following is a JSON representation of the resource.</span></span>

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
