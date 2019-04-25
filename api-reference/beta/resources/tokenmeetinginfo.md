---
title: Тип ресурса Токенмитингинфо
description: Тип Токенмитингинфо.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8e115887e67f19375ca8b96a216af98c80e0b312
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523023"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="a75ee-103">Тип ресурса Токенмитингинфо</span><span class="sxs-lookup"><span data-stu-id="a75ee-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a75ee-104">Тип Токенмитингинфо.</span><span class="sxs-lookup"><span data-stu-id="a75ee-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="a75ee-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a75ee-105">Properties</span></span>

| <span data-ttu-id="a75ee-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a75ee-106">Property</span></span>                     | <span data-ttu-id="a75ee-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a75ee-107">Type</span></span>    | <span data-ttu-id="a75ee-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a75ee-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="a75ee-109">Алловконверсатионвисаусост</span><span class="sxs-lookup"><span data-stu-id="a75ee-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="a75ee-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="a75ee-110">Boolean</span></span> | <span data-ttu-id="a75ee-111">Указывает, может ли беседа продолжиться после закрытия узла беседы.</span><span class="sxs-lookup"><span data-stu-id="a75ee-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="a75ee-112">токен</span><span class="sxs-lookup"><span data-stu-id="a75ee-112">token</span></span>                        | <span data-ttu-id="a75ee-113">Строка</span><span class="sxs-lookup"><span data-stu-id="a75ee-113">String</span></span>  | <span data-ttu-id="a75ee-114">Токен для присоединения и активации собрания.</span><span class="sxs-lookup"><span data-stu-id="a75ee-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="a75ee-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a75ee-115">JSON representation</span></span>

<span data-ttu-id="a75ee-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a75ee-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="a75ee-117">Пример</span><span class="sxs-lookup"><span data-stu-id="a75ee-117">Example</span></span>

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
