---
title: Тип ресурса Теамсаппдефинитион
description: Представляет сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 08a652c5b4ad4b9555eb7c09e33398f140ed97b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036935"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="20f5a-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="20f5a-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="20f5a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20f5a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="20f5a-105">Представляет сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="20f5a-105">Represents the details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="20f5a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="20f5a-106">Properties</span></span>

| <span data-ttu-id="20f5a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="20f5a-107">Property</span></span>            | <span data-ttu-id="20f5a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="20f5a-108">Type</span></span>     | <span data-ttu-id="20f5a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="20f5a-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="20f5a-110">id</span><span class="sxs-lookup"><span data-stu-id="20f5a-110">id</span></span>                  | <span data-ttu-id="20f5a-111">string</span><span class="sxs-lookup"><span data-stu-id="20f5a-111">string</span></span>   | <span data-ttu-id="20f5a-112">Уникальный идентификатор (не идентификатор приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="20f5a-112">A unique ID (not the Teams app ID).</span></span> |
| <span data-ttu-id="20f5a-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="20f5a-113">teamsAppId</span></span>          | <span data-ttu-id="20f5a-114">string</span><span class="sxs-lookup"><span data-stu-id="20f5a-114">string</span></span>   | <span data-ttu-id="20f5a-115">ИДЕНТИФИКАТОР из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="20f5a-115">The ID from the Teams app manifest.</span></span> |
| <span data-ttu-id="20f5a-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="20f5a-116">publishingState</span></span>| <span data-ttu-id="20f5a-117">string</span><span class="sxs-lookup"><span data-stu-id="20f5a-117">string</span></span>|<span data-ttu-id="20f5a-118">Опубликованное состояние определенной версии приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="20f5a-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="20f5a-119">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="20f5a-119">Possible values are:</span></span></br><span data-ttu-id="20f5a-120">`submitted` — Определенная версия приложения Teams была отправлена и находится в процессе рецензирования.</span><span class="sxs-lookup"><span data-stu-id="20f5a-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="20f5a-121">`published`  — Запрос на публикацию определенной версии приложения Teams утвержден администратором, и приложение публикуется.</span><span class="sxs-lookup"><span data-stu-id="20f5a-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="20f5a-122">`rejected` — Запрос на публикацию определенной версии приложения Teams был отклонен администратором.</span><span class="sxs-lookup"><span data-stu-id="20f5a-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="20f5a-123">displayName</span><span class="sxs-lookup"><span data-stu-id="20f5a-123">displayName</span></span>         | <span data-ttu-id="20f5a-124">string</span><span class="sxs-lookup"><span data-stu-id="20f5a-124">string</span></span>   | <span data-ttu-id="20f5a-125">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="20f5a-125">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="20f5a-126">version</span><span class="sxs-lookup"><span data-stu-id="20f5a-126">version</span></span>             | <span data-ttu-id="20f5a-127">string</span><span class="sxs-lookup"><span data-stu-id="20f5a-127">string</span></span>   | <span data-ttu-id="20f5a-128">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="20f5a-128">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20f5a-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="20f5a-129">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
  "teamsAppId": "string",
  "displayName": "string",
  "version": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="20f5a-130">См. также</span><span class="sxs-lookup"><span data-stu-id="20f5a-130">See also</span></span>

- [<span data-ttu-id="20f5a-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="20f5a-131">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="20f5a-132">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="20f5a-132">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="20f5a-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="20f5a-133">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

