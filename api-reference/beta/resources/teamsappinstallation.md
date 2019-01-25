---
title: Тип ресурса teamsAppInstallation
description: 'TeamsApp, установленные в группе. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b4cf14c36fc0ab0b33f88d4b330e76957e65164a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512838"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="c19b3-103">Тип ресурса teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c19b3-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c19b3-104">[TeamsApp](teamsapp.md) установлен в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="c19b3-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="c19b3-105">Любой программы-роботы, являющихся частью приложения становится частью любой группы добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="c19b3-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="c19b3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="c19b3-106">Methods</span></span>

| <span data-ttu-id="c19b3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="c19b3-107">Method</span></span>       | <span data-ttu-id="c19b3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c19b3-108">Return Type</span></span>  |<span data-ttu-id="c19b3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c19b3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c19b3-110">Список приложений</span><span class="sxs-lookup"><span data-stu-id="c19b3-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="c19b3-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c19b3-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="c19b3-112">Список приложений, установленные в группе.</span><span class="sxs-lookup"><span data-stu-id="c19b3-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="c19b3-113">Добавить приложение</span><span class="sxs-lookup"><span data-stu-id="c19b3-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="c19b3-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c19b3-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="c19b3-115">Добавляет (установить) приложения в группу.</span><span class="sxs-lookup"><span data-stu-id="c19b3-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="c19b3-116">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="c19b3-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="c19b3-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c19b3-117">None</span></span> | <span data-ttu-id="c19b3-118">Удаляет (удаление) приложения из группы.</span><span class="sxs-lookup"><span data-stu-id="c19b3-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="c19b3-119">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="c19b3-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="c19b3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c19b3-120">None</span></span> | <span data-ttu-id="c19b3-121">Обновление до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="c19b3-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="c19b3-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="c19b3-122">Properties</span></span>

| <span data-ttu-id="c19b3-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="c19b3-123">Property</span></span>            | <span data-ttu-id="c19b3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c19b3-124">Type</span></span>     | <span data-ttu-id="c19b3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c19b3-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="c19b3-126">id</span><span class="sxs-lookup"><span data-stu-id="c19b3-126">id</span></span>                  | <span data-ttu-id="c19b3-127">string</span><span class="sxs-lookup"><span data-stu-id="c19b3-127">string</span></span>   | <span data-ttu-id="c19b3-128">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="c19b3-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="c19b3-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="c19b3-129">Relationships</span></span>

| <span data-ttu-id="c19b3-130">Связь</span><span class="sxs-lookup"><span data-stu-id="c19b3-130">Relationship</span></span>   | <span data-ttu-id="c19b3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c19b3-131">Type</span></span>    | <span data-ttu-id="c19b3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c19b3-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c19b3-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c19b3-133">teamsApp</span></span>|[<span data-ttu-id="c19b3-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c19b3-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="c19b3-135">Приложения, которая устанавливается.</span><span class="sxs-lookup"><span data-stu-id="c19b3-135">The app that is installed.</span></span> |
|<span data-ttu-id="c19b3-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c19b3-136">teamsAppDefinition</span></span>|[<span data-ttu-id="c19b3-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c19b3-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="c19b3-138">Подробные сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="c19b3-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c19b3-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c19b3-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a><span data-ttu-id="c19b3-140">См. также</span><span class="sxs-lookup"><span data-stu-id="c19b3-140">See also</span></span>

- [<span data-ttu-id="c19b3-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c19b3-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="c19b3-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="c19b3-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="c19b3-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c19b3-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstallation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

