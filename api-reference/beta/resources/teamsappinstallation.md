---
title: Тип ресурса teamsAppInstallation
description: 'TeamsApp, установленные в группе. '
ms.openlocfilehash: 64573e163c0ec5ce9f3282e747dffd4ccc6718de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077813"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="a8c87-103">Тип ресурса teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a8c87-103">teamsAppInstallation resource type</span></span>

> <span data-ttu-id="a8c87-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a8c87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8c87-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8c87-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8c87-106">[TeamsApp](teamsapp.md) установлен в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="a8c87-106">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="a8c87-107">Любой программы-роботы, являющихся частью приложения становится частью любой группы добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="a8c87-107">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="a8c87-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a8c87-108">Methods</span></span>

| <span data-ttu-id="a8c87-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a8c87-109">Method</span></span>       | <span data-ttu-id="a8c87-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a8c87-110">Return Type</span></span>  |<span data-ttu-id="a8c87-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a8c87-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8c87-112">Список приложений</span><span class="sxs-lookup"><span data-stu-id="a8c87-112">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="a8c87-113">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a8c87-113">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="a8c87-114">Список приложений, установленные в группе.</span><span class="sxs-lookup"><span data-stu-id="a8c87-114">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="a8c87-115">Добавить приложение</span><span class="sxs-lookup"><span data-stu-id="a8c87-115">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="a8c87-116">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a8c87-116">teamsAppInstallation</span></span>](teamsapp.md) | <span data-ttu-id="a8c87-117">Добавляет (установить) приложения в группу.</span><span class="sxs-lookup"><span data-stu-id="a8c87-117">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="a8c87-118">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="a8c87-118">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="a8c87-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a8c87-119">None</span></span> | <span data-ttu-id="a8c87-120">Удаляет (удаление) приложения из группы.</span><span class="sxs-lookup"><span data-stu-id="a8c87-120">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="a8c87-121">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="a8c87-121">Upgrade app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="a8c87-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a8c87-122">None</span></span> | <span data-ttu-id="a8c87-123">Обновление до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="a8c87-123">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8c87-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8c87-124">Properties</span></span>

| <span data-ttu-id="a8c87-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8c87-125">Property</span></span>            | <span data-ttu-id="a8c87-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a8c87-126">Type</span></span>     | <span data-ttu-id="a8c87-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a8c87-127">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="a8c87-128">id</span><span class="sxs-lookup"><span data-stu-id="a8c87-128">id</span></span>                  | <span data-ttu-id="a8c87-129">строка</span><span class="sxs-lookup"><span data-stu-id="a8c87-129">string</span></span>   | <span data-ttu-id="a8c87-130">Уникальный идентификатор (не appid команды).</span><span class="sxs-lookup"><span data-stu-id="a8c87-130">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="a8c87-131">Связи</span><span class="sxs-lookup"><span data-stu-id="a8c87-131">Relationships</span></span>

| <span data-ttu-id="a8c87-132">Связь</span><span class="sxs-lookup"><span data-stu-id="a8c87-132">Relationship</span></span>   | <span data-ttu-id="a8c87-133">Тип</span><span class="sxs-lookup"><span data-stu-id="a8c87-133">Type</span></span>    | <span data-ttu-id="a8c87-134">Description</span><span class="sxs-lookup"><span data-stu-id="a8c87-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a8c87-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a8c87-135">teamsApp</span></span>|[<span data-ttu-id="a8c87-136">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a8c87-136">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="a8c87-137">Приложения, которая устанавливается.</span><span class="sxs-lookup"><span data-stu-id="a8c87-137">The app that is installed.</span></span> |
|<span data-ttu-id="a8c87-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a8c87-138">teamsAppDefinition</span></span>|[<span data-ttu-id="a8c87-139">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a8c87-139">teamsAppDefinition</span></span>](teamsapp.md)| <span data-ttu-id="a8c87-140">Подробные сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="a8c87-140">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8c87-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8c87-141">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="a8c87-142">См. также</span><span class="sxs-lookup"><span data-stu-id="a8c87-142">See also</span></span>

- [<span data-ttu-id="a8c87-143">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a8c87-143">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="a8c87-144">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="a8c87-144">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="a8c87-145">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a8c87-145">teamsTab</span></span>](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

