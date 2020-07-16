---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c5d73738a24e0ffd21b259c58ce44cbe000c54df
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909732"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="dc5f8-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="dc5f8-103">teamsTab resource type</span></span>

<span data-ttu-id="dc5f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc5f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc5f8-105">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="dc5f8-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="dc5f8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="dc5f8-106">Methods</span></span>

| <span data-ttu-id="dc5f8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="dc5f8-107">Method</span></span>       | <span data-ttu-id="dc5f8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dc5f8-108">Return Type</span></span>  |<span data-ttu-id="dc5f8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="dc5f8-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc5f8-110">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="dc5f8-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="dc5f8-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dc5f8-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="dc5f8-112">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="dc5f8-113">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="dc5f8-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="dc5f8-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dc5f8-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="dc5f8-115">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="dc5f8-116">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="dc5f8-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="dc5f8-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dc5f8-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="dc5f8-118">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="dc5f8-119">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="dc5f8-119">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="dc5f8-120">Нет</span><span class="sxs-lookup"><span data-stu-id="dc5f8-120">None</span></span> | <span data-ttu-id="dc5f8-121">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="dc5f8-122">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="dc5f8-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="dc5f8-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="dc5f8-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="dc5f8-124">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="dc5f8-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc5f8-125">Properties</span></span>

|<span data-ttu-id="dc5f8-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc5f8-126">Property</span></span>|<span data-ttu-id="dc5f8-127">Тип</span><span class="sxs-lookup"><span data-stu-id="dc5f8-127">Type</span></span>|<span data-ttu-id="dc5f8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="dc5f8-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="dc5f8-129">id</span><span class="sxs-lookup"><span data-stu-id="dc5f8-129">id</span></span>              |   <span data-ttu-id="dc5f8-130">строка</span><span class="sxs-lookup"><span data-stu-id="dc5f8-130">string</span></span>                  |  <span data-ttu-id="dc5f8-131">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="dc5f8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="dc5f8-132">displayName</span></span>            |   <span data-ttu-id="dc5f8-133">string</span><span class="sxs-lookup"><span data-stu-id="dc5f8-133">string</span></span>                  |  <span data-ttu-id="dc5f8-134">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="dc5f8-135">name</span><span class="sxs-lookup"><span data-stu-id="dc5f8-135">name</span></span>            |   <span data-ttu-id="dc5f8-136">string</span><span class="sxs-lookup"><span data-stu-id="dc5f8-136">string</span></span>                  |  <span data-ttu-id="dc5f8-137">Устаревшие Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-137">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="dc5f8-138">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="dc5f8-138">teamsAppId</span></span>           |   <span data-ttu-id="dc5f8-139">string</span><span class="sxs-lookup"><span data-stu-id="dc5f8-139">string</span></span>             |  <span data-ttu-id="dc5f8-140">Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-140">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="dc5f8-141">сортордериндекс</span><span class="sxs-lookup"><span data-stu-id="dc5f8-141">sortOrderIndex</span></span>  |   <span data-ttu-id="dc5f8-142">string</span><span class="sxs-lookup"><span data-stu-id="dc5f8-142">string</span></span>                  |  <span data-ttu-id="dc5f8-143">Индекс заказа, используемого для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-143">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="dc5f8-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="dc5f8-144">webUrl</span></span>          |   <span data-ttu-id="dc5f8-145">string</span><span class="sxs-lookup"><span data-stu-id="dc5f8-145">string</span></span>                  |  <span data-ttu-id="dc5f8-146">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-146">Deep link URL of the tab instance.</span></span> <span data-ttu-id="dc5f8-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-147">Read only.</span></span>     |
|  <span data-ttu-id="dc5f8-148">configuration</span><span class="sxs-lookup"><span data-stu-id="dc5f8-148">configuration</span></span>        |   [<span data-ttu-id="dc5f8-149">теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="dc5f8-149">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="dc5f8-150">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-150">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="dc5f8-151">Связи</span><span class="sxs-lookup"><span data-stu-id="dc5f8-151">Relationships</span></span>

| <span data-ttu-id="dc5f8-152">Связь</span><span class="sxs-lookup"><span data-stu-id="dc5f8-152">Relationship</span></span> | <span data-ttu-id="dc5f8-153">Тип</span><span class="sxs-lookup"><span data-stu-id="dc5f8-153">Type</span></span>   | <span data-ttu-id="dc5f8-154">Описание</span><span class="sxs-lookup"><span data-stu-id="dc5f8-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dc5f8-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="dc5f8-155">teamsApp</span></span>|[<span data-ttu-id="dc5f8-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="dc5f8-156">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="dc5f8-157">Приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-157">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dc5f8-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dc5f8-158">JSON representation</span></span>

<span data-ttu-id="dc5f8-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc5f8-159">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="dc5f8-160">См. также</span><span class="sxs-lookup"><span data-stu-id="dc5f8-160">See also</span></span>

[<span data-ttu-id="dc5f8-161">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="dc5f8-161">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
