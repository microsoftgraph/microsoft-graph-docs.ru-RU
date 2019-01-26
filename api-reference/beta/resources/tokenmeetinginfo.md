---
title: Тип ресурса tokenMeetingInfo
description: Тип tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 717bfbd14c92ea44987cbdadc25eef06ed31a0cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571074"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="b82d7-103">Тип ресурса tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="b82d7-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b82d7-104">Тип tokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="b82d7-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="b82d7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b82d7-105">Properties</span></span>

| <span data-ttu-id="b82d7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b82d7-106">Property</span></span>                     | <span data-ttu-id="b82d7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b82d7-107">Type</span></span>    | <span data-ttu-id="b82d7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b82d7-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="b82d7-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="b82d7-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="b82d7-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="b82d7-110">Boolean</span></span> | <span data-ttu-id="b82d7-111">Указывает, если беседы можно продолжить после покидает узла беседы.</span><span class="sxs-lookup"><span data-stu-id="b82d7-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="b82d7-112">токен</span><span class="sxs-lookup"><span data-stu-id="b82d7-112">token</span></span>                        | <span data-ttu-id="b82d7-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b82d7-113">String</span></span>  | <span data-ttu-id="b82d7-114">Маркер для присоединения к/активации собрания.</span><span class="sxs-lookup"><span data-stu-id="b82d7-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="b82d7-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b82d7-115">JSON representation</span></span>

<span data-ttu-id="b82d7-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b82d7-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.meetingInfo",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="b82d7-117">Пример</span><span class="sxs-lookup"><span data-stu-id="b82d7-117">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tokenmeetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
