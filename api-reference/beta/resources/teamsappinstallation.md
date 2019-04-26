---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8d8770a21b11c9ba1042c9a0f59d9405dce96f9d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345808"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="ec5ce-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="ec5ce-103">teamsAppInstallation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec5ce-104">[TeamsApp](teamsapp.md) , установленный в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="ec5ce-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="ec5ce-105">Все боты, которые входят в состав приложения, станут частью любой команды, в которую добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="ec5ce-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="ec5ce-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ec5ce-106">Methods</span></span>

| <span data-ttu-id="ec5ce-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ec5ce-107">Method</span></span>       | <span data-ttu-id="ec5ce-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec5ce-108">Return Type</span></span>  |<span data-ttu-id="ec5ce-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ec5ce-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec5ce-110">Список приложений</span><span class="sxs-lookup"><span data-stu-id="ec5ce-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="ec5ce-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ec5ce-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="ec5ce-112">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="ec5ce-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="ec5ce-113">Добавление приложения</span><span class="sxs-lookup"><span data-stu-id="ec5ce-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="ec5ce-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ec5ce-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="ec5ce-115">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="ec5ce-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="ec5ce-116">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="ec5ce-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="ec5ce-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ec5ce-117">None</span></span> | <span data-ttu-id="ec5ce-118">Удаляет приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="ec5ce-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="ec5ce-119">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="ec5ce-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="ec5ce-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ec5ce-120">None</span></span> | <span data-ttu-id="ec5ce-121">Обновление до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ec5ce-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec5ce-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec5ce-122">Properties</span></span>

| <span data-ttu-id="ec5ce-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec5ce-123">Property</span></span>            | <span data-ttu-id="ec5ce-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ec5ce-124">Type</span></span>     | <span data-ttu-id="ec5ce-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ec5ce-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ec5ce-126">id</span><span class="sxs-lookup"><span data-stu-id="ec5ce-126">id</span></span>                  | <span data-ttu-id="ec5ce-127">строка</span><span class="sxs-lookup"><span data-stu-id="ec5ce-127">string</span></span>   | <span data-ttu-id="ec5ce-128">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="ec5ce-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="ec5ce-129">Связи</span><span class="sxs-lookup"><span data-stu-id="ec5ce-129">Relationships</span></span>

| <span data-ttu-id="ec5ce-130">Отношение</span><span class="sxs-lookup"><span data-stu-id="ec5ce-130">Relationship</span></span>   | <span data-ttu-id="ec5ce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ec5ce-131">Type</span></span>    | <span data-ttu-id="ec5ce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ec5ce-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ec5ce-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ec5ce-133">teamsApp</span></span>|[<span data-ttu-id="ec5ce-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ec5ce-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="ec5ce-135">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="ec5ce-135">The app that is installed.</span></span> |
|<span data-ttu-id="ec5ce-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ec5ce-136">teamsAppDefinition</span></span>|[<span data-ttu-id="ec5ce-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ec5ce-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="ec5ce-138">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="ec5ce-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ec5ce-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ec5ce-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="ec5ce-140">См. также</span><span class="sxs-lookup"><span data-stu-id="ec5ce-140">See also</span></span>

- [<span data-ttu-id="ec5ce-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ec5ce-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="ec5ce-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="ec5ce-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="ec5ce-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ec5ce-143">teamsTab</span></span>](../resources/teamstab.md)


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

