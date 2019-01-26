---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая прикрепленных (вложенный) канала в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 181d2fd23ff922709b3e098f6069adf300ad3928
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574672"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="a0741-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0741-103">teamsTab resource type</span></span>



<span data-ttu-id="a0741-104">TeamsTab — [вкладку](../resources/teamstab.md) , которая прикрепленных (вложенный) [канала](channel.md) в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="a0741-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="a0741-105">Методы</span><span class="sxs-lookup"><span data-stu-id="a0741-105">Methods</span></span>

| <span data-ttu-id="a0741-106">Метод</span><span class="sxs-lookup"><span data-stu-id="a0741-106">Method</span></span>       | <span data-ttu-id="a0741-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a0741-107">Return Type</span></span>  |<span data-ttu-id="a0741-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a0741-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a0741-109">Список вкладок</span><span class="sxs-lookup"><span data-stu-id="a0741-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="a0741-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0741-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0741-111">Списки вкладок прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="a0741-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="a0741-112">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="a0741-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="a0741-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0741-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0741-114">Считывает вкладки, прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="a0741-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="a0741-115">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="a0741-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="a0741-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0741-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0741-117">Добавляет (PIN) вкладки на канал.</span><span class="sxs-lookup"><span data-stu-id="a0741-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="a0741-118">Удалить вкладку ""</span><span class="sxs-lookup"><span data-stu-id="a0741-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="a0741-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a0741-119">None</span></span> | <span data-ttu-id="a0741-120">Удаляет (отключит) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="a0741-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="a0741-121">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="a0741-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="a0741-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a0741-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a0741-123">Обновляет свойства вкладки.</span><span class="sxs-lookup"><span data-stu-id="a0741-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="a0741-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0741-124">Properties</span></span>

|<span data-ttu-id="a0741-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0741-125">Property</span></span>|<span data-ttu-id="a0741-126">Тип</span><span class="sxs-lookup"><span data-stu-id="a0741-126">Type</span></span>|<span data-ttu-id="a0741-127">Описание</span><span class="sxs-lookup"><span data-stu-id="a0741-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="a0741-128">id</span><span class="sxs-lookup"><span data-stu-id="a0741-128">id</span></span>              |   <span data-ttu-id="a0741-129">string</span><span class="sxs-lookup"><span data-stu-id="a0741-129">string</span></span>                  |  <span data-ttu-id="a0741-130">Идентификатор, который уникальным образом определяет определенный экземпляр канала вкладку чтения только.</span><span class="sxs-lookup"><span data-stu-id="a0741-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="a0741-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a0741-131">displayName</span></span>            |   <span data-ttu-id="a0741-132">string</span><span class="sxs-lookup"><span data-stu-id="a0741-132">string</span></span>                  |  <span data-ttu-id="a0741-133">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="a0741-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="a0741-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="a0741-134">webUrl</span></span>          |   <span data-ttu-id="a0741-135">string</span><span class="sxs-lookup"><span data-stu-id="a0741-135">string</span></span>                  |  <span data-ttu-id="a0741-136">Прямая ссылка URL-адрес экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="a0741-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="a0741-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a0741-137">Read only.</span></span>     |
|  <span data-ttu-id="a0741-138">configuration</span><span class="sxs-lookup"><span data-stu-id="a0741-138">configuration</span></span>        |   [<span data-ttu-id="a0741-139">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0741-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="a0741-140">Контейнер для пользовательских параметров, применяемых на вкладке. Вкладка считается настроены только после этого свойства.</span><span class="sxs-lookup"><span data-stu-id="a0741-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="a0741-141">Связи</span><span class="sxs-lookup"><span data-stu-id="a0741-141">Relationships</span></span>

| <span data-ttu-id="a0741-142">Связь</span><span class="sxs-lookup"><span data-stu-id="a0741-142">Relationship</span></span> | <span data-ttu-id="a0741-143">Тип</span><span class="sxs-lookup"><span data-stu-id="a0741-143">Type</span></span>   | <span data-ttu-id="a0741-144">Описание</span><span class="sxs-lookup"><span data-stu-id="a0741-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a0741-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a0741-145">teamsApp</span></span>|[<span data-ttu-id="a0741-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a0741-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a0741-147">Приложения, связанного с вкладки. Это нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="a0741-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a0741-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0741-148">JSON representation</span></span>

<span data-ttu-id="a0741-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0741-149">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a><span data-ttu-id="a0741-150">См. также</span><span class="sxs-lookup"><span data-stu-id="a0741-150">See also</span></span>

[<span data-ttu-id="a0741-151">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="a0741-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
