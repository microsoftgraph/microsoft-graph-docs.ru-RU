---
title: Тип ресурса электронной почты
description: Ниже представлено описание ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: cc1fc5bf69cb420b8cd0476a439123e90b236b48
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512586"
---
# <a name="email-resource-type"></a><span data-ttu-id="41355-103">Тип ресурса электронной почты</span><span class="sxs-lookup"><span data-stu-id="41355-103">email resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="41355-104">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41355-104">JSON representation</span></span>

<span data-ttu-id="41355-105">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="41355-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.email"
}-->

```json
{
  "address": "string"
}

```
## <a name="properties"></a><span data-ttu-id="41355-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="41355-106">Properties</span></span>
| <span data-ttu-id="41355-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="41355-107">Property</span></span>     | <span data-ttu-id="41355-108">Тип</span><span class="sxs-lookup"><span data-stu-id="41355-108">Type</span></span>   |<span data-ttu-id="41355-109">Описание</span><span class="sxs-lookup"><span data-stu-id="41355-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41355-110">address</span><span class="sxs-lookup"><span data-stu-id="41355-110">address</span></span>|<span data-ttu-id="41355-111">String</span><span class="sxs-lookup"><span data-stu-id="41355-111">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "email resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/email.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
