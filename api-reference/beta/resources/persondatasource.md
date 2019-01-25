---
title: Тип ресурса personDataSource
description: Представляет источников, которые пользователь данные извлекаются из, например, каталогов и контактов Outlook.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 431cd9163873305508d5244005e6fe0a80501771
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509093"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="63807-103">Тип ресурса personDataSource</span><span class="sxs-lookup"><span data-stu-id="63807-103">personDataSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63807-104">Представляет источников, которые пользователь данные извлекаются из, например, каталогов и контактов Outlook.</span><span class="sxs-lookup"><span data-stu-id="63807-104">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63807-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63807-105">JSON representation</span></span>

<span data-ttu-id="63807-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="63807-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="63807-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="63807-107">Properties</span></span>
| <span data-ttu-id="63807-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="63807-108">Property</span></span>     | <span data-ttu-id="63807-109">Тип</span><span class="sxs-lookup"><span data-stu-id="63807-109">Type</span></span>   |<span data-ttu-id="63807-110">Описание</span><span class="sxs-lookup"><span data-stu-id="63807-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63807-111">type</span><span class="sxs-lookup"><span data-stu-id="63807-111">type</span></span>|<span data-ttu-id="63807-112">String</span><span class="sxs-lookup"><span data-stu-id="63807-112">String</span></span>|<span data-ttu-id="63807-113">Тип источника данных.</span><span class="sxs-lookup"><span data-stu-id="63807-113">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/persondatasource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
