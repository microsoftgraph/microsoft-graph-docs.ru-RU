---
title: Тип ресурса teamsTemplate
description: Описание сущности teamsTemplate.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e75b3d8df318b116d5d908a40d4f756d9ee70864
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513048"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="d6444-103">Тип ресурса teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="d6444-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6444-104">Шаблон группы — это план для создания [группы](../resources/team.md) в группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d6444-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="d6444-105">Шаблон указывает структуры, параметры и даже контента, который следует предоставить в новые группы, созданные на основе шаблона.</span><span class="sxs-lookup"><span data-stu-id="d6444-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="d6444-106">Корпорация Майкрософт предоставляет набор базовых шаблонов и пользователи могут сохранять свои собственные пользовательские шаблоны.</span><span class="sxs-lookup"><span data-stu-id="d6444-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="d6444-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6444-107">Properties</span></span>

| <span data-ttu-id="d6444-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6444-108">Property</span></span>            | <span data-ttu-id="d6444-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d6444-109">Type</span></span>     | <span data-ttu-id="d6444-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d6444-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="d6444-111">id</span><span class="sxs-lookup"><span data-stu-id="d6444-111">id</span></span>                  | <span data-ttu-id="d6444-112">String</span><span class="sxs-lookup"><span data-stu-id="d6444-112">String</span></span>   | <span data-ttu-id="d6444-113">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="d6444-113">Unique identifier of the template.</span></span> <span data-ttu-id="d6444-114">Не может быть null.</span><span class="sxs-lookup"><span data-stu-id="d6444-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d6444-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6444-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="d6444-116">См. также</span><span class="sxs-lookup"><span data-stu-id="d6444-116">See also</span></span>

- <span data-ttu-id="d6444-117">Команда</span><span class="sxs-lookup"><span data-stu-id="d6444-117">[team](team.md)</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
