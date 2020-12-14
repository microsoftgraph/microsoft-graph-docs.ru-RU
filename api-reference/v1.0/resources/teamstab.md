---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, закрепленная (прикрепленная) к каналу в команде. '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8314604d6ed15eeb154ff46c8e3b90f4be4f5cde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658550"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="812be-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="812be-103">teamsTab resource type</span></span>

<span data-ttu-id="812be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="812be-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="812be-105">TeamsTab — [это](../resources/teamstab.md) вкладка, закрепленная (прикрепленная) к [каналу](channel.md) в [команде.](team.md)</span><span class="sxs-lookup"><span data-stu-id="812be-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="812be-106">Методы</span><span class="sxs-lookup"><span data-stu-id="812be-106">Methods</span></span>

| <span data-ttu-id="812be-107">Метод</span><span class="sxs-lookup"><span data-stu-id="812be-107">Method</span></span>       | <span data-ttu-id="812be-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="812be-108">Return Type</span></span>  |<span data-ttu-id="812be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="812be-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="812be-110">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="812be-110">List tabs</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="812be-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="812be-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="812be-112">Перечисление вкладок, закрепленных на канале.</span><span class="sxs-lookup"><span data-stu-id="812be-112">List tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="812be-113">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="812be-113">Get tab</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="812be-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="812be-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="812be-115">Чтение вкладки, закрепленной в канале.</span><span class="sxs-lookup"><span data-stu-id="812be-115">Read a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="812be-116">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="812be-116">Add tab</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="812be-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="812be-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="812be-118">Добавление (закрепление) вкладки на канал.</span><span class="sxs-lookup"><span data-stu-id="812be-118">Add (pin) a tab to a channel.</span></span>|
|[<span data-ttu-id="812be-119">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="812be-119">Update tab</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="812be-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="812be-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="812be-121">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="812be-121">Update the tab properties.</span></span>|
|[<span data-ttu-id="812be-122">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="812be-122">Remove tab</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="812be-123">Нет</span><span class="sxs-lookup"><span data-stu-id="812be-123">None</span></span> | <span data-ttu-id="812be-124">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="812be-124">Remove (unpin) a tab from a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="812be-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="812be-125">Properties</span></span>

|<span data-ttu-id="812be-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="812be-126">Property</span></span>|<span data-ttu-id="812be-127">Тип</span><span class="sxs-lookup"><span data-stu-id="812be-127">Type</span></span>|<span data-ttu-id="812be-128">Описание</span><span class="sxs-lookup"><span data-stu-id="812be-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="812be-129">id</span><span class="sxs-lookup"><span data-stu-id="812be-129">id</span></span>              |   <span data-ttu-id="812be-130">string</span><span class="sxs-lookup"><span data-stu-id="812be-130">string</span></span>                  |  <span data-ttu-id="812be-131">Идентификатор, однозначно определяя определенный экземпляр вкладки канала. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="812be-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="812be-132">displayName</span><span class="sxs-lookup"><span data-stu-id="812be-132">displayName</span></span>            |   <span data-ttu-id="812be-133">string</span><span class="sxs-lookup"><span data-stu-id="812be-133">string</span></span>                  |  <span data-ttu-id="812be-134">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="812be-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="812be-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="812be-135">webUrl</span></span>          |   <span data-ttu-id="812be-136">string</span><span class="sxs-lookup"><span data-stu-id="812be-136">string</span></span>                  |  <span data-ttu-id="812be-137">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="812be-137">Deep link URL of the tab instance.</span></span> <span data-ttu-id="812be-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="812be-138">Read only.</span></span>     |
|  <span data-ttu-id="812be-139">configuration</span><span class="sxs-lookup"><span data-stu-id="812be-139">configuration</span></span>        |   [<span data-ttu-id="812be-140">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="812be-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="812be-141">Контейнер для настраиваемой настройки, примененной к вкладке. Вкладка считается настроенной только после настройки этого свойства.</span><span class="sxs-lookup"><span data-stu-id="812be-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="812be-142">Связи</span><span class="sxs-lookup"><span data-stu-id="812be-142">Relationships</span></span>

| <span data-ttu-id="812be-143">Связь</span><span class="sxs-lookup"><span data-stu-id="812be-143">Relationship</span></span> | <span data-ttu-id="812be-144">Тип</span><span class="sxs-lookup"><span data-stu-id="812be-144">Type</span></span>   | <span data-ttu-id="812be-145">Описание</span><span class="sxs-lookup"><span data-stu-id="812be-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="812be-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="812be-146">teamsApp</span></span>|[<span data-ttu-id="812be-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="812be-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="812be-148">Приложение, связанное со вкладками. Его нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="812be-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="812be-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="812be-149">JSON representation</span></span>

<span data-ttu-id="812be-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="812be-150">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="812be-151">См. также</span><span class="sxs-lookup"><span data-stu-id="812be-151">See also</span></span>

[<span data-ttu-id="812be-152">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="812be-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

