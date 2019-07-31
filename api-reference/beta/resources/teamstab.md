---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 318e3df2d643011537c5d1d9597910fc6b045362
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007650"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="0090a-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="0090a-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0090a-104">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="0090a-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="0090a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="0090a-105">Methods</span></span>

| <span data-ttu-id="0090a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="0090a-106">Method</span></span>       | <span data-ttu-id="0090a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0090a-107">Return Type</span></span>  |<span data-ttu-id="0090a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0090a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0090a-109">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="0090a-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="0090a-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0090a-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0090a-111">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="0090a-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="0090a-112">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="0090a-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="0090a-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0090a-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0090a-114">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="0090a-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="0090a-115">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="0090a-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="0090a-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0090a-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0090a-117">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="0090a-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="0090a-118">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="0090a-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="0090a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0090a-119">None</span></span> | <span data-ttu-id="0090a-120">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="0090a-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="0090a-121">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="0090a-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="0090a-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0090a-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0090a-123">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="0090a-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="0090a-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="0090a-124">Properties</span></span>

|<span data-ttu-id="0090a-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="0090a-125">Property</span></span>|<span data-ttu-id="0090a-126">Тип</span><span class="sxs-lookup"><span data-stu-id="0090a-126">Type</span></span>|<span data-ttu-id="0090a-127">Описание</span><span class="sxs-lookup"><span data-stu-id="0090a-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="0090a-128">id</span><span class="sxs-lookup"><span data-stu-id="0090a-128">id</span></span>              |   <span data-ttu-id="0090a-129">string</span><span class="sxs-lookup"><span data-stu-id="0090a-129">string</span></span>                  |  <span data-ttu-id="0090a-130">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="0090a-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="0090a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0090a-131">displayName</span></span>            |   <span data-ttu-id="0090a-132">string</span><span class="sxs-lookup"><span data-stu-id="0090a-132">string</span></span>                  |  <span data-ttu-id="0090a-133">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="0090a-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="0090a-134">name</span><span class="sxs-lookup"><span data-stu-id="0090a-134">name</span></span>            |   <span data-ttu-id="0090a-135">строка</span><span class="sxs-lookup"><span data-stu-id="0090a-135">string</span></span>                  |  <span data-ttu-id="0090a-136">Устаревшие Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="0090a-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="0090a-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="0090a-137">teamsAppId</span></span>           |   <span data-ttu-id="0090a-138">string</span><span class="sxs-lookup"><span data-stu-id="0090a-138">string</span></span>             |  <span data-ttu-id="0090a-139">Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="0090a-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="0090a-140">Сортордериндекс</span><span class="sxs-lookup"><span data-stu-id="0090a-140">sortOrderIndex</span></span>  |   <span data-ttu-id="0090a-141">string</span><span class="sxs-lookup"><span data-stu-id="0090a-141">string</span></span>                  |  <span data-ttu-id="0090a-142">Индекс заказа, используемого для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="0090a-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="0090a-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="0090a-143">webUrl</span></span>          |   <span data-ttu-id="0090a-144">string</span><span class="sxs-lookup"><span data-stu-id="0090a-144">string</span></span>                  |  <span data-ttu-id="0090a-145">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="0090a-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="0090a-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0090a-146">Read only.</span></span>     |
|  <span data-ttu-id="0090a-147">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="0090a-147">configuration</span></span>        |   [<span data-ttu-id="0090a-148">Теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0090a-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="0090a-149">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="0090a-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="0090a-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="0090a-150">Relationships</span></span>

| <span data-ttu-id="0090a-151">Отношение</span><span class="sxs-lookup"><span data-stu-id="0090a-151">Relationship</span></span> | <span data-ttu-id="0090a-152">Тип</span><span class="sxs-lookup"><span data-stu-id="0090a-152">Type</span></span>   | <span data-ttu-id="0090a-153">Описание</span><span class="sxs-lookup"><span data-stu-id="0090a-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0090a-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0090a-154">teamsApp</span></span>|[<span data-ttu-id="0090a-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0090a-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="0090a-156">Приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="0090a-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0090a-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0090a-157">JSON representation</span></span>

<span data-ttu-id="0090a-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0090a-158">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="0090a-159">См. также</span><span class="sxs-lookup"><span data-stu-id="0090a-159">See also</span></span>

[<span data-ttu-id="0090a-160">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="0090a-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
