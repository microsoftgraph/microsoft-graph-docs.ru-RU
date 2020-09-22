---
title: Тип ресурса Теамсаппдефинитион
description: Сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d4d9cb74777985dd28988e1ebc417ee564932865
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046596"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="3e1f6-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="3e1f6-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="3e1f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e1f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e1f6-105">Сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="3e1f6-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3e1f6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e1f6-106">Properties</span></span>

| <span data-ttu-id="3e1f6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e1f6-107">Property</span></span>            | <span data-ttu-id="3e1f6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3e1f6-108">Type</span></span>     | <span data-ttu-id="3e1f6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3e1f6-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="3e1f6-110">id</span><span class="sxs-lookup"><span data-stu-id="3e1f6-110">id</span></span>                  | <span data-ttu-id="3e1f6-111">string</span><span class="sxs-lookup"><span data-stu-id="3e1f6-111">string</span></span>   | <span data-ttu-id="3e1f6-112">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="3e1f6-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="3e1f6-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="3e1f6-113">teamsAppId</span></span>          | <span data-ttu-id="3e1f6-114">string</span><span class="sxs-lookup"><span data-stu-id="3e1f6-114">string</span></span>   | <span data-ttu-id="3e1f6-115">Идентификатор из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="3e1f6-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="3e1f6-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="3e1f6-116">publishingState</span></span>| <span data-ttu-id="3e1f6-117">string</span><span class="sxs-lookup"><span data-stu-id="3e1f6-117">string</span></span>|<span data-ttu-id="3e1f6-118">Опубликованное состояние определенной версии приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="3e1f6-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="3e1f6-119">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="3e1f6-119">Possible values are:</span></span></br><span data-ttu-id="3e1f6-120">`submitted` — Определенная версия приложения Teams была отправлена и находится в процессе рецензирования.</span><span class="sxs-lookup"><span data-stu-id="3e1f6-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="3e1f6-121">`published`  — Запрос на публикацию определенной версии приложения Teams утвержден администратором, и приложение публикуется.</span><span class="sxs-lookup"><span data-stu-id="3e1f6-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="3e1f6-122">`rejected` — Запрос на публикацию определенной версии приложения Teams был отклонен администратором.</span><span class="sxs-lookup"><span data-stu-id="3e1f6-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="3e1f6-123">азуреадаппид</span><span class="sxs-lookup"><span data-stu-id="3e1f6-123">azureADAppId</span></span>        | <span data-ttu-id="3e1f6-124">string</span><span class="sxs-lookup"><span data-stu-id="3e1f6-124">string</span></span>   | <span data-ttu-id="3e1f6-125">WebApplicationInfo.id из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="3e1f6-125">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="3e1f6-126">displayName</span><span class="sxs-lookup"><span data-stu-id="3e1f6-126">displayName</span></span>         | <span data-ttu-id="3e1f6-127">string</span><span class="sxs-lookup"><span data-stu-id="3e1f6-127">string</span></span>   | <span data-ttu-id="3e1f6-128">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="3e1f6-128">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="3e1f6-129">version</span><span class="sxs-lookup"><span data-stu-id="3e1f6-129">version</span></span>             | <span data-ttu-id="3e1f6-130">string</span><span class="sxs-lookup"><span data-stu-id="3e1f6-130">string</span></span>   | <span data-ttu-id="3e1f6-131">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="3e1f6-131">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3e1f6-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3e1f6-132">JSON representation</span></span>

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
  "version": "1.0.0"
}
```

## <a name="see-also"></a><span data-ttu-id="3e1f6-133">См. также</span><span class="sxs-lookup"><span data-stu-id="3e1f6-133">See also</span></span>

- [<span data-ttu-id="3e1f6-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="3e1f6-134">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="3e1f6-135">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="3e1f6-135">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="3e1f6-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="3e1f6-136">teamsTab</span></span>](../resources/teamstab.md)

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


