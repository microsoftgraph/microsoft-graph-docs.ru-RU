---
title: Тип ресурса Теамсаппдефинитион
description: Сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5e28a5e07d3572f91afd6f03ce5344e191467084
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033791"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="6b42f-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="6b42f-103">teamsAppDefinition resource type</span></span>



<span data-ttu-id="6b42f-104">Сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="6b42f-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6b42f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b42f-105">Properties</span></span>

| <span data-ttu-id="6b42f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b42f-106">Property</span></span>            | <span data-ttu-id="6b42f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6b42f-107">Type</span></span>     | <span data-ttu-id="6b42f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6b42f-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="6b42f-109">id</span><span class="sxs-lookup"><span data-stu-id="6b42f-109">id</span></span>                  | <span data-ttu-id="6b42f-110">string</span><span class="sxs-lookup"><span data-stu-id="6b42f-110">string</span></span>   | <span data-ttu-id="6b42f-111">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="6b42f-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="6b42f-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="6b42f-112">teamsAppId</span></span>          | <span data-ttu-id="6b42f-113">string</span><span class="sxs-lookup"><span data-stu-id="6b42f-113">string</span></span>   | <span data-ttu-id="6b42f-114">Идентификатор из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="6b42f-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="6b42f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="6b42f-115">displayName</span></span>         | <span data-ttu-id="6b42f-116">string</span><span class="sxs-lookup"><span data-stu-id="6b42f-116">string</span></span>   | <span data-ttu-id="6b42f-117">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="6b42f-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="6b42f-118">version</span><span class="sxs-lookup"><span data-stu-id="6b42f-118">version</span></span>             | <span data-ttu-id="6b42f-119">string</span><span class="sxs-lookup"><span data-stu-id="6b42f-119">string</span></span>   | <span data-ttu-id="6b42f-120">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="6b42f-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6b42f-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6b42f-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="6b42f-122">См. также</span><span class="sxs-lookup"><span data-stu-id="6b42f-122">See also</span></span>

- [<span data-ttu-id="6b42f-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="6b42f-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="6b42f-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="6b42f-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="6b42f-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6b42f-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

