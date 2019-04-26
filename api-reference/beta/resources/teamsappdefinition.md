---
title: Тип ресурса Теамсаппдефинитион
description: Сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4b350c5ebe39da336dfe467bb73f5b91270dc31c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345805"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="51e43-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="51e43-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51e43-104">Сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="51e43-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="51e43-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="51e43-105">Properties</span></span>

| <span data-ttu-id="51e43-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="51e43-106">Property</span></span>            | <span data-ttu-id="51e43-107">Тип</span><span class="sxs-lookup"><span data-stu-id="51e43-107">Type</span></span>     | <span data-ttu-id="51e43-108">Описание</span><span class="sxs-lookup"><span data-stu-id="51e43-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="51e43-109">id</span><span class="sxs-lookup"><span data-stu-id="51e43-109">id</span></span>                  | <span data-ttu-id="51e43-110">строка</span><span class="sxs-lookup"><span data-stu-id="51e43-110">string</span></span>   | <span data-ttu-id="51e43-111">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="51e43-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="51e43-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="51e43-112">teamsAppId</span></span>          | <span data-ttu-id="51e43-113">строка</span><span class="sxs-lookup"><span data-stu-id="51e43-113">string</span></span>   | <span data-ttu-id="51e43-114">Идентификатор из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="51e43-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="51e43-115">displayName</span><span class="sxs-lookup"><span data-stu-id="51e43-115">displayName</span></span>         | <span data-ttu-id="51e43-116">string</span><span class="sxs-lookup"><span data-stu-id="51e43-116">string</span></span>   | <span data-ttu-id="51e43-117">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="51e43-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="51e43-118">version</span><span class="sxs-lookup"><span data-stu-id="51e43-118">version</span></span>             | <span data-ttu-id="51e43-119">строка</span><span class="sxs-lookup"><span data-stu-id="51e43-119">string</span></span>   | <span data-ttu-id="51e43-120">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="51e43-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="51e43-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="51e43-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="51e43-122">См. также</span><span class="sxs-lookup"><span data-stu-id="51e43-122">See also</span></span>

- [<span data-ttu-id="51e43-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="51e43-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="51e43-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="51e43-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="51e43-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="51e43-125">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

