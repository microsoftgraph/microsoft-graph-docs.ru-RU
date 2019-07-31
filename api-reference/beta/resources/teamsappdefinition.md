---
title: Тип ресурса Теамсаппдефинитион
description: Сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c4849afe745a8554243bd37d85cb82d831e00a64
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007706"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="ffaa7-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="ffaa7-103">teamsAppDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffaa7-104">Сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="ffaa7-104">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ffaa7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffaa7-105">Properties</span></span>

| <span data-ttu-id="ffaa7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffaa7-106">Property</span></span>            | <span data-ttu-id="ffaa7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ffaa7-107">Type</span></span>     | <span data-ttu-id="ffaa7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ffaa7-108">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ffaa7-109">id</span><span class="sxs-lookup"><span data-stu-id="ffaa7-109">id</span></span>                  | <span data-ttu-id="ffaa7-110">string</span><span class="sxs-lookup"><span data-stu-id="ffaa7-110">string</span></span>   | <span data-ttu-id="ffaa7-111">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="ffaa7-111">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="ffaa7-112">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ffaa7-112">teamsAppId</span></span>          | <span data-ttu-id="ffaa7-113">string</span><span class="sxs-lookup"><span data-stu-id="ffaa7-113">string</span></span>   | <span data-ttu-id="ffaa7-114">Идентификатор из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="ffaa7-114">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="ffaa7-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ffaa7-115">displayName</span></span>         | <span data-ttu-id="ffaa7-116">string</span><span class="sxs-lookup"><span data-stu-id="ffaa7-116">string</span></span>   | <span data-ttu-id="ffaa7-117">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="ffaa7-117">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="ffaa7-118">version</span><span class="sxs-lookup"><span data-stu-id="ffaa7-118">version</span></span>             | <span data-ttu-id="ffaa7-119">string</span><span class="sxs-lookup"><span data-stu-id="ffaa7-119">string</span></span>   | <span data-ttu-id="ffaa7-120">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ffaa7-120">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ffaa7-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ffaa7-121">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="ffaa7-122">См. также</span><span class="sxs-lookup"><span data-stu-id="ffaa7-122">See also</span></span>

- [<span data-ttu-id="ffaa7-123">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ffaa7-123">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="ffaa7-124">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ffaa7-124">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="ffaa7-125">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ffaa7-125">teamsTab</span></span>](../resources/teamstab.md)

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

