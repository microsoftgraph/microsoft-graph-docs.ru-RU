---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa675992401c8953b5611739ba69cb0d5688f833
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606955"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="61d1d-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="61d1d-103">teamsTab resource type</span></span>

<span data-ttu-id="61d1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61d1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61d1d-105">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="61d1d-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="61d1d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="61d1d-106">Methods</span></span>

| <span data-ttu-id="61d1d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="61d1d-107">Method</span></span>       | <span data-ttu-id="61d1d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="61d1d-108">Return Type</span></span>  |<span data-ttu-id="61d1d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="61d1d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="61d1d-110">Вкладки списка в канале</span><span class="sxs-lookup"><span data-stu-id="61d1d-110">List tabs in channel</span></span>](../api/channel-list-tabs.md) | [<span data-ttu-id="61d1d-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="61d1d-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="61d1d-112">Вкладки со списками, закрепленные по каналу.</span><span class="sxs-lookup"><span data-stu-id="61d1d-112">List tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="61d1d-113">Получение вкладки в канале</span><span class="sxs-lookup"><span data-stu-id="61d1d-113">Get tab in channel</span></span>](../api/channel-get-tabs.md) | [<span data-ttu-id="61d1d-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="61d1d-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="61d1d-115">Получение определенной вкладки, закрепленной в канале.</span><span class="sxs-lookup"><span data-stu-id="61d1d-115">Get a specific tab pinned to a channel.</span></span>|
|[<span data-ttu-id="61d1d-116">Добавление вкладки в канал</span><span class="sxs-lookup"><span data-stu-id="61d1d-116">Add tab to channel</span></span>](../api/channel-post-tabs.md) | [<span data-ttu-id="61d1d-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="61d1d-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="61d1d-118">Добавление вкладки к каналу (ПИН-код).</span><span class="sxs-lookup"><span data-stu-id="61d1d-118">Add (pin) a tab to a channel.</span></span>|
|[<span data-ttu-id="61d1d-119">Вкладка "обновление" в канале</span><span class="sxs-lookup"><span data-stu-id="61d1d-119">Update tab in channel</span></span>](../api/channel-patch-tabs.md) | [<span data-ttu-id="61d1d-120">teamsTab</span><span class="sxs-lookup"><span data-stu-id="61d1d-120">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="61d1d-121">Обновляет свойства вкладки в канале.</span><span class="sxs-lookup"><span data-stu-id="61d1d-121">Updates the properties of a tab in a channel.</span></span>|
|[<span data-ttu-id="61d1d-122">Удаление вкладки из канала</span><span class="sxs-lookup"><span data-stu-id="61d1d-122">Remove tab from channel</span></span>](../api/channel-delete-tabs.md) | <span data-ttu-id="61d1d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="61d1d-123">None</span></span> | <span data-ttu-id="61d1d-124">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="61d1d-124">Remove (unpin) a tab from a channel.</span></span>|
|[<span data-ttu-id="61d1d-125">Список вкладок в чате</span><span class="sxs-lookup"><span data-stu-id="61d1d-125">List tabs in chat</span></span>](../api/chat-list-tabs.md) | [<span data-ttu-id="61d1d-126">teamsTab</span><span class="sxs-lookup"><span data-stu-id="61d1d-126">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="61d1d-127">Список вкладок, закрепленных в чате.</span><span class="sxs-lookup"><span data-stu-id="61d1d-127">List tabs pinned to a chat.</span></span>|
|[<span data-ttu-id="61d1d-128">Получение вкладки в чате</span><span class="sxs-lookup"><span data-stu-id="61d1d-128">Get tab in chat</span></span>](../api/chat-get-tabs.md) | [<span data-ttu-id="61d1d-129">teamsTab</span><span class="sxs-lookup"><span data-stu-id="61d1d-129">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="61d1d-130">Получение определенной вкладки, закрепленной в чате.</span><span class="sxs-lookup"><span data-stu-id="61d1d-130">Get a specific tab pinned to a chat.</span></span>|
|[<span data-ttu-id="61d1d-131">Добавление вкладки в чат</span><span class="sxs-lookup"><span data-stu-id="61d1d-131">Add tab to chat</span></span>](../api/chat-post-tabs.md) | [<span data-ttu-id="61d1d-132">teamsTab</span><span class="sxs-lookup"><span data-stu-id="61d1d-132">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="61d1d-133">Добавление вкладки в чат (ПИН-код).</span><span class="sxs-lookup"><span data-stu-id="61d1d-133">Add (pin) a tab to a chat.</span></span>|
|[<span data-ttu-id="61d1d-134">Вкладка "обновление" в чате</span><span class="sxs-lookup"><span data-stu-id="61d1d-134">Update tab in chat</span></span>](../api/chat-patch-tabs.md) | [<span data-ttu-id="61d1d-135">teamsTab</span><span class="sxs-lookup"><span data-stu-id="61d1d-135">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="61d1d-136">Обновляет свойства вкладки в чате.</span><span class="sxs-lookup"><span data-stu-id="61d1d-136">Updates the properties of a tab in a chat.</span></span>|
|[<span data-ttu-id="61d1d-137">Удаление вкладки из чата</span><span class="sxs-lookup"><span data-stu-id="61d1d-137">Remove tab from chat</span></span>](../api/chat-delete-tabs.md) | <span data-ttu-id="61d1d-138">Нет</span><span class="sxs-lookup"><span data-stu-id="61d1d-138">None</span></span> | <span data-ttu-id="61d1d-139">Удаление (открепление) вкладки из чата.</span><span class="sxs-lookup"><span data-stu-id="61d1d-139">Remove (unpin) a tab from a chat.</span></span>|



## <a name="properties"></a><span data-ttu-id="61d1d-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="61d1d-140">Properties</span></span>

|<span data-ttu-id="61d1d-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="61d1d-141">Property</span></span>|<span data-ttu-id="61d1d-142">Тип</span><span class="sxs-lookup"><span data-stu-id="61d1d-142">Type</span></span>|<span data-ttu-id="61d1d-143">Описание</span><span class="sxs-lookup"><span data-stu-id="61d1d-143">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="61d1d-144">id</span><span class="sxs-lookup"><span data-stu-id="61d1d-144">id</span></span>              |   <span data-ttu-id="61d1d-145">string</span><span class="sxs-lookup"><span data-stu-id="61d1d-145">string</span></span>                  |  <span data-ttu-id="61d1d-146">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="61d1d-146">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="61d1d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="61d1d-147">displayName</span></span>            |   <span data-ttu-id="61d1d-148">string</span><span class="sxs-lookup"><span data-stu-id="61d1d-148">string</span></span>                  |  <span data-ttu-id="61d1d-149">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="61d1d-149">Name of the tab.</span></span>     |
|  <span data-ttu-id="61d1d-150">имя (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="61d1d-150">name (deprecated)</span></span>      |   <span data-ttu-id="61d1d-151">string</span><span class="sxs-lookup"><span data-stu-id="61d1d-151">string</span></span>                  |  <span data-ttu-id="61d1d-152">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="61d1d-152">Name of the tab.</span></span>     |
|  <span data-ttu-id="61d1d-153">Теамсаппид (устаревший)</span><span class="sxs-lookup"><span data-stu-id="61d1d-153">teamsAppId (deprecated)</span></span>|   <span data-ttu-id="61d1d-154">string</span><span class="sxs-lookup"><span data-stu-id="61d1d-154">string</span></span>             |  <span data-ttu-id="61d1d-155">Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="61d1d-155">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span> <span data-ttu-id="61d1d-156">Так как это свойство является устаревшим, рекомендуем развернуть **teamsApp** , чтобы получить приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="61d1d-156">Because this property is deprecated, we recommend expanding **teamsApp** to retrieve the application that is linked to the tab.</span></span> |
|  <span data-ttu-id="61d1d-157">сортордериндекс</span><span class="sxs-lookup"><span data-stu-id="61d1d-157">sortOrderIndex</span></span>  |   <span data-ttu-id="61d1d-158">string</span><span class="sxs-lookup"><span data-stu-id="61d1d-158">string</span></span>                  |  <span data-ttu-id="61d1d-159">Индекс заказа, используемого для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="61d1d-159">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="61d1d-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="61d1d-160">webUrl</span></span>          |   <span data-ttu-id="61d1d-161">string</span><span class="sxs-lookup"><span data-stu-id="61d1d-161">string</span></span>                  |  <span data-ttu-id="61d1d-162">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="61d1d-162">Deep link URL of the tab instance.</span></span> <span data-ttu-id="61d1d-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="61d1d-163">Read only.</span></span>     |
|  <span data-ttu-id="61d1d-164">configuration</span><span class="sxs-lookup"><span data-stu-id="61d1d-164">configuration</span></span>        |   [<span data-ttu-id="61d1d-165">теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="61d1d-165">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="61d1d-166">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="61d1d-166">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="61d1d-167">Связи</span><span class="sxs-lookup"><span data-stu-id="61d1d-167">Relationships</span></span>

| <span data-ttu-id="61d1d-168">Связь</span><span class="sxs-lookup"><span data-stu-id="61d1d-168">Relationship</span></span> | <span data-ttu-id="61d1d-169">Тип</span><span class="sxs-lookup"><span data-stu-id="61d1d-169">Type</span></span>   | <span data-ttu-id="61d1d-170">Описание</span><span class="sxs-lookup"><span data-stu-id="61d1d-170">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="61d1d-171">teamsApp</span><span class="sxs-lookup"><span data-stu-id="61d1d-171">teamsApp</span></span>|[<span data-ttu-id="61d1d-172">teamsApp</span><span class="sxs-lookup"><span data-stu-id="61d1d-172">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="61d1d-173">Приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="61d1d-173">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61d1d-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61d1d-174">JSON representation</span></span>

<span data-ttu-id="61d1d-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61d1d-175">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="61d1d-176">См. также</span><span class="sxs-lookup"><span data-stu-id="61d1d-176">See also</span></span>

[<span data-ttu-id="61d1d-177">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="61d1d-177">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


