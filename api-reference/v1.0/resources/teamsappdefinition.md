---
title: Тип ресурса Теамсаппдефинитион
description: Сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b71fb575eeb22f76419a88c7a56837bf34a31770
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533507"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="2e626-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="2e626-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="2e626-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e626-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="2e626-105">Сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="2e626-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2e626-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e626-106">Properties</span></span>

| <span data-ttu-id="2e626-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e626-107">Property</span></span>            | <span data-ttu-id="2e626-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2e626-108">Type</span></span>     | <span data-ttu-id="2e626-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2e626-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="2e626-110">id</span><span class="sxs-lookup"><span data-stu-id="2e626-110">id</span></span>                  | <span data-ttu-id="2e626-111">string</span><span class="sxs-lookup"><span data-stu-id="2e626-111">string</span></span>   | <span data-ttu-id="2e626-112">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="2e626-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="2e626-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="2e626-113">teamsAppId</span></span>          | <span data-ttu-id="2e626-114">string</span><span class="sxs-lookup"><span data-stu-id="2e626-114">string</span></span>   | <span data-ttu-id="2e626-115">Идентификатор из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="2e626-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="2e626-116">displayName</span><span class="sxs-lookup"><span data-stu-id="2e626-116">displayName</span></span>         | <span data-ttu-id="2e626-117">string</span><span class="sxs-lookup"><span data-stu-id="2e626-117">string</span></span>   | <span data-ttu-id="2e626-118">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="2e626-118">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="2e626-119">version</span><span class="sxs-lookup"><span data-stu-id="2e626-119">version</span></span>             | <span data-ttu-id="2e626-120">string</span><span class="sxs-lookup"><span data-stu-id="2e626-120">string</span></span>   | <span data-ttu-id="2e626-121">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="2e626-121">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e626-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2e626-122">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="2e626-123">См. также</span><span class="sxs-lookup"><span data-stu-id="2e626-123">See also</span></span>

- [<span data-ttu-id="2e626-124">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2e626-124">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="2e626-125">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2e626-125">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="2e626-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2e626-126">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

