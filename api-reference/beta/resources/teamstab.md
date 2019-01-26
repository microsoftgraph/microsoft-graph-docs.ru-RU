---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая прикрепленных (вложенный) канала в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 207b9d1d4d27199f07ae22bd47587411f917afae
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574952"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="ac6f1-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="ac6f1-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac6f1-104">TeamsTab — [вкладку](../resources/teamstab.md) , которая прикрепленных (вложенный) [канала](channel.md) в [группы](team.md).</span><span class="sxs-lookup"><span data-stu-id="ac6f1-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="ac6f1-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ac6f1-105">Methods</span></span>

| <span data-ttu-id="ac6f1-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ac6f1-106">Method</span></span>       | <span data-ttu-id="ac6f1-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ac6f1-107">Return Type</span></span>  |<span data-ttu-id="ac6f1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6f1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ac6f1-109">Список вкладок</span><span class="sxs-lookup"><span data-stu-id="ac6f1-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="ac6f1-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ac6f1-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ac6f1-111">Списки вкладок прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="ac6f1-112">Получить вкладки</span><span class="sxs-lookup"><span data-stu-id="ac6f1-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="ac6f1-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ac6f1-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ac6f1-114">Считывает вкладки, прикрепленных к каналу.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="ac6f1-115">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="ac6f1-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="ac6f1-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ac6f1-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ac6f1-117">Добавляет (PIN) вкладки на канал.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="ac6f1-118">Удалить вкладку ""</span><span class="sxs-lookup"><span data-stu-id="ac6f1-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="ac6f1-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ac6f1-119">None</span></span> | <span data-ttu-id="ac6f1-120">Удаляет (отключит) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="ac6f1-121">Вкладка "обновления"</span><span class="sxs-lookup"><span data-stu-id="ac6f1-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="ac6f1-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ac6f1-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ac6f1-123">Обновляет свойства вкладки.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="ac6f1-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac6f1-124">Properties</span></span>

|<span data-ttu-id="ac6f1-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac6f1-125">Property</span></span>|<span data-ttu-id="ac6f1-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ac6f1-126">Type</span></span>|<span data-ttu-id="ac6f1-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6f1-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="ac6f1-128">id</span><span class="sxs-lookup"><span data-stu-id="ac6f1-128">id</span></span>              |   <span data-ttu-id="ac6f1-129">string</span><span class="sxs-lookup"><span data-stu-id="ac6f1-129">string</span></span>                  |  <span data-ttu-id="ac6f1-130">Идентификатор, который уникальным образом определяет определенный экземпляр канала вкладку чтения только.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="ac6f1-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ac6f1-131">displayName</span></span>            |   <span data-ttu-id="ac6f1-132">string</span><span class="sxs-lookup"><span data-stu-id="ac6f1-132">string</span></span>                  |  <span data-ttu-id="ac6f1-133">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="ac6f1-134">name</span><span class="sxs-lookup"><span data-stu-id="ac6f1-134">name</span></span>            |   <span data-ttu-id="ac6f1-135">строка</span><span class="sxs-lookup"><span data-stu-id="ac6f1-135">string</span></span>                  |  <span data-ttu-id="ac6f1-136">(Устарело) Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="ac6f1-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ac6f1-137">teamsAppId</span></span>           |   <span data-ttu-id="ac6f1-138">string</span><span class="sxs-lookup"><span data-stu-id="ac6f1-138">string</span></span>             |  <span data-ttu-id="ac6f1-139">Идентификатор приложения определения вкладки. После создания вкладки не может изменить это значение.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="ac6f1-140">sortOrderIndex</span><span class="sxs-lookup"><span data-stu-id="ac6f1-140">sortOrderIndex</span></span>  |   <span data-ttu-id="ac6f1-141">string</span><span class="sxs-lookup"><span data-stu-id="ac6f1-141">string</span></span>                  |  <span data-ttu-id="ac6f1-142">Индекс порядок, используемый для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="ac6f1-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="ac6f1-143">webUrl</span></span>          |   <span data-ttu-id="ac6f1-144">string</span><span class="sxs-lookup"><span data-stu-id="ac6f1-144">string</span></span>                  |  <span data-ttu-id="ac6f1-145">Прямая ссылка URL-адрес экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="ac6f1-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-146">Read only.</span></span>     |
|  <span data-ttu-id="ac6f1-147">configuration</span><span class="sxs-lookup"><span data-stu-id="ac6f1-147">configuration</span></span>        |   [<span data-ttu-id="ac6f1-148">teamsTabConfiguration</span><span class="sxs-lookup"><span data-stu-id="ac6f1-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="ac6f1-149">Контейнер для пользовательских параметров, применяемых на вкладке. Вкладка считается настроены только после этого свойства.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="ac6f1-150">Связи</span><span class="sxs-lookup"><span data-stu-id="ac6f1-150">Relationships</span></span>

| <span data-ttu-id="ac6f1-151">Связь</span><span class="sxs-lookup"><span data-stu-id="ac6f1-151">Relationship</span></span> | <span data-ttu-id="ac6f1-152">Тип</span><span class="sxs-lookup"><span data-stu-id="ac6f1-152">Type</span></span>   | <span data-ttu-id="ac6f1-153">Описание</span><span class="sxs-lookup"><span data-stu-id="ac6f1-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ac6f1-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ac6f1-154">teamsApp</span></span>|[<span data-ttu-id="ac6f1-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ac6f1-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="ac6f1-156">Приложения, связанного с вкладки.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ac6f1-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac6f1-157">JSON representation</span></span>

<span data-ttu-id="ac6f1-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac6f1-158">The following is a JSON representation of the resource.</span></span>


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
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstab.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="ac6f1-159">См. также</span><span class="sxs-lookup"><span data-stu-id="ac6f1-159">See also</span></span>

[<span data-ttu-id="ac6f1-160">Настройка типов встроенную вкладку</span><span class="sxs-lookup"><span data-stu-id="ac6f1-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
