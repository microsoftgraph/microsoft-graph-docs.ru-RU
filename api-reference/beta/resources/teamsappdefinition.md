---
title: Тип ресурса teamsAppDefinition
description: Подробные сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 94e2c790f8bf4623e56ca76bde164b718ee6fa38
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509982"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="37f34-103">Тип ресурса teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="37f34-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37f34-104">Подробные сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="37f34-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="37f34-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="37f34-105">Properties</span></span>

| <span data-ttu-id="37f34-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="37f34-106">Property</span></span>            | <span data-ttu-id="37f34-107">Тип</span><span class="sxs-lookup"><span data-stu-id="37f34-107">Type</span></span>     | <span data-ttu-id="37f34-108">Описание</span><span class="sxs-lookup"><span data-stu-id="37f34-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="37f34-109">id</span><span class="sxs-lookup"><span data-stu-id="37f34-109">id</span></span>                  | <span data-ttu-id="37f34-110">string</span><span class="sxs-lookup"><span data-stu-id="37f34-110">string</span></span>   | <span data-ttu-id="37f34-111">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="37f34-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="37f34-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="37f34-112">teamsAppId</span></span>          | <span data-ttu-id="37f34-113">string</span><span class="sxs-lookup"><span data-stu-id="37f34-113">string</span></span>   | <span data-ttu-id="37f34-114">Идентификатор в манифесте приложения группы.</span><span class="sxs-lookup"><span data-stu-id="37f34-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="37f34-115">displayName</span><span class="sxs-lookup"><span data-stu-id="37f34-115">displayName</span></span>         | <span data-ttu-id="37f34-116">строка</span><span class="sxs-lookup"><span data-stu-id="37f34-116">string</span></span>   | <span data-ttu-id="37f34-117">Имя приложения, предоставляемый разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="37f34-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="37f34-118">version</span><span class="sxs-lookup"><span data-stu-id="37f34-118">version</span></span>             | <span data-ttu-id="37f34-119">string</span><span class="sxs-lookup"><span data-stu-id="37f34-119">string</span></span>   | <span data-ttu-id="37f34-120">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="37f34-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37f34-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37f34-121">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "Test App",
  "version": "1.0.0",
}
```

# <a name="see-also"></a><span data-ttu-id="37f34-122">См. также</span><span class="sxs-lookup"><span data-stu-id="37f34-122">See also</span></span>

- [<span data-ttu-id="37f34-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="37f34-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="37f34-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="37f34-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="37f34-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="37f34-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappdefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

