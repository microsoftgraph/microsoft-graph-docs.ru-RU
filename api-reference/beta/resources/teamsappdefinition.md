---
title: Тип ресурса Теамсаппдефинитион
description: Сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b8dd3e7b3e50ed5642aeb23076705f4995e27759
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272712"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="4db4a-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="4db4a-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="4db4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4db4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4db4a-105">Сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="4db4a-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4db4a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4db4a-106">Properties</span></span>

| <span data-ttu-id="4db4a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4db4a-107">Property</span></span>            | <span data-ttu-id="4db4a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4db4a-108">Type</span></span>     | <span data-ttu-id="4db4a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4db4a-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="4db4a-110">id</span><span class="sxs-lookup"><span data-stu-id="4db4a-110">id</span></span>                  | <span data-ttu-id="4db4a-111">string</span><span class="sxs-lookup"><span data-stu-id="4db4a-111">string</span></span>   | <span data-ttu-id="4db4a-112">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="4db4a-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="4db4a-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="4db4a-113">teamsAppId</span></span>          | <span data-ttu-id="4db4a-114">string</span><span class="sxs-lookup"><span data-stu-id="4db4a-114">string</span></span>   | <span data-ttu-id="4db4a-115">Идентификатор из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="4db4a-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="4db4a-116">азуреадаппид</span><span class="sxs-lookup"><span data-stu-id="4db4a-116">azureADAppId</span></span>        | <span data-ttu-id="4db4a-117">string</span><span class="sxs-lookup"><span data-stu-id="4db4a-117">string</span></span>   | <span data-ttu-id="4db4a-118">WebApplicationInfo.id из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="4db4a-118">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="4db4a-119">displayName</span><span class="sxs-lookup"><span data-stu-id="4db4a-119">displayName</span></span>         | <span data-ttu-id="4db4a-120">string</span><span class="sxs-lookup"><span data-stu-id="4db4a-120">string</span></span>   | <span data-ttu-id="4db4a-121">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="4db4a-121">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="4db4a-122">version</span><span class="sxs-lookup"><span data-stu-id="4db4a-122">version</span></span>             | <span data-ttu-id="4db4a-123">string</span><span class="sxs-lookup"><span data-stu-id="4db4a-123">string</span></span>   | <span data-ttu-id="4db4a-124">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="4db4a-124">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4db4a-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4db4a-125">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4db4a-126">См. также</span><span class="sxs-lookup"><span data-stu-id="4db4a-126">See also</span></span>

- [<span data-ttu-id="4db4a-127">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4db4a-127">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="4db4a-128">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="4db4a-128">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="4db4a-129">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4db4a-129">teamsTab</span></span>](../resources/teamstab.md)

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

