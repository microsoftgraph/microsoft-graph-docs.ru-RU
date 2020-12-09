---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9d81c9f21d04690bcaa7360fb83595a13c7be156
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607030"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="a6c96-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="a6c96-103">teamsTab resource type</span></span>

<span data-ttu-id="a6c96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6c96-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a6c96-105">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="a6c96-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="a6c96-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a6c96-106">Methods</span></span>

| <span data-ttu-id="a6c96-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a6c96-107">Method</span></span>       | <span data-ttu-id="a6c96-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a6c96-108">Return Type</span></span>  |<span data-ttu-id="a6c96-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c96-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a6c96-110">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="a6c96-110">List tabs</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="a6c96-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a6c96-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a6c96-112">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="a6c96-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="a6c96-113">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="a6c96-113">Get tab</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="a6c96-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a6c96-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a6c96-115">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="a6c96-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="a6c96-116">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="a6c96-116">Add tab</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="a6c96-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a6c96-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a6c96-118">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="a6c96-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="a6c96-119">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="a6c96-119">Update tab</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="a6c96-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="a6c96-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="a6c96-121">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="a6c96-121">Updates the tab properties.</span></span>|
|[<span data-ttu-id="a6c96-122">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="a6c96-122">Remove tab</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="a6c96-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a6c96-123">None</span></span> | <span data-ttu-id="a6c96-124">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="a6c96-124">Removes (unpins) a tab from a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="a6c96-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6c96-125">Properties</span></span>

|<span data-ttu-id="a6c96-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6c96-126">Property</span></span>|<span data-ttu-id="a6c96-127">Тип</span><span class="sxs-lookup"><span data-stu-id="a6c96-127">Type</span></span>|<span data-ttu-id="a6c96-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c96-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="a6c96-129">id</span><span class="sxs-lookup"><span data-stu-id="a6c96-129">id</span></span>              |   <span data-ttu-id="a6c96-130">string</span><span class="sxs-lookup"><span data-stu-id="a6c96-130">string</span></span>                  |  <span data-ttu-id="a6c96-131">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="a6c96-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="a6c96-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a6c96-132">displayName</span></span>            |   <span data-ttu-id="a6c96-133">string</span><span class="sxs-lookup"><span data-stu-id="a6c96-133">string</span></span>                  |  <span data-ttu-id="a6c96-134">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="a6c96-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="a6c96-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="a6c96-135">webUrl</span></span>          |   <span data-ttu-id="a6c96-136">string</span><span class="sxs-lookup"><span data-stu-id="a6c96-136">string</span></span>                  |  <span data-ttu-id="a6c96-137">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="a6c96-137">Deep link URL of the tab instance.</span></span> <span data-ttu-id="a6c96-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a6c96-138">Read only.</span></span>     |
|  <span data-ttu-id="a6c96-139">configuration</span><span class="sxs-lookup"><span data-stu-id="a6c96-139">configuration</span></span>        |   [<span data-ttu-id="a6c96-140">теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a6c96-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="a6c96-141">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="a6c96-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="a6c96-142">Связи</span><span class="sxs-lookup"><span data-stu-id="a6c96-142">Relationships</span></span>

| <span data-ttu-id="a6c96-143">Связь</span><span class="sxs-lookup"><span data-stu-id="a6c96-143">Relationship</span></span> | <span data-ttu-id="a6c96-144">Тип</span><span class="sxs-lookup"><span data-stu-id="a6c96-144">Type</span></span>   | <span data-ttu-id="a6c96-145">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c96-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a6c96-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a6c96-146">teamsApp</span></span>|[<span data-ttu-id="a6c96-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="a6c96-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="a6c96-148">Приложение, связанное с вкладкой. Его нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="a6c96-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6c96-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6c96-149">JSON representation</span></span>

<span data-ttu-id="a6c96-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6c96-150">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="a6c96-151">См. также</span><span class="sxs-lookup"><span data-stu-id="a6c96-151">See also</span></span>

[<span data-ttu-id="a6c96-152">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="a6c96-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

