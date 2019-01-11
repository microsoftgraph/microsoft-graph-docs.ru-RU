---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая прикрепленных (вложенный) канала в группе. '
localization_priority: Normal
ms.openlocfilehash: a1c3302251ac9b68be1cd8d6a011b7e0a7d216b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860846"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="4945b-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="4945b-103">teamsTab resource type</span></span>



<span data-ttu-id="4945b-104">TeamsTab — [вкладку](../resources/teamstab.md) , которая прикрепленных (вложенный) [канала](channel.md) в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="4945b-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="4945b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4945b-105">Methods</span></span>

| <span data-ttu-id="4945b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="4945b-106">Method</span></span>       | <span data-ttu-id="4945b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4945b-107">Return Type</span></span>  |<span data-ttu-id="4945b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4945b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4945b-109">Список вкладок</span><span class="sxs-lookup"><span data-stu-id="4945b-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="4945b-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4945b-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4945b-111">Списки вкладок прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="4945b-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="4945b-112">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="4945b-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="4945b-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4945b-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4945b-114">Считывает вкладки, прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="4945b-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="4945b-115">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="4945b-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="4945b-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4945b-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4945b-117">Добавляет (PIN) вкладки на канал.</span><span class="sxs-lookup"><span data-stu-id="4945b-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="4945b-118">Удалить вкладку ""</span><span class="sxs-lookup"><span data-stu-id="4945b-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="4945b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="4945b-119">None</span></span> | <span data-ttu-id="4945b-120">Удаляет (отключит) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="4945b-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="4945b-121">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="4945b-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="4945b-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4945b-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="4945b-123">Обновляет свойства вкладки.</span><span class="sxs-lookup"><span data-stu-id="4945b-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="4945b-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="4945b-124">Properties</span></span>

|<span data-ttu-id="4945b-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="4945b-125">Property</span></span>|<span data-ttu-id="4945b-126">Тип</span><span class="sxs-lookup"><span data-stu-id="4945b-126">Type</span></span>|<span data-ttu-id="4945b-127">Описание</span><span class="sxs-lookup"><span data-stu-id="4945b-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="4945b-128">id</span><span class="sxs-lookup"><span data-stu-id="4945b-128">id</span></span>              |   <span data-ttu-id="4945b-129">строка</span><span class="sxs-lookup"><span data-stu-id="4945b-129">string</span></span>                  |  <span data-ttu-id="4945b-130">Идентификатор, который уникальным образом определяет определенный экземпляр канала вкладку чтения только.</span><span class="sxs-lookup"><span data-stu-id="4945b-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="4945b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="4945b-131">displayName</span></span>            |   <span data-ttu-id="4945b-132">строка</span><span class="sxs-lookup"><span data-stu-id="4945b-132">string</span></span>                  |  <span data-ttu-id="4945b-133">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="4945b-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="4945b-134">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="4945b-134">sortOrderIndex</span></span>  |   <span data-ttu-id="4945b-135">int</span><span class="sxs-lookup"><span data-stu-id="4945b-135">int</span></span>                     |  <span data-ttu-id="4945b-136">Индекс порядок, используемый для сортировки вкладок</span><span class="sxs-lookup"><span data-stu-id="4945b-136">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="4945b-137">webUrl</span><span class="sxs-lookup"><span data-stu-id="4945b-137">webUrl</span></span>          |   <span data-ttu-id="4945b-138">string</span><span class="sxs-lookup"><span data-stu-id="4945b-138">string</span></span>                  |  <span data-ttu-id="4945b-139">Прямая ссылка URL-адрес экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="4945b-139">Deep link url of the tab instance.</span></span> <span data-ttu-id="4945b-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4945b-140">Read only.</span></span>     |
|  <span data-ttu-id="4945b-141">configuration</span><span class="sxs-lookup"><span data-stu-id="4945b-141">configuration</span></span>        |   [<span data-ttu-id="4945b-142">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="4945b-142">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="4945b-143">Контейнер для пользовательских параметров, применяемых на вкладке. Вкладка считается настроены только после этого свойства.</span><span class="sxs-lookup"><span data-stu-id="4945b-143">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="4945b-144">Связи</span><span class="sxs-lookup"><span data-stu-id="4945b-144">Relationships</span></span>

| <span data-ttu-id="4945b-145">Связь</span><span class="sxs-lookup"><span data-stu-id="4945b-145">Relationship</span></span> | <span data-ttu-id="4945b-146">Тип</span><span class="sxs-lookup"><span data-stu-id="4945b-146">Type</span></span>   | <span data-ttu-id="4945b-147">Описание</span><span class="sxs-lookup"><span data-stu-id="4945b-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4945b-148">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4945b-148">teamsApp</span></span>|[<span data-ttu-id="4945b-149">teamsApp</span><span class="sxs-lookup"><span data-stu-id="4945b-149">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="4945b-150">Приложения, связанного с вкладки. Это нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="4945b-150">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4945b-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4945b-151">JSON representation</span></span>

<span data-ttu-id="4945b-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4945b-152">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
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

## <a name="see-also"></a><span data-ttu-id="4945b-153">См. также</span><span class="sxs-lookup"><span data-stu-id="4945b-153">See also</span></span>

[<span data-ttu-id="4945b-154">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="4945b-154">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
