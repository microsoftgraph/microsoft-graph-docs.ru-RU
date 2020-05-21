---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1e3ed231c6bd741afe3dcd502d517006c402fc77
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335336"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="10d7e-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="10d7e-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="10d7e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10d7e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10d7e-105">[TeamsApp](teamsapp.md) , установленный в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="10d7e-105">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="10d7e-106">Все боты, которые входят в состав приложения, станут частью любой команды, в которую добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="10d7e-106">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="10d7e-107">Методы</span><span class="sxs-lookup"><span data-stu-id="10d7e-107">Methods</span></span>

| <span data-ttu-id="10d7e-108">Метод</span><span class="sxs-lookup"><span data-stu-id="10d7e-108">Method</span></span>       | <span data-ttu-id="10d7e-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="10d7e-109">Return Type</span></span>  |<span data-ttu-id="10d7e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="10d7e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="10d7e-111">Список приложений</span><span class="sxs-lookup"><span data-stu-id="10d7e-111">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="10d7e-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="10d7e-112">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="10d7e-113">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="10d7e-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="10d7e-114">Добавление приложения</span><span class="sxs-lookup"><span data-stu-id="10d7e-114">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="10d7e-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="10d7e-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="10d7e-116">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="10d7e-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="10d7e-117">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="10d7e-117">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="10d7e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="10d7e-118">None</span></span> | <span data-ttu-id="10d7e-119">Удаляет приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="10d7e-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="10d7e-120">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="10d7e-120">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="10d7e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="10d7e-121">None</span></span> | <span data-ttu-id="10d7e-122">Обновление до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="10d7e-122">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="10d7e-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="10d7e-123">Properties</span></span>

| <span data-ttu-id="10d7e-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="10d7e-124">Property</span></span>            | <span data-ttu-id="10d7e-125">Тип</span><span class="sxs-lookup"><span data-stu-id="10d7e-125">Type</span></span>     | <span data-ttu-id="10d7e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="10d7e-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="10d7e-127">id</span><span class="sxs-lookup"><span data-stu-id="10d7e-127">id</span></span>                  | <span data-ttu-id="10d7e-128">string</span><span class="sxs-lookup"><span data-stu-id="10d7e-128">string</span></span>   | <span data-ttu-id="10d7e-129">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="10d7e-129">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="10d7e-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="10d7e-130">Relationships</span></span>

| <span data-ttu-id="10d7e-131">Связь</span><span class="sxs-lookup"><span data-stu-id="10d7e-131">Relationship</span></span>   | <span data-ttu-id="10d7e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="10d7e-132">Type</span></span>    | <span data-ttu-id="10d7e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="10d7e-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="10d7e-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="10d7e-134">teamsApp</span></span>|[<span data-ttu-id="10d7e-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="10d7e-135">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="10d7e-136">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="10d7e-136">The app that is installed.</span></span> |
|<span data-ttu-id="10d7e-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="10d7e-137">teamsAppDefinition</span></span>|[<span data-ttu-id="10d7e-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="10d7e-138">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="10d7e-139">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="10d7e-139">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="10d7e-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="10d7e-140">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="10d7e-141">См. также</span><span class="sxs-lookup"><span data-stu-id="10d7e-141">See also</span></span>

- [<span data-ttu-id="10d7e-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="10d7e-142">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="10d7e-143">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="10d7e-143">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="10d7e-144">teamsTab</span><span class="sxs-lookup"><span data-stu-id="10d7e-144">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
