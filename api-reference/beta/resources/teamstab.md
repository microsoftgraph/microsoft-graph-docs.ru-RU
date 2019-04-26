---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 6666fbcd69ac46e778ef46380c426c4e94a129fc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345706"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="0be7b-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="0be7b-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0be7b-104">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="0be7b-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="0be7b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="0be7b-105">Methods</span></span>

| <span data-ttu-id="0be7b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="0be7b-106">Method</span></span>       | <span data-ttu-id="0be7b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0be7b-107">Return Type</span></span>  |<span data-ttu-id="0be7b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="0be7b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0be7b-109">Список вкладок</span><span class="sxs-lookup"><span data-stu-id="0be7b-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="0be7b-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0be7b-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0be7b-111">Список вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="0be7b-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="0be7b-112">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="0be7b-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="0be7b-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0be7b-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0be7b-114">Считывает вкладку, закрепленную в канале.</span><span class="sxs-lookup"><span data-stu-id="0be7b-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="0be7b-115">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="0be7b-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="0be7b-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0be7b-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0be7b-117">Добавляет в канал вкладку (ПИН-код).</span><span class="sxs-lookup"><span data-stu-id="0be7b-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="0be7b-118">Удалить вкладку</span><span class="sxs-lookup"><span data-stu-id="0be7b-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="0be7b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0be7b-119">None</span></span> | <span data-ttu-id="0be7b-120">Удаляет (открепляет) вкладку из канала.</span><span class="sxs-lookup"><span data-stu-id="0be7b-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="0be7b-121">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="0be7b-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="0be7b-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="0be7b-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="0be7b-123">Обновляет свойства вкладки.</span><span class="sxs-lookup"><span data-stu-id="0be7b-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="0be7b-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="0be7b-124">Properties</span></span>

|<span data-ttu-id="0be7b-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="0be7b-125">Property</span></span>|<span data-ttu-id="0be7b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="0be7b-126">Type</span></span>|<span data-ttu-id="0be7b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="0be7b-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="0be7b-128">id</span><span class="sxs-lookup"><span data-stu-id="0be7b-128">id</span></span>              |   <span data-ttu-id="0be7b-129">строка</span><span class="sxs-lookup"><span data-stu-id="0be7b-129">string</span></span>                  |  <span data-ttu-id="0be7b-130">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="0be7b-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="0be7b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="0be7b-131">displayName</span></span>            |   <span data-ttu-id="0be7b-132">string</span><span class="sxs-lookup"><span data-stu-id="0be7b-132">string</span></span>                  |  <span data-ttu-id="0be7b-133">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="0be7b-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="0be7b-134">name</span><span class="sxs-lookup"><span data-stu-id="0be7b-134">name</span></span>            |   <span data-ttu-id="0be7b-135">строка</span><span class="sxs-lookup"><span data-stu-id="0be7b-135">string</span></span>                  |  <span data-ttu-id="0be7b-136">Устаревшие Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="0be7b-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="0be7b-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="0be7b-137">teamsAppId</span></span>           |   <span data-ttu-id="0be7b-138">строка</span><span class="sxs-lookup"><span data-stu-id="0be7b-138">string</span></span>             |  <span data-ttu-id="0be7b-139">Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="0be7b-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="0be7b-140">Сортордериндекс</span><span class="sxs-lookup"><span data-stu-id="0be7b-140">sortOrderIndex</span></span>  |   <span data-ttu-id="0be7b-141">строка</span><span class="sxs-lookup"><span data-stu-id="0be7b-141">string</span></span>                  |  <span data-ttu-id="0be7b-142">Индекс заказа, используемого для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="0be7b-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="0be7b-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="0be7b-143">webUrl</span></span>          |   <span data-ttu-id="0be7b-144">string</span><span class="sxs-lookup"><span data-stu-id="0be7b-144">string</span></span>                  |  <span data-ttu-id="0be7b-145">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="0be7b-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="0be7b-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0be7b-146">Read only.</span></span>     |
|  <span data-ttu-id="0be7b-147">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="0be7b-147">configuration</span></span>        |   [<span data-ttu-id="0be7b-148">Теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0be7b-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="0be7b-149">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="0be7b-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="0be7b-150">Связи</span><span class="sxs-lookup"><span data-stu-id="0be7b-150">Relationships</span></span>

| <span data-ttu-id="0be7b-151">Отношение</span><span class="sxs-lookup"><span data-stu-id="0be7b-151">Relationship</span></span> | <span data-ttu-id="0be7b-152">Тип</span><span class="sxs-lookup"><span data-stu-id="0be7b-152">Type</span></span>   | <span data-ttu-id="0be7b-153">Описание</span><span class="sxs-lookup"><span data-stu-id="0be7b-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0be7b-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0be7b-154">teamsApp</span></span>|[<span data-ttu-id="0be7b-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="0be7b-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="0be7b-156">Приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="0be7b-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0be7b-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0be7b-157">JSON representation</span></span>

<span data-ttu-id="0be7b-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0be7b-158">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="0be7b-159">См. также</span><span class="sxs-lookup"><span data-stu-id="0be7b-159">See also</span></span>

[<span data-ttu-id="0be7b-160">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="0be7b-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
