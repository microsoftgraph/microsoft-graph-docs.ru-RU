---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 74dfe42bc48757ffe8799a033dfebf2df61f913d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519850"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="ad8c7-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="ad8c7-103">teamsTab resource type</span></span>

<span data-ttu-id="ad8c7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ad8c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad8c7-105">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="ad8c7-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="ad8c7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ad8c7-106">Methods</span></span>

| <span data-ttu-id="ad8c7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ad8c7-107">Method</span></span>       | <span data-ttu-id="ad8c7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ad8c7-108">Return Type</span></span>  |<span data-ttu-id="ad8c7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ad8c7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad8c7-110">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="ad8c7-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="ad8c7-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ad8c7-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ad8c7-112">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="ad8c7-113">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="ad8c7-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="ad8c7-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ad8c7-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ad8c7-115">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="ad8c7-116">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="ad8c7-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="ad8c7-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ad8c7-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ad8c7-118">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="ad8c7-119">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="ad8c7-119">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="ad8c7-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ad8c7-120">None</span></span> | <span data-ttu-id="ad8c7-121">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="ad8c7-122">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="ad8c7-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="ad8c7-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ad8c7-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ad8c7-124">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="ad8c7-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad8c7-125">Properties</span></span>

|<span data-ttu-id="ad8c7-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad8c7-126">Property</span></span>|<span data-ttu-id="ad8c7-127">Тип</span><span class="sxs-lookup"><span data-stu-id="ad8c7-127">Type</span></span>|<span data-ttu-id="ad8c7-128">Описание</span><span class="sxs-lookup"><span data-stu-id="ad8c7-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="ad8c7-129">id</span><span class="sxs-lookup"><span data-stu-id="ad8c7-129">id</span></span>              |   <span data-ttu-id="ad8c7-130">строка</span><span class="sxs-lookup"><span data-stu-id="ad8c7-130">string</span></span>                  |  <span data-ttu-id="ad8c7-131">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="ad8c7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ad8c7-132">displayName</span></span>            |   <span data-ttu-id="ad8c7-133">string</span><span class="sxs-lookup"><span data-stu-id="ad8c7-133">string</span></span>                  |  <span data-ttu-id="ad8c7-134">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="ad8c7-135">name</span><span class="sxs-lookup"><span data-stu-id="ad8c7-135">name</span></span>            |   <span data-ttu-id="ad8c7-136">string</span><span class="sxs-lookup"><span data-stu-id="ad8c7-136">string</span></span>                  |  <span data-ttu-id="ad8c7-137">Устаревшие Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-137">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="ad8c7-138">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ad8c7-138">teamsAppId</span></span>           |   <span data-ttu-id="ad8c7-139">строка</span><span class="sxs-lookup"><span data-stu-id="ad8c7-139">string</span></span>             |  <span data-ttu-id="ad8c7-140">Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-140">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="ad8c7-141">сортордериндекс</span><span class="sxs-lookup"><span data-stu-id="ad8c7-141">sortOrderIndex</span></span>  |   <span data-ttu-id="ad8c7-142">строка</span><span class="sxs-lookup"><span data-stu-id="ad8c7-142">string</span></span>                  |  <span data-ttu-id="ad8c7-143">Индекс заказа, используемого для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-143">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="ad8c7-144">webUrl</span><span class="sxs-lookup"><span data-stu-id="ad8c7-144">webUrl</span></span>          |   <span data-ttu-id="ad8c7-145">string</span><span class="sxs-lookup"><span data-stu-id="ad8c7-145">string</span></span>                  |  <span data-ttu-id="ad8c7-146">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-146">Deep link url of the tab instance.</span></span> <span data-ttu-id="ad8c7-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-147">Read only.</span></span>     |
|  <span data-ttu-id="ad8c7-148">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="ad8c7-148">configuration</span></span>        |   [<span data-ttu-id="ad8c7-149">теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ad8c7-149">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="ad8c7-150">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-150">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="ad8c7-151">Связи</span><span class="sxs-lookup"><span data-stu-id="ad8c7-151">Relationships</span></span>

| <span data-ttu-id="ad8c7-152">Связь</span><span class="sxs-lookup"><span data-stu-id="ad8c7-152">Relationship</span></span> | <span data-ttu-id="ad8c7-153">Тип</span><span class="sxs-lookup"><span data-stu-id="ad8c7-153">Type</span></span>   | <span data-ttu-id="ad8c7-154">Описание</span><span class="sxs-lookup"><span data-stu-id="ad8c7-154">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ad8c7-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ad8c7-155">teamsApp</span></span>|[<span data-ttu-id="ad8c7-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ad8c7-156">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="ad8c7-157">Приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-157">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ad8c7-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad8c7-158">JSON representation</span></span>

<span data-ttu-id="ad8c7-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad8c7-159">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="ad8c7-160">См. также</span><span class="sxs-lookup"><span data-stu-id="ad8c7-160">See also</span></span>

[<span data-ttu-id="ad8c7-161">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="ad8c7-161">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
