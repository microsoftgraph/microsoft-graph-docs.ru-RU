---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая прикрепленных (вложенный) канала в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 3c5cf5ef33f53cfaca7189df24e5dfd880a77241
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947150"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="35361-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="35361-103">teamsTab resource type</span></span>

> <span data-ttu-id="35361-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35361-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35361-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35361-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35361-106">TeamsTab — [вкладку](../resources/teamstab.md) , которая прикрепленных (вложенный) [канала](channel.md) в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="35361-106">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="35361-107">Методы</span><span class="sxs-lookup"><span data-stu-id="35361-107">Methods</span></span>

| <span data-ttu-id="35361-108">Метод</span><span class="sxs-lookup"><span data-stu-id="35361-108">Method</span></span>       | <span data-ttu-id="35361-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35361-109">Return Type</span></span>  |<span data-ttu-id="35361-110">Описание</span><span class="sxs-lookup"><span data-stu-id="35361-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35361-111">Список вкладок</span><span class="sxs-lookup"><span data-stu-id="35361-111">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="35361-112">teamsTab</span><span class="sxs-lookup"><span data-stu-id="35361-112">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="35361-113">Списки вкладок прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="35361-113">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="35361-114">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="35361-114">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="35361-115">teamsTab</span><span class="sxs-lookup"><span data-stu-id="35361-115">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="35361-116">Считывает вкладки, прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="35361-116">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="35361-117">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="35361-117">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="35361-118">teamsTab</span><span class="sxs-lookup"><span data-stu-id="35361-118">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="35361-119">Добавляет (PIN) вкладки на канал.</span><span class="sxs-lookup"><span data-stu-id="35361-119">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="35361-120">Удалить вкладку ""</span><span class="sxs-lookup"><span data-stu-id="35361-120">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="35361-121">Нет</span><span class="sxs-lookup"><span data-stu-id="35361-121">None</span></span> | <span data-ttu-id="35361-122">Удаляет (отключит) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="35361-122">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="35361-123">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="35361-123">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="35361-124">teamsTab</span><span class="sxs-lookup"><span data-stu-id="35361-124">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="35361-125">Обновляет свойства вкладки.</span><span class="sxs-lookup"><span data-stu-id="35361-125">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="35361-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="35361-126">Properties</span></span>

|<span data-ttu-id="35361-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="35361-127">Property</span></span>|<span data-ttu-id="35361-128">Тип</span><span class="sxs-lookup"><span data-stu-id="35361-128">Type</span></span>|<span data-ttu-id="35361-129">Описание</span><span class="sxs-lookup"><span data-stu-id="35361-129">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="35361-130">id</span><span class="sxs-lookup"><span data-stu-id="35361-130">id</span></span>              |   <span data-ttu-id="35361-131">строка</span><span class="sxs-lookup"><span data-stu-id="35361-131">string</span></span>                  |  <span data-ttu-id="35361-132">Идентификатор, который уникальным образом определяет определенный экземпляр канала вкладку чтения только.</span><span class="sxs-lookup"><span data-stu-id="35361-132">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="35361-133">displayName</span><span class="sxs-lookup"><span data-stu-id="35361-133">displayName</span></span>            |   <span data-ttu-id="35361-134">строка</span><span class="sxs-lookup"><span data-stu-id="35361-134">string</span></span>                  |  <span data-ttu-id="35361-135">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="35361-135">Name of the tab.</span></span>     |
|  <span data-ttu-id="35361-136">name</span><span class="sxs-lookup"><span data-stu-id="35361-136">name</span></span>            |   <span data-ttu-id="35361-137">строка</span><span class="sxs-lookup"><span data-stu-id="35361-137">string</span></span>                  |  <span data-ttu-id="35361-138">(Устарело) Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="35361-138">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="35361-139">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="35361-139">teamsAppId</span></span>           |   <span data-ttu-id="35361-140">строка</span><span class="sxs-lookup"><span data-stu-id="35361-140">string</span></span>             |  <span data-ttu-id="35361-141">Идентификатор приложения определения вкладки. После создания вкладки не может изменить это значение.</span><span class="sxs-lookup"><span data-stu-id="35361-141">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="35361-142">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="35361-142">sortOrderIndex</span></span>  |   <span data-ttu-id="35361-143">int</span><span class="sxs-lookup"><span data-stu-id="35361-143">int</span></span>                     |  <span data-ttu-id="35361-144">Индекс порядок, используемый для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="35361-144">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="35361-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="35361-145">webUrl</span></span>          |   <span data-ttu-id="35361-146">строка</span><span class="sxs-lookup"><span data-stu-id="35361-146">string</span></span>                  |  <span data-ttu-id="35361-147">Прямая ссылка URL-адрес экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="35361-147">Deep link url of the tab instance.</span></span> <span data-ttu-id="35361-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35361-148">Read only.</span></span>     |
|  <span data-ttu-id="35361-149">configuration</span><span class="sxs-lookup"><span data-stu-id="35361-149">configuration</span></span>        |   [<span data-ttu-id="35361-150">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="35361-150">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="35361-151">Контейнер для пользовательских параметров, применяемых на вкладке. Вкладка считается настроены только после этого свойства.</span><span class="sxs-lookup"><span data-stu-id="35361-151">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="35361-152">Связи</span><span class="sxs-lookup"><span data-stu-id="35361-152">Relationships</span></span>

| <span data-ttu-id="35361-153">Связь</span><span class="sxs-lookup"><span data-stu-id="35361-153">Relationship</span></span> | <span data-ttu-id="35361-154">Тип</span><span class="sxs-lookup"><span data-stu-id="35361-154">Type</span></span>   | <span data-ttu-id="35361-155">Описание</span><span class="sxs-lookup"><span data-stu-id="35361-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="35361-156">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35361-156">teamsApp</span></span>|[<span data-ttu-id="35361-157">teamsApp</span><span class="sxs-lookup"><span data-stu-id="35361-157">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="35361-158">Приложения, связанного с вкладки.</span><span class="sxs-lookup"><span data-stu-id="35361-158">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35361-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35361-159">JSON representation</span></span>

<span data-ttu-id="35361-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35361-160">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="35361-161">См. также</span><span class="sxs-lookup"><span data-stu-id="35361-161">See also</span></span>

[<span data-ttu-id="35361-162">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="35361-162">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
