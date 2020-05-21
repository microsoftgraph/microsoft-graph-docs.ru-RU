---
title: Тип ресурса Теамсаппдефинитион
description: Сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 95f701151370a6f741e7fa97aa1792ef67ad15d3
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334958"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="86c9d-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="86c9d-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="86c9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86c9d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="86c9d-105">Сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="86c9d-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="86c9d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="86c9d-106">Properties</span></span>

| <span data-ttu-id="86c9d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="86c9d-107">Property</span></span>            | <span data-ttu-id="86c9d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="86c9d-108">Type</span></span>     | <span data-ttu-id="86c9d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="86c9d-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="86c9d-110">id</span><span class="sxs-lookup"><span data-stu-id="86c9d-110">id</span></span>                  | <span data-ttu-id="86c9d-111">string</span><span class="sxs-lookup"><span data-stu-id="86c9d-111">string</span></span>   | <span data-ttu-id="86c9d-112">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="86c9d-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="86c9d-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="86c9d-113">teamsAppId</span></span>          | <span data-ttu-id="86c9d-114">string</span><span class="sxs-lookup"><span data-stu-id="86c9d-114">string</span></span>   | <span data-ttu-id="86c9d-115">Идентификатор из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="86c9d-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="86c9d-116">displayName</span><span class="sxs-lookup"><span data-stu-id="86c9d-116">displayName</span></span>         | <span data-ttu-id="86c9d-117">string</span><span class="sxs-lookup"><span data-stu-id="86c9d-117">string</span></span>   | <span data-ttu-id="86c9d-118">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="86c9d-118">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="86c9d-119">version</span><span class="sxs-lookup"><span data-stu-id="86c9d-119">version</span></span>             | <span data-ttu-id="86c9d-120">string</span><span class="sxs-lookup"><span data-stu-id="86c9d-120">string</span></span>   | <span data-ttu-id="86c9d-121">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="86c9d-121">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86c9d-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="86c9d-122">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="86c9d-123">См. также</span><span class="sxs-lookup"><span data-stu-id="86c9d-123">See also</span></span>

- [<span data-ttu-id="86c9d-124">teamsApp</span><span class="sxs-lookup"><span data-stu-id="86c9d-124">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="86c9d-125">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="86c9d-125">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="86c9d-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="86c9d-126">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

