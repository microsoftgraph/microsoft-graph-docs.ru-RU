---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, закрепленная (прикрепленная) к каналу в команде. '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 38351b0bde174b03f0e01392e7c8ec9c4df0db44
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660116"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="6e622-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e622-103">teamsTab resource type</span></span>

<span data-ttu-id="6e622-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e622-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e622-105">TeamsTab — [это](../resources/teamstab.md) вкладка, закрепленная (прикрепленная) к [каналу](channel.md) в [команде.](team.md)</span><span class="sxs-lookup"><span data-stu-id="6e622-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="6e622-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6e622-106">Methods</span></span>

| <span data-ttu-id="6e622-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6e622-107">Method</span></span>       | <span data-ttu-id="6e622-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6e622-108">Return Type</span></span>  |<span data-ttu-id="6e622-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6e622-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e622-110">Список вкладок на канале</span><span class="sxs-lookup"><span data-stu-id="6e622-110">List tabs in channel</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="6e622-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e622-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e622-112">Перечисление вкладок, закрепленных на канале.</span><span class="sxs-lookup"><span data-stu-id="6e622-112">List tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="6e622-113">Получение вкладки на канале</span><span class="sxs-lookup"><span data-stu-id="6e622-113">Get tab in channel</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="6e622-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e622-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e622-115">Получение определенной вкладки, закрепленной на канале.</span><span class="sxs-lookup"><span data-stu-id="6e622-115">Get a specific tab pinned to a channel.</span></span>|
|[<span data-ttu-id="6e622-116">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="6e622-116">Add tab to channel</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="6e622-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e622-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e622-118">Добавление (закрепление) вкладки на канал.</span><span class="sxs-lookup"><span data-stu-id="6e622-118">Add (pin) a tab to a channel.</span></span>|
|[<span data-ttu-id="6e622-119">Вкладка "обновление" на канале</span><span class="sxs-lookup"><span data-stu-id="6e622-119">Update tab in channel</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="6e622-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e622-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e622-121">Обновляет свойства вкладки на канале.</span><span class="sxs-lookup"><span data-stu-id="6e622-121">Updates the properties of a tab in a channel.</span></span>|
|[<span data-ttu-id="6e622-122">Удаление вкладки из канала</span><span class="sxs-lookup"><span data-stu-id="6e622-122">Remove tab from channel</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="6e622-123">Нет</span><span class="sxs-lookup"><span data-stu-id="6e622-123">None</span></span> | <span data-ttu-id="6e622-124">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="6e622-124">Remove (unpin) a tab from a channel.</span></span>|
|[<span data-ttu-id="6e622-125">Список вкладок в чате</span><span class="sxs-lookup"><span data-stu-id="6e622-125">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="6e622-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e622-126">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e622-127">Список вкладок, закрепленных в чате.</span><span class="sxs-lookup"><span data-stu-id="6e622-127">List tabs pinned to a chat.</span></span>|
|[<span data-ttu-id="6e622-128">Получить вкладку в чате</span><span class="sxs-lookup"><span data-stu-id="6e622-128">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="6e622-129">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e622-129">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e622-130">Получите определенную вкладку, закрепленную в чате.</span><span class="sxs-lookup"><span data-stu-id="6e622-130">Get a specific tab pinned to a chat.</span></span>|
|[<span data-ttu-id="6e622-131">Добавление вкладки в чат</span><span class="sxs-lookup"><span data-stu-id="6e622-131">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="6e622-132">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e622-132">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e622-133">Добавление (закрепление) вкладки в чат.</span><span class="sxs-lookup"><span data-stu-id="6e622-133">Add (pin) a tab to a chat.</span></span>|
|[<span data-ttu-id="6e622-134">Вкладка "Обновление" в чате</span><span class="sxs-lookup"><span data-stu-id="6e622-134">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="6e622-135">teamsTab</span><span class="sxs-lookup"><span data-stu-id="6e622-135">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="6e622-136">Обновление свойств вкладки в чате.</span><span class="sxs-lookup"><span data-stu-id="6e622-136">Update the properties of a tab in a chat.</span></span>|
|[<span data-ttu-id="6e622-137">Удаление вкладки из чата</span><span class="sxs-lookup"><span data-stu-id="6e622-137">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="6e622-138">Нет</span><span class="sxs-lookup"><span data-stu-id="6e622-138">None</span></span> | <span data-ttu-id="6e622-139">Удалите (открепите) вкладку из чата.</span><span class="sxs-lookup"><span data-stu-id="6e622-139">Remove (unpin) a tab from a chat.</span></span>|



## <a name="properties"></a><span data-ttu-id="6e622-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e622-140">Properties</span></span>

|<span data-ttu-id="6e622-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e622-141">Property</span></span>|<span data-ttu-id="6e622-142">Тип</span><span class="sxs-lookup"><span data-stu-id="6e622-142">Type</span></span>|<span data-ttu-id="6e622-143">Описание</span><span class="sxs-lookup"><span data-stu-id="6e622-143">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="6e622-144">id</span><span class="sxs-lookup"><span data-stu-id="6e622-144">id</span></span>              |   <span data-ttu-id="6e622-145">string</span><span class="sxs-lookup"><span data-stu-id="6e622-145">string</span></span>                  |  <span data-ttu-id="6e622-146">Идентификатор, однозначно определяя определенный экземпляр вкладки канала. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e622-146">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="6e622-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6e622-147">displayName</span></span>            |   <span data-ttu-id="6e622-148">string</span><span class="sxs-lookup"><span data-stu-id="6e622-148">string</span></span>                  |  <span data-ttu-id="6e622-149">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="6e622-149">Name of the tab.</span></span>     |
|  <span data-ttu-id="6e622-150">name (неподготовленное)</span><span class="sxs-lookup"><span data-stu-id="6e622-150">name (deprecated)</span></span>      |   <span data-ttu-id="6e622-151">Строка</span><span class="sxs-lookup"><span data-stu-id="6e622-151">string</span></span>                  |  <span data-ttu-id="6e622-152">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="6e622-152">Name of the tab.</span></span>     |
|  <span data-ttu-id="6e622-153">teamsAppId (неименовее)</span><span class="sxs-lookup"><span data-stu-id="6e622-153">teamsAppId (deprecated)</span></span>|   <span data-ttu-id="6e622-154">Строка</span><span class="sxs-lookup"><span data-stu-id="6e622-154">string</span></span>             |  <span data-ttu-id="6e622-155">Идентификатор определения приложения для вкладки. Это значение нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="6e622-155">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span> <span data-ttu-id="6e622-156">Так как это свойство является неподготовленным, мы рекомендуем развернуть **teamsApp,** чтобы получить приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="6e622-156">Because this property is deprecated, we recommend expanding **teamsApp** to retrieve the application that is linked to the tab.</span></span> |
|  <span data-ttu-id="6e622-157">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="6e622-157">sortOrderIndex</span></span>  |   <span data-ttu-id="6e622-158">Строка</span><span class="sxs-lookup"><span data-stu-id="6e622-158">string</span></span>                  |  <span data-ttu-id="6e622-159">Индекс порядка, используемого для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="6e622-159">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="6e622-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="6e622-160">webUrl</span></span>          |   <span data-ttu-id="6e622-161">string</span><span class="sxs-lookup"><span data-stu-id="6e622-161">string</span></span>                  |  <span data-ttu-id="6e622-162">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="6e622-162">Deep link URL of the tab instance.</span></span> <span data-ttu-id="6e622-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e622-163">Read only.</span></span>     |
|  <span data-ttu-id="6e622-164">configuration</span><span class="sxs-lookup"><span data-stu-id="6e622-164">configuration</span></span>        |   [<span data-ttu-id="6e622-165">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e622-165">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="6e622-166">Контейнер для настраиваемой настройки, примененной к вкладке. Вкладка считается настроенной только после настройки этого свойства.</span><span class="sxs-lookup"><span data-stu-id="6e622-166">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="6e622-167">Связи</span><span class="sxs-lookup"><span data-stu-id="6e622-167">Relationships</span></span>

| <span data-ttu-id="6e622-168">Связь</span><span class="sxs-lookup"><span data-stu-id="6e622-168">Relationship</span></span> | <span data-ttu-id="6e622-169">Тип</span><span class="sxs-lookup"><span data-stu-id="6e622-169">Type</span></span>   | <span data-ttu-id="6e622-170">Описание</span><span class="sxs-lookup"><span data-stu-id="6e622-170">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6e622-171">teamsApp</span><span class="sxs-lookup"><span data-stu-id="6e622-171">teamsApp</span></span>|[<span data-ttu-id="6e622-172">teamsApp</span><span class="sxs-lookup"><span data-stu-id="6e622-172">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="6e622-173">Приложение, связанное со вкладками.</span><span class="sxs-lookup"><span data-stu-id="6e622-173">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6e622-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e622-174">JSON representation</span></span>

<span data-ttu-id="6e622-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e622-175">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration": "teamsTabConfiguration",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a><span data-ttu-id="6e622-176">См. также</span><span class="sxs-lookup"><span data-stu-id="6e622-176">See also</span></span>

[<span data-ttu-id="6e622-177">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="6e622-177">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


