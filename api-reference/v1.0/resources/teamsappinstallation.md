---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1a76d11472b3faef95e87ed4724f1397ebe467a6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033784"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="2933a-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="2933a-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="2933a-104">[TeamsApp](teamsapp.md) , установленный в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="2933a-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="2933a-105">Все боты, которые входят в состав приложения, станут частью любой команды, в которую добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="2933a-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="2933a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2933a-106">Methods</span></span>

| <span data-ttu-id="2933a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2933a-107">Method</span></span>       | <span data-ttu-id="2933a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2933a-108">Return Type</span></span>  |<span data-ttu-id="2933a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2933a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2933a-110">Список приложений</span><span class="sxs-lookup"><span data-stu-id="2933a-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="2933a-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2933a-111">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="2933a-112">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="2933a-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="2933a-113">Добавление приложения</span><span class="sxs-lookup"><span data-stu-id="2933a-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="2933a-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="2933a-114">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="2933a-115">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="2933a-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="2933a-116">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="2933a-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="2933a-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2933a-117">None</span></span> | <span data-ttu-id="2933a-118">Удаляет приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="2933a-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="2933a-119">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="2933a-119">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="2933a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2933a-120">None</span></span> | <span data-ttu-id="2933a-121">Обновление до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="2933a-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="2933a-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="2933a-122">Properties</span></span>

| <span data-ttu-id="2933a-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="2933a-123">Property</span></span>            | <span data-ttu-id="2933a-124">Тип</span><span class="sxs-lookup"><span data-stu-id="2933a-124">Type</span></span>     | <span data-ttu-id="2933a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2933a-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="2933a-126">id</span><span class="sxs-lookup"><span data-stu-id="2933a-126">id</span></span>                  | <span data-ttu-id="2933a-127">string</span><span class="sxs-lookup"><span data-stu-id="2933a-127">string</span></span>   | <span data-ttu-id="2933a-128">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="2933a-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="2933a-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="2933a-129">Relationships</span></span>

| <span data-ttu-id="2933a-130">Отношение</span><span class="sxs-lookup"><span data-stu-id="2933a-130">Relationship</span></span>   | <span data-ttu-id="2933a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2933a-131">Type</span></span>    | <span data-ttu-id="2933a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2933a-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2933a-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2933a-133">teamsApp</span></span>|[<span data-ttu-id="2933a-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2933a-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="2933a-135">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="2933a-135">The app that is installed.</span></span> |
|<span data-ttu-id="2933a-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2933a-136">teamsAppDefinition</span></span>|[<span data-ttu-id="2933a-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2933a-137">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="2933a-138">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="2933a-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2933a-139">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2933a-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="2933a-140">См. также</span><span class="sxs-lookup"><span data-stu-id="2933a-140">See also</span></span>

- [<span data-ttu-id="2933a-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="2933a-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="2933a-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="2933a-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="2933a-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="2933a-143">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
