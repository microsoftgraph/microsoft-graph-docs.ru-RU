---
title: Тип ресурса Теамсаппдефинитион
description: Представляет сведения о одной версии teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 322b7f50ccb51702ae05ca55f8e73396321a0283
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791682"
---
# <a name="teamsappdefinition-resource-type"></a><span data-ttu-id="13249-103">Тип ресурса Теамсаппдефинитион</span><span class="sxs-lookup"><span data-stu-id="13249-103">teamsAppDefinition resource type</span></span>

<span data-ttu-id="13249-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13249-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13249-105">Представляет сведения о одной версии [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="13249-105">Represents the details of one version of a [teamsApp](teamsapp.md).</span></span>

## <a name="properties"></a><span data-ttu-id="13249-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="13249-106">Properties</span></span>

| <span data-ttu-id="13249-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="13249-107">Property</span></span>            | <span data-ttu-id="13249-108">Тип</span><span class="sxs-lookup"><span data-stu-id="13249-108">Type</span></span>     | <span data-ttu-id="13249-109">Описание</span><span class="sxs-lookup"><span data-stu-id="13249-109">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="13249-110">id</span><span class="sxs-lookup"><span data-stu-id="13249-110">id</span></span>                  | <span data-ttu-id="13249-111">string</span><span class="sxs-lookup"><span data-stu-id="13249-111">string</span></span>   | <span data-ttu-id="13249-112">Уникальный идентификатор (не идентификатор приложения Teams).</span><span class="sxs-lookup"><span data-stu-id="13249-112">A unique ID (not the Teams app ID).</span></span> |
| <span data-ttu-id="13249-113">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="13249-113">teamsAppId</span></span>          | <span data-ttu-id="13249-114">string</span><span class="sxs-lookup"><span data-stu-id="13249-114">string</span></span>   | <span data-ttu-id="13249-115">ИДЕНТИФИКАТОР из манифеста приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="13249-115">The ID from the Teams app manifest.</span></span> |
| <span data-ttu-id="13249-116">publishingState</span><span class="sxs-lookup"><span data-stu-id="13249-116">publishingState</span></span>| <span data-ttu-id="13249-117">string</span><span class="sxs-lookup"><span data-stu-id="13249-117">string</span></span>|<span data-ttu-id="13249-118">Опубликованное состояние определенной версии приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="13249-118">The published status of a specific version of a Teams app.</span></span> <span data-ttu-id="13249-119">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="13249-119">Possible values are:</span></span></br><span data-ttu-id="13249-120">`submitted` — Определенная версия приложения Teams была отправлена и находится в процессе рецензирования.</span><span class="sxs-lookup"><span data-stu-id="13249-120">`submitted` — The specific version of the Teams app has been submitted and is under review.</span></span> </br><span data-ttu-id="13249-121">`published`  — Запрос на публикацию определенной версии приложения Teams утвержден администратором, и приложение публикуется.</span><span class="sxs-lookup"><span data-stu-id="13249-121">`published`  — The request to publish the specific version of the Teams app has been approved by the admin and the app is published.</span></span> </br> <span data-ttu-id="13249-122">`rejected` — Запрос на публикацию определенной версии приложения Teams был отклонен администратором.</span><span class="sxs-lookup"><span data-stu-id="13249-122">`rejected` — The request to publish the specific version of the Teams app was rejected by the admin.</span></span> |
| <span data-ttu-id="13249-123">displayName</span><span class="sxs-lookup"><span data-stu-id="13249-123">displayName</span></span>         | <span data-ttu-id="13249-124">string</span><span class="sxs-lookup"><span data-stu-id="13249-124">string</span></span>   | <span data-ttu-id="13249-125">Имя приложения, предоставленное разработчиком приложения.</span><span class="sxs-lookup"><span data-stu-id="13249-125">The name of the app provided by the app developer.</span></span> |
| <span data-ttu-id="13249-126">version</span><span class="sxs-lookup"><span data-stu-id="13249-126">version</span></span>             | <span data-ttu-id="13249-127">string</span><span class="sxs-lookup"><span data-stu-id="13249-127">string</span></span>   | <span data-ttu-id="13249-128">Номер версии приложения.</span><span class="sxs-lookup"><span data-stu-id="13249-128">The version number of the application.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="13249-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="13249-129">JSON representation</span></span>

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
  "version": "string",
}
```

## <a name="see-also"></a><span data-ttu-id="13249-130">См. также</span><span class="sxs-lookup"><span data-stu-id="13249-130">See also</span></span>

- [<span data-ttu-id="13249-131">teamsApp</span><span class="sxs-lookup"><span data-stu-id="13249-131">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="13249-132">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="13249-132">teamsAppInstallation</span></span>](teamsappinstallation.md)
- [<span data-ttu-id="13249-133">teamsTab</span><span class="sxs-lookup"><span data-stu-id="13249-133">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
