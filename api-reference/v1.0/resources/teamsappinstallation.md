---
title: Тип ресурса Теамсаппинсталлатион
description: 'TeamsApp, установленный в команде. '
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 70dfe86840bd908a2e626b7f965d89251b9221aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533500"
---
# <a name="teamsappinstallation-resource-type"></a><span data-ttu-id="080ee-103">Тип ресурса Теамсаппинсталлатион</span><span class="sxs-lookup"><span data-stu-id="080ee-103">teamsAppInstallation resource type</span></span>

<span data-ttu-id="080ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="080ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="080ee-105">[TeamsApp](teamsapp.md) , установленный в [команде](team.md).</span><span class="sxs-lookup"><span data-stu-id="080ee-105">A [teamsApp](teamsapp.md) installed in a [team](team.md).</span></span> <span data-ttu-id="080ee-106">Все боты, которые входят в состав приложения, станут частью любой команды, в которую добавляется приложение.</span><span class="sxs-lookup"><span data-stu-id="080ee-106">Any bots that are part of the app will become part of any team the app is added to.</span></span>

## <a name="methods"></a><span data-ttu-id="080ee-107">Методы</span><span class="sxs-lookup"><span data-stu-id="080ee-107">Methods</span></span>

| <span data-ttu-id="080ee-108">Метод</span><span class="sxs-lookup"><span data-stu-id="080ee-108">Method</span></span>       | <span data-ttu-id="080ee-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="080ee-109">Return Type</span></span>  |<span data-ttu-id="080ee-110">Описание</span><span class="sxs-lookup"><span data-stu-id="080ee-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="080ee-111">Список приложений</span><span class="sxs-lookup"><span data-stu-id="080ee-111">List apps</span></span>](../api/teamsappinstallation-list.md) | [<span data-ttu-id="080ee-112">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="080ee-112">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="080ee-113">Список приложений, установленных в команде.</span><span class="sxs-lookup"><span data-stu-id="080ee-113">Lists apps installed in a team.</span></span>|
|[<span data-ttu-id="080ee-114">Добавление приложения</span><span class="sxs-lookup"><span data-stu-id="080ee-114">Add app</span></span>](../api/teamsappinstallation-add.md) | [<span data-ttu-id="080ee-115">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="080ee-115">teamsAppInstallation</span></span>](teamsappinstallation.md) | <span data-ttu-id="080ee-116">Добавляет (устанавливает) приложение в команду.</span><span class="sxs-lookup"><span data-stu-id="080ee-116">Adds (installs) an app to a team.</span></span>|
|[<span data-ttu-id="080ee-117">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="080ee-117">Remove app</span></span>](../api/teamsappinstallation-delete.md) | <span data-ttu-id="080ee-118">Нет</span><span class="sxs-lookup"><span data-stu-id="080ee-118">None</span></span> | <span data-ttu-id="080ee-119">Удаляет приложение из команды.</span><span class="sxs-lookup"><span data-stu-id="080ee-119">Removes (uninstalls) an app from a team.</span></span>|
|[<span data-ttu-id="080ee-120">Обновление приложения</span><span class="sxs-lookup"><span data-stu-id="080ee-120">Upgrade app</span></span>](../api/teamsappinstallation-upgrade.md) | <span data-ttu-id="080ee-121">Нет</span><span class="sxs-lookup"><span data-stu-id="080ee-121">None</span></span> | <span data-ttu-id="080ee-122">Обновление до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="080ee-122">Upgrades to the latest version of the app.</span></span>|

## <a name="properties"></a><span data-ttu-id="080ee-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="080ee-123">Properties</span></span>

| <span data-ttu-id="080ee-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="080ee-124">Property</span></span>            | <span data-ttu-id="080ee-125">Тип</span><span class="sxs-lookup"><span data-stu-id="080ee-125">Type</span></span>     | <span data-ttu-id="080ee-126">Описание</span><span class="sxs-lookup"><span data-stu-id="080ee-126">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="080ee-127">id</span><span class="sxs-lookup"><span data-stu-id="080ee-127">id</span></span>                  | <span data-ttu-id="080ee-128">string</span><span class="sxs-lookup"><span data-stu-id="080ee-128">string</span></span>   | <span data-ttu-id="080ee-129">Уникальный идентификатор (а не идентификаторы Teams).</span><span class="sxs-lookup"><span data-stu-id="080ee-129">A unique id (not the teams appid).</span></span> |

## <a name="relationships"></a><span data-ttu-id="080ee-130">Связи</span><span class="sxs-lookup"><span data-stu-id="080ee-130">Relationships</span></span>

| <span data-ttu-id="080ee-131">Связь</span><span class="sxs-lookup"><span data-stu-id="080ee-131">Relationship</span></span>   | <span data-ttu-id="080ee-132">Тип</span><span class="sxs-lookup"><span data-stu-id="080ee-132">Type</span></span>    | <span data-ttu-id="080ee-133">Описание</span><span class="sxs-lookup"><span data-stu-id="080ee-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="080ee-134">teamsApp</span><span class="sxs-lookup"><span data-stu-id="080ee-134">teamsApp</span></span>|[<span data-ttu-id="080ee-135">teamsApp</span><span class="sxs-lookup"><span data-stu-id="080ee-135">teamsApp</span></span>](teamsapp.md)| <span data-ttu-id="080ee-136">Установленное приложение.</span><span class="sxs-lookup"><span data-stu-id="080ee-136">The app that is installed.</span></span> |
|<span data-ttu-id="080ee-137">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="080ee-137">teamsAppDefinition</span></span>|[<span data-ttu-id="080ee-138">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="080ee-138">teamsAppDefinition</span></span>](teamsappdefinition.md)| <span data-ttu-id="080ee-139">Сведения о данной версии приложения.</span><span class="sxs-lookup"><span data-stu-id="080ee-139">The details of this version of the app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="080ee-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="080ee-140">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="080ee-141">См. также</span><span class="sxs-lookup"><span data-stu-id="080ee-141">See also</span></span>

- [<span data-ttu-id="080ee-142">teamsApp</span><span class="sxs-lookup"><span data-stu-id="080ee-142">teamsApp</span></span>](teamsapp.md)
- [<span data-ttu-id="080ee-143">teamsAppDefinition</span><span class="sxs-lookup"><span data-stu-id="080ee-143">teamsAppDefinition</span></span>](teamsappdefinition.md)
- [<span data-ttu-id="080ee-144">teamsTab</span><span class="sxs-lookup"><span data-stu-id="080ee-144">teamsTab</span></span>](../resources/teamstab.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
