---
title: Тип ресурса teamsAppInstallation
description: 'TeamsApp, установленные в группе. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 037cda1a98f45db94ecfc31b112bc3ab82bf4698
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891191"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="be468-103">Тип ресурса teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="be468-103">teamsAppInstallation resource type</span></span>



<span data-ttu-id="be468-104">[TeamsApp](teamsapp.md) установлен в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="be468-104">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="be468-105">Любой программы-роботы, являющихся частью приложения становится частью любой группы добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="be468-105">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="be468-106">Методы</span><span class="sxs-lookup"><span data-stu-id="be468-106">Methods</span></span>

| <span data-ttu-id="be468-107">Метод</span><span class="sxs-lookup"><span data-stu-id="be468-107">Method</span></span>       | <span data-ttu-id="be468-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be468-108">Return Type</span></span>  |<span data-ttu-id="be468-109">Описание</span><span class="sxs-lookup"><span data-stu-id="be468-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be468-110">Список приложений</span><span class="sxs-lookup"><span data-stu-id="be468-110">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="be468-111">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="be468-111">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="be468-112">Список приложений, установленные в группе.</span><span class="sxs-lookup"><span data-stu-id="be468-112">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="be468-113">Добавить приложение</span><span class="sxs-lookup"><span data-stu-id="be468-113">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="be468-114">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="be468-114">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="be468-115">Добавляет (установить) приложения в группу.</span><span class="sxs-lookup"><span data-stu-id="be468-115">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="be468-116">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="be468-116">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="be468-117">Нет</span><span class="sxs-lookup"><span data-stu-id="be468-117">None</span></span> | <span data-ttu-id="be468-118">Удаляет (удаление) приложения из группы.</span><span class="sxs-lookup"><span data-stu-id="be468-118">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="be468-119">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="be468-119">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="be468-120">Нет</span><span class="sxs-lookup"><span data-stu-id="be468-120">None</span></span> | <span data-ttu-id="be468-121">Обновление до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="be468-121">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="be468-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="be468-122">Properties</span></span>

| <span data-ttu-id="be468-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="be468-123">Property</span></span>            | <span data-ttu-id="be468-124">Тип</span><span class="sxs-lookup"><span data-stu-id="be468-124">Type</span></span>     | <span data-ttu-id="be468-125">Описание</span><span class="sxs-lookup"><span data-stu-id="be468-125">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="be468-126">id</span><span class="sxs-lookup"><span data-stu-id="be468-126">id</span></span>                  | <span data-ttu-id="be468-127">строка</span><span class="sxs-lookup"><span data-stu-id="be468-127">string</span></span>   | <span data-ttu-id="be468-128">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="be468-128">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="be468-129">Связи</span><span class="sxs-lookup"><span data-stu-id="be468-129">Relationships</span></span>

| <span data-ttu-id="be468-130">Связь</span><span class="sxs-lookup"><span data-stu-id="be468-130">Relationship</span></span>   | <span data-ttu-id="be468-131">Тип</span><span class="sxs-lookup"><span data-stu-id="be468-131">Type</span></span>    | <span data-ttu-id="be468-132">Описание</span><span class="sxs-lookup"><span data-stu-id="be468-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="be468-133">teamsApp</span><span class="sxs-lookup"><span data-stu-id="be468-133">teamsApp</span></span>|[<span data-ttu-id="be468-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="be468-134">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="be468-135">Приложения, которая устанавливается.</span><span class="sxs-lookup"><span data-stu-id="be468-135">The app that is installed.</span></span> |
|<span data-ttu-id="be468-136">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="be468-136">teamsAppDefinition</span></span>|[<span data-ttu-id="be468-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="be468-137">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="be468-138">Подробные сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="be468-138">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="be468-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be468-139">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="be468-140">См. также</span><span class="sxs-lookup"><span data-stu-id="be468-140">See also</span></span>

- [<span data-ttu-id="be468-141">teamsApp</span><span class="sxs-lookup"><span data-stu-id="be468-141">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="be468-142">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="be468-142">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="be468-143">teamsTab</span><span class="sxs-lookup"><span data-stu-id="be468-143">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

