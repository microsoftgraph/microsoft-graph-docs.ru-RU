---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая прикрепленных (вложенный) канала в группе. '
ms.openlocfilehash: 4e9773fa2e4ea6a114c1f2695906c09d84b3f043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026288"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="01b63-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="01b63-103">teamsTab resource type</span></span>



<span data-ttu-id="01b63-104">TeamsTab — [вкладку](../resources/teamstab.md) , которая прикрепленных (вложенный) [канала](channel.md) в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="01b63-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="01b63-105">Методы</span><span class="sxs-lookup"><span data-stu-id="01b63-105">Methods</span></span>

| <span data-ttu-id="01b63-106">Метод</span><span class="sxs-lookup"><span data-stu-id="01b63-106">Method</span></span>       | <span data-ttu-id="01b63-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="01b63-107">Return Type</span></span>  |<span data-ttu-id="01b63-108">Описание</span><span class="sxs-lookup"><span data-stu-id="01b63-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="01b63-109">Список вкладок</span><span class="sxs-lookup"><span data-stu-id="01b63-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="01b63-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="01b63-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="01b63-111">Списки вкладок прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="01b63-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="01b63-112">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="01b63-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="01b63-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="01b63-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="01b63-114">Считывает вкладки, прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="01b63-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="01b63-115">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="01b63-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="01b63-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="01b63-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="01b63-117">Добавляет (PIN) вкладки на канал.</span><span class="sxs-lookup"><span data-stu-id="01b63-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="01b63-118">Удалить вкладку ""</span><span class="sxs-lookup"><span data-stu-id="01b63-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="01b63-119">Нет</span><span class="sxs-lookup"><span data-stu-id="01b63-119">None</span></span> | <span data-ttu-id="01b63-120">Удаляет (отключит) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="01b63-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="01b63-121">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="01b63-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="01b63-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="01b63-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="01b63-123">Обновляет свойства вкладки.</span><span class="sxs-lookup"><span data-stu-id="01b63-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="01b63-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="01b63-124">Properties</span></span>

|<span data-ttu-id="01b63-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="01b63-125">Property</span></span>|<span data-ttu-id="01b63-126">Тип</span><span class="sxs-lookup"><span data-stu-id="01b63-126">Type</span></span>|<span data-ttu-id="01b63-127">Описание</span><span class="sxs-lookup"><span data-stu-id="01b63-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="01b63-128">id</span><span class="sxs-lookup"><span data-stu-id="01b63-128">id</span></span>              |   <span data-ttu-id="01b63-129">строка</span><span class="sxs-lookup"><span data-stu-id="01b63-129">string</span></span>                  |  <span data-ttu-id="01b63-130">Идентификатор, который уникальным образом определяет определенный экземпляр канала вкладку чтения только.</span><span class="sxs-lookup"><span data-stu-id="01b63-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="01b63-131">displayName</span><span class="sxs-lookup"><span data-stu-id="01b63-131">displayName</span></span>            |   <span data-ttu-id="01b63-132">строка</span><span class="sxs-lookup"><span data-stu-id="01b63-132">string</span></span>                  |  <span data-ttu-id="01b63-133">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="01b63-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="01b63-134">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="01b63-134">sortOrderIndex</span></span>  |   <span data-ttu-id="01b63-135">целое</span><span class="sxs-lookup"><span data-stu-id="01b63-135">int</span></span>                     |  <span data-ttu-id="01b63-136">Индекс порядок, используемый для сортировки вкладок</span><span class="sxs-lookup"><span data-stu-id="01b63-136">Index of the order used for sorting tabs</span></span>     |
|  <span data-ttu-id="01b63-137">webUrl</span><span class="sxs-lookup"><span data-stu-id="01b63-137">webUrl</span></span>          |   <span data-ttu-id="01b63-138">string</span><span class="sxs-lookup"><span data-stu-id="01b63-138">string</span></span>                  |  <span data-ttu-id="01b63-139">Прямая ссылка URL-адрес экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="01b63-139">Deep link url of the tab instance.</span></span> <span data-ttu-id="01b63-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="01b63-140">Read only.</span></span>     |
|  <span data-ttu-id="01b63-141">configuration</span><span class="sxs-lookup"><span data-stu-id="01b63-141">configuration</span></span>        |   [<span data-ttu-id="01b63-142">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="01b63-142">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="01b63-143">Контейнер для пользовательских параметров, применяемых на вкладке. Вкладка считается настроены только после этого свойства.</span><span class="sxs-lookup"><span data-stu-id="01b63-143">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="01b63-144">Связи</span><span class="sxs-lookup"><span data-stu-id="01b63-144">Relationships</span></span>

| <span data-ttu-id="01b63-145">Связь</span><span class="sxs-lookup"><span data-stu-id="01b63-145">Relationship</span></span> | <span data-ttu-id="01b63-146">Тип</span><span class="sxs-lookup"><span data-stu-id="01b63-146">Type</span></span>   | <span data-ttu-id="01b63-147">Description</span><span class="sxs-lookup"><span data-stu-id="01b63-147">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="01b63-148">teamsApp</span><span class="sxs-lookup"><span data-stu-id="01b63-148">teamsApp</span></span>|[<span data-ttu-id="01b63-149">teamsApp</span><span class="sxs-lookup"><span data-stu-id="01b63-149">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="01b63-150">Приложения, связанного с вкладки. Это нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="01b63-150">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="01b63-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01b63-151">JSON representation</span></span>

<span data-ttu-id="01b63-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01b63-152">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="01b63-153">См. также</span><span class="sxs-lookup"><span data-stu-id="01b63-153">See also</span></span>

[<span data-ttu-id="01b63-154">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="01b63-154">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
