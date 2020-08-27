---
title: Тип ресурса Теамсаппдефинитион
description: Сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6f8cb1f316bf9051dba0fe0ac138d75faf95c8d7
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287493"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="7c7ce-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="7c7ce-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="7c7ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c7ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c7ce-105">Сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c7ce-105">The details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7c7ce-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c7ce-106">Properties</span></span>

| <span data-ttu-id="7c7ce-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c7ce-107">Property</span></span>            | <span data-ttu-id="7c7ce-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7c7ce-108">Type</span></span>     | <span data-ttu-id="7c7ce-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7c7ce-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7c7ce-110">id</span><span class="sxs-lookup"><span data-stu-id="7c7ce-110">id</span></span>                  | <span data-ttu-id="7c7ce-111">string</span><span class="sxs-lookup"><span data-stu-id="7c7ce-111">string</span></span>   | <span data-ttu-id="7c7ce-112">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="7c7ce-112">A unique id (not the teams appid).</span></span> |
| <span data-ttu-id="7c7ce-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="7c7ce-113">teamsAppId</span></span>          | <span data-ttu-id="7c7ce-114">string</span><span class="sxs-lookup"><span data-stu-id="7c7ce-114">string</span></span>   | <span data-ttu-id="7c7ce-115">Идентификатор из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="7c7ce-115">The id from the Teams App manifest.</span></span> |
| <span data-ttu-id="7c7ce-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="7c7ce-116">publishingState</span></span>| <span data-ttu-id="7c7ce-117">string</span><span class="sxs-lookup"><span data-stu-id="7c7ce-117">string</span></span>|<span data-ttu-id="7c7ce-118">Опубликованное состояние определенной версии приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="7c7ce-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="7c7ce-119">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="7c7ce-119">Possible values are:</span></span></br><span data-ttu-id="7c7ce-120">`submitted` — Определенная версия приложения Teams была отправлена и находится в процессе рецензирования.</span><span class="sxs-lookup"><span data-stu-id="7c7ce-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="7c7ce-121">`published`  — Запрос на публикацию определенной версии приложения Teams утвержден администратором, и приложение публикуется.</span><span class="sxs-lookup"><span data-stu-id="7c7ce-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="7c7ce-122">`rejected` — Запрос на публикацию определенной версии приложения Teams был отклонен администратором.</span><span class="sxs-lookup"><span data-stu-id="7c7ce-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="7c7ce-123">азуреадаппид</span><span class="sxs-lookup"><span data-stu-id="7c7ce-123">azureADAppId</span></span>        | <span data-ttu-id="7c7ce-124">string</span><span class="sxs-lookup"><span data-stu-id="7c7ce-124">string</span></span>   | <span data-ttu-id="7c7ce-125">WebApplicationInfo.id из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="7c7ce-125">The WebApplicationInfo.id from the Teams App manifest.</span></span> |
| <span data-ttu-id="7c7ce-126">displayName</span><span class="sxs-lookup"><span data-stu-id="7c7ce-126">displayName</span></span>         | <span data-ttu-id="7c7ce-127">string</span><span class="sxs-lookup"><span data-stu-id="7c7ce-127">string</span></span>   | <span data-ttu-id="7c7ce-128">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="7c7ce-128">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="7c7ce-129">version</span><span class="sxs-lookup"><span data-stu-id="7c7ce-129">version</span></span>             | <span data-ttu-id="7c7ce-130">string</span><span class="sxs-lookup"><span data-stu-id="7c7ce-130">string</span></span>   | <span data-ttu-id="7c7ce-131">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="7c7ce-131">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c7ce-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7c7ce-132">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7c7ce-133">См. также</span><span class="sxs-lookup"><span data-stu-id="7c7ce-133">See also</span></span>

- [<span data-ttu-id="7c7ce-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="7c7ce-134">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="7c7ce-135">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7c7ce-135">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="7c7ce-136">teamsTab</span><span class="sxs-lookup"><span data-stu-id="7c7ce-136">teamsTab</span></span>](../resources/teamstab.md)

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
