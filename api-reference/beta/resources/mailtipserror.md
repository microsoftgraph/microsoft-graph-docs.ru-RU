---
title: Тип ресурса mailTipsError
description: Ошибка, возникающая во время действия.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 8e8a029eb00e5419f8c0e945e71dd0ba1ed2e147
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523990"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="e671b-103">Тип ресурса mailTipsError</span><span class="sxs-lookup"><span data-stu-id="e671b-103">mailTipsError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e671b-104">Ошибка, возникающая во время действия.</span><span class="sxs-lookup"><span data-stu-id="e671b-104">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="e671b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e671b-105">Properties</span></span>
| <span data-ttu-id="e671b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e671b-106">Property</span></span>     | <span data-ttu-id="e671b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e671b-107">Type</span></span>   |<span data-ttu-id="e671b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e671b-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="e671b-109">message</span><span class="sxs-lookup"><span data-stu-id="e671b-109">message</span></span> | <span data-ttu-id="e671b-110">String</span><span class="sxs-lookup"><span data-stu-id="e671b-110">String</span></span> | <span data-ttu-id="e671b-111">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e671b-111">The error message.</span></span> |
| <span data-ttu-id="e671b-112">code</span><span class="sxs-lookup"><span data-stu-id="e671b-112">code</span></span> | <span data-ttu-id="e671b-113">String</span><span class="sxs-lookup"><span data-stu-id="e671b-113">String</span></span> | <span data-ttu-id="e671b-114">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="e671b-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e671b-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e671b-115">JSON representation</span></span>

<span data-ttu-id="e671b-116">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e671b-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailtipserror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
