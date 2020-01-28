---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d4b8bf73499bc2cca2a7497e57e3cce6c8cbe5b9
ms.sourcegitcommit: 0f39f39a1c0300ef013ebd12e4df2b5ba4dabbf8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2020
ms.locfileid: "41559042"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="ba5ff-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="ba5ff-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba5ff-104">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="ba5ff-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="ba5ff-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ba5ff-105">Methods</span></span>

| <span data-ttu-id="ba5ff-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ba5ff-106">Method</span></span>       | <span data-ttu-id="ba5ff-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ba5ff-107">Return Type</span></span>  |<span data-ttu-id="ba5ff-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5ff-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ba5ff-109">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="ba5ff-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="ba5ff-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ba5ff-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ba5ff-111">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="ba5ff-112">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="ba5ff-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="ba5ff-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ba5ff-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ba5ff-114">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="ba5ff-115">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="ba5ff-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="ba5ff-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ba5ff-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ba5ff-117">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="ba5ff-118">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="ba5ff-118">Delete tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="ba5ff-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ba5ff-119">None</span></span> | <span data-ttu-id="ba5ff-120">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="ba5ff-121">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="ba5ff-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="ba5ff-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ba5ff-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ba5ff-123">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="ba5ff-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="ba5ff-124">Properties</span></span>

|<span data-ttu-id="ba5ff-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba5ff-125">Property</span></span>|<span data-ttu-id="ba5ff-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ba5ff-126">Type</span></span>|<span data-ttu-id="ba5ff-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5ff-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="ba5ff-128">id</span><span class="sxs-lookup"><span data-stu-id="ba5ff-128">id</span></span>              |   <span data-ttu-id="ba5ff-129">строка</span><span class="sxs-lookup"><span data-stu-id="ba5ff-129">string</span></span>                  |  <span data-ttu-id="ba5ff-130">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="ba5ff-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ba5ff-131">displayName</span></span>            |   <span data-ttu-id="ba5ff-132">string</span><span class="sxs-lookup"><span data-stu-id="ba5ff-132">string</span></span>                  |  <span data-ttu-id="ba5ff-133">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="ba5ff-134">name</span><span class="sxs-lookup"><span data-stu-id="ba5ff-134">name</span></span>            |   <span data-ttu-id="ba5ff-135">string</span><span class="sxs-lookup"><span data-stu-id="ba5ff-135">string</span></span>                  |  <span data-ttu-id="ba5ff-136">Устаревшие Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="ba5ff-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ba5ff-137">teamsAppId</span></span>           |   <span data-ttu-id="ba5ff-138">string</span><span class="sxs-lookup"><span data-stu-id="ba5ff-138">string</span></span>             |  <span data-ttu-id="ba5ff-139">Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="ba5ff-140">сортордериндекс</span><span class="sxs-lookup"><span data-stu-id="ba5ff-140">sortOrderIndex</span></span>  |   <span data-ttu-id="ba5ff-141">string</span><span class="sxs-lookup"><span data-stu-id="ba5ff-141">string</span></span>                  |  <span data-ttu-id="ba5ff-142">Индекс заказа, используемого для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="ba5ff-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="ba5ff-143">webUrl</span></span>          |   <span data-ttu-id="ba5ff-144">string</span><span class="sxs-lookup"><span data-stu-id="ba5ff-144">string</span></span>                  |  <span data-ttu-id="ba5ff-145">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="ba5ff-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-146">Read only.</span></span>     |
|  <span data-ttu-id="ba5ff-147">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="ba5ff-147">configuration</span></span>        |   [<span data-ttu-id="ba5ff-148">теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ba5ff-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="ba5ff-149">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="ba5ff-150">Связи</span><span class="sxs-lookup"><span data-stu-id="ba5ff-150">Relationships</span></span>

| <span data-ttu-id="ba5ff-151">Связь</span><span class="sxs-lookup"><span data-stu-id="ba5ff-151">Relationship</span></span> | <span data-ttu-id="ba5ff-152">Тип</span><span class="sxs-lookup"><span data-stu-id="ba5ff-152">Type</span></span>   | <span data-ttu-id="ba5ff-153">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5ff-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ba5ff-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ba5ff-154">teamsApp</span></span>|[<span data-ttu-id="ba5ff-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ba5ff-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="ba5ff-156">Приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba5ff-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ba5ff-157">JSON representation</span></span>

<span data-ttu-id="ba5ff-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba5ff-158">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="ba5ff-159">См. также</span><span class="sxs-lookup"><span data-stu-id="ba5ff-159">See also</span></span>

[<span data-ttu-id="ba5ff-160">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="ba5ff-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
