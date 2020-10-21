---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c60e47a65c9d5b17433891161fe5c16ca182a5ca
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634664"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="90fa6-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="90fa6-103">teamsTab resource type</span></span>

<span data-ttu-id="90fa6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90fa6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90fa6-105">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="90fa6-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="90fa6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="90fa6-106">Methods</span></span>

| <span data-ttu-id="90fa6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="90fa6-107">Method</span></span>       | <span data-ttu-id="90fa6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="90fa6-108">Return Type</span></span>  |<span data-ttu-id="90fa6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="90fa6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90fa6-110">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="90fa6-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="90fa6-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="90fa6-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="90fa6-112">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="90fa6-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="90fa6-113">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="90fa6-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="90fa6-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="90fa6-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="90fa6-115">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="90fa6-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="90fa6-116">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="90fa6-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="90fa6-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="90fa6-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="90fa6-118">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="90fa6-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="90fa6-119">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="90fa6-119">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="90fa6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="90fa6-120">None</span></span> | <span data-ttu-id="90fa6-121">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="90fa6-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="90fa6-122">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="90fa6-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="90fa6-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="90fa6-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="90fa6-124">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="90fa6-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="90fa6-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="90fa6-125">Properties</span></span>

|<span data-ttu-id="90fa6-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="90fa6-126">Property</span></span>|<span data-ttu-id="90fa6-127">Тип</span><span class="sxs-lookup"><span data-stu-id="90fa6-127">Type</span></span>|<span data-ttu-id="90fa6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="90fa6-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="90fa6-129">id</span><span class="sxs-lookup"><span data-stu-id="90fa6-129">id</span></span>              |   <span data-ttu-id="90fa6-130">строка</span><span class="sxs-lookup"><span data-stu-id="90fa6-130">string</span></span>                  |  <span data-ttu-id="90fa6-131">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="90fa6-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="90fa6-132">displayName</span><span class="sxs-lookup"><span data-stu-id="90fa6-132">displayName</span></span>            |   <span data-ttu-id="90fa6-133">string</span><span class="sxs-lookup"><span data-stu-id="90fa6-133">string</span></span>                  |  <span data-ttu-id="90fa6-134">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="90fa6-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="90fa6-135">имя (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="90fa6-135">name (deprecated)</span></span>      |   <span data-ttu-id="90fa6-136">строка</span><span class="sxs-lookup"><span data-stu-id="90fa6-136">string</span></span>                  |  <span data-ttu-id="90fa6-137">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="90fa6-137">Name of the tab.</span></span>     |
|  <span data-ttu-id="90fa6-138">Теамсаппид (устаревший)</span><span class="sxs-lookup"><span data-stu-id="90fa6-138">teamsAppId (deprecated)</span></span>|   <span data-ttu-id="90fa6-139">строка</span><span class="sxs-lookup"><span data-stu-id="90fa6-139">string</span></span>             |  <span data-ttu-id="90fa6-140">Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="90fa6-140">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span> <span data-ttu-id="90fa6-141">Так как это свойство является устаревшим, рекомендуем развернуть **teamsApp** , чтобы получить приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="90fa6-141">Because this property is deprecated, we recommend expanding **teamsApp** to retrieve the application that is linked to the tab.</span></span> |
|  <span data-ttu-id="90fa6-142">сортордериндекс</span><span class="sxs-lookup"><span data-stu-id="90fa6-142">sortOrderIndex</span></span>  |   <span data-ttu-id="90fa6-143">строка</span><span class="sxs-lookup"><span data-stu-id="90fa6-143">string</span></span>                  |  <span data-ttu-id="90fa6-144">Индекс заказа, используемого для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="90fa6-144">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="90fa6-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="90fa6-145">webUrl</span></span>          |   <span data-ttu-id="90fa6-146">string</span><span class="sxs-lookup"><span data-stu-id="90fa6-146">string</span></span>                  |  <span data-ttu-id="90fa6-147">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="90fa6-147">Deep link URL of the tab instance.</span></span> <span data-ttu-id="90fa6-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="90fa6-148">Read only.</span></span>     |
|  <span data-ttu-id="90fa6-149">configuration</span><span class="sxs-lookup"><span data-stu-id="90fa6-149">configuration</span></span>        |   [<span data-ttu-id="90fa6-150">теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="90fa6-150">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="90fa6-151">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="90fa6-151">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="90fa6-152">Связи</span><span class="sxs-lookup"><span data-stu-id="90fa6-152">Relationships</span></span>

| <span data-ttu-id="90fa6-153">Связь</span><span class="sxs-lookup"><span data-stu-id="90fa6-153">Relationship</span></span> | <span data-ttu-id="90fa6-154">Тип</span><span class="sxs-lookup"><span data-stu-id="90fa6-154">Type</span></span>   | <span data-ttu-id="90fa6-155">Описание</span><span class="sxs-lookup"><span data-stu-id="90fa6-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="90fa6-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="90fa6-156">teamsApp</span></span>|[<span data-ttu-id="90fa6-157">teamsApp</span><span class="sxs-lookup"><span data-stu-id="90fa6-157">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="90fa6-158">Приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="90fa6-158">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="90fa6-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="90fa6-159">JSON representation</span></span>

<span data-ttu-id="90fa6-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90fa6-160">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="90fa6-161">См. также</span><span class="sxs-lookup"><span data-stu-id="90fa6-161">See also</span></span>

[<span data-ttu-id="90fa6-162">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="90fa6-162">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)


