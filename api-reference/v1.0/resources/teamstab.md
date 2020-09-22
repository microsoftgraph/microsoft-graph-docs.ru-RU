---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5209670c004da2b58d41444c0bfa31f12891b8d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074848"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="bb8c0-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="bb8c0-103">teamsTab resource type</span></span>

<span data-ttu-id="bb8c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb8c0-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="bb8c0-105">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="bb8c0-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="bb8c0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bb8c0-106">Methods</span></span>

| <span data-ttu-id="bb8c0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bb8c0-107">Method</span></span>       | <span data-ttu-id="bb8c0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bb8c0-108">Return Type</span></span>  |<span data-ttu-id="bb8c0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bb8c0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bb8c0-110">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="bb8c0-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="bb8c0-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bb8c0-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="bb8c0-112">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="bb8c0-113">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="bb8c0-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="bb8c0-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bb8c0-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="bb8c0-115">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="bb8c0-116">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="bb8c0-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="bb8c0-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bb8c0-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="bb8c0-118">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="bb8c0-119">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="bb8c0-119">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="bb8c0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="bb8c0-120">None</span></span> | <span data-ttu-id="bb8c0-121">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="bb8c0-122">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="bb8c0-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="bb8c0-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="bb8c0-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="bb8c0-124">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="bb8c0-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb8c0-125">Properties</span></span>

|<span data-ttu-id="bb8c0-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb8c0-126">Property</span></span>|<span data-ttu-id="bb8c0-127">Тип</span><span class="sxs-lookup"><span data-stu-id="bb8c0-127">Type</span></span>|<span data-ttu-id="bb8c0-128">Описание</span><span class="sxs-lookup"><span data-stu-id="bb8c0-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="bb8c0-129">id</span><span class="sxs-lookup"><span data-stu-id="bb8c0-129">id</span></span>              |   <span data-ttu-id="bb8c0-130">string</span><span class="sxs-lookup"><span data-stu-id="bb8c0-130">string</span></span>                  |  <span data-ttu-id="bb8c0-131">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="bb8c0-132">displayName</span><span class="sxs-lookup"><span data-stu-id="bb8c0-132">displayName</span></span>            |   <span data-ttu-id="bb8c0-133">string</span><span class="sxs-lookup"><span data-stu-id="bb8c0-133">string</span></span>                  |  <span data-ttu-id="bb8c0-134">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="bb8c0-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="bb8c0-135">webUrl</span></span>          |   <span data-ttu-id="bb8c0-136">string</span><span class="sxs-lookup"><span data-stu-id="bb8c0-136">string</span></span>                  |  <span data-ttu-id="bb8c0-137">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-137">Deep link URL of the tab instance.</span></span> <span data-ttu-id="bb8c0-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-138">Read only.</span></span>     |
|  <span data-ttu-id="bb8c0-139">configuration</span><span class="sxs-lookup"><span data-stu-id="bb8c0-139">configuration</span></span>        |   [<span data-ttu-id="bb8c0-140">теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bb8c0-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="bb8c0-141">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="bb8c0-142">Связи</span><span class="sxs-lookup"><span data-stu-id="bb8c0-142">Relationships</span></span>

| <span data-ttu-id="bb8c0-143">Связь</span><span class="sxs-lookup"><span data-stu-id="bb8c0-143">Relationship</span></span> | <span data-ttu-id="bb8c0-144">Тип</span><span class="sxs-lookup"><span data-stu-id="bb8c0-144">Type</span></span>   | <span data-ttu-id="bb8c0-145">Описание</span><span class="sxs-lookup"><span data-stu-id="bb8c0-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bb8c0-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="bb8c0-146">teamsApp</span></span>|[<span data-ttu-id="bb8c0-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="bb8c0-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="bb8c0-148">Приложение, связанное с вкладкой. Его нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bb8c0-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb8c0-149">JSON representation</span></span>

<span data-ttu-id="bb8c0-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb8c0-150">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="bb8c0-151">См. также</span><span class="sxs-lookup"><span data-stu-id="bb8c0-151">See also</span></span>

[<span data-ttu-id="bb8c0-152">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="bb8c0-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

