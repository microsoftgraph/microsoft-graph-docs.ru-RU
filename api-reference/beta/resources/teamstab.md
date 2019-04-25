---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 207b9d1d4d27199f07ae22bd47587411f917afae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553647"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="ea938-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="ea938-103">teamsTab resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea938-104">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="ea938-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="ea938-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ea938-105">Methods</span></span>

| <span data-ttu-id="ea938-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ea938-106">Method</span></span>       | <span data-ttu-id="ea938-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ea938-107">Return Type</span></span>  |<span data-ttu-id="ea938-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ea938-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea938-109">Список вкладок</span><span class="sxs-lookup"><span data-stu-id="ea938-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="ea938-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ea938-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ea938-111">Список вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="ea938-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="ea938-112">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="ea938-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="ea938-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ea938-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ea938-114">Считывает вкладку, закрепленную в канале.</span><span class="sxs-lookup"><span data-stu-id="ea938-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="ea938-115">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="ea938-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="ea938-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ea938-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ea938-117">Добавляет в канал вкладку (ПИН-код).</span><span class="sxs-lookup"><span data-stu-id="ea938-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="ea938-118">Удалить вкладку</span><span class="sxs-lookup"><span data-stu-id="ea938-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="ea938-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ea938-119">None</span></span> | <span data-ttu-id="ea938-120">Удаляет (открепляет) вкладку из канала.</span><span class="sxs-lookup"><span data-stu-id="ea938-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="ea938-121">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="ea938-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="ea938-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="ea938-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="ea938-123">Обновляет свойства вкладки.</span><span class="sxs-lookup"><span data-stu-id="ea938-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="ea938-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea938-124">Properties</span></span>

|<span data-ttu-id="ea938-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea938-125">Property</span></span>|<span data-ttu-id="ea938-126">Тип</span><span class="sxs-lookup"><span data-stu-id="ea938-126">Type</span></span>|<span data-ttu-id="ea938-127">Описание</span><span class="sxs-lookup"><span data-stu-id="ea938-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="ea938-128">id</span><span class="sxs-lookup"><span data-stu-id="ea938-128">id</span></span>              |   <span data-ttu-id="ea938-129">строка</span><span class="sxs-lookup"><span data-stu-id="ea938-129">string</span></span>                  |  <span data-ttu-id="ea938-130">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="ea938-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="ea938-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ea938-131">displayName</span></span>            |   <span data-ttu-id="ea938-132">string</span><span class="sxs-lookup"><span data-stu-id="ea938-132">string</span></span>                  |  <span data-ttu-id="ea938-133">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="ea938-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="ea938-134">name</span><span class="sxs-lookup"><span data-stu-id="ea938-134">name</span></span>            |   <span data-ttu-id="ea938-135">строка</span><span class="sxs-lookup"><span data-stu-id="ea938-135">string</span></span>                  |  <span data-ttu-id="ea938-136">Устаревшие Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="ea938-136">(Deprecated) Name of the tab.</span></span>     |
|  <span data-ttu-id="ea938-137">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="ea938-137">teamsAppId</span></span>           |   <span data-ttu-id="ea938-138">string</span><span class="sxs-lookup"><span data-stu-id="ea938-138">string</span></span>             |  <span data-ttu-id="ea938-139">Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="ea938-139">App definition identifier of the tab. This value cannot be changed after tab creation.</span></span>     |
|  <span data-ttu-id="ea938-140">Сортордериндекс</span><span class="sxs-lookup"><span data-stu-id="ea938-140">sortOrderIndex</span></span>  |   <span data-ttu-id="ea938-141">string</span><span class="sxs-lookup"><span data-stu-id="ea938-141">string</span></span>                  |  <span data-ttu-id="ea938-142">Индекс заказа, используемого для сортировки вкладок.</span><span class="sxs-lookup"><span data-stu-id="ea938-142">Index of the order used for sorting tabs.</span></span>     |
|  <span data-ttu-id="ea938-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="ea938-143">webUrl</span></span>          |   <span data-ttu-id="ea938-144">string</span><span class="sxs-lookup"><span data-stu-id="ea938-144">string</span></span>                  |  <span data-ttu-id="ea938-145">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="ea938-145">Deep link url of the tab instance.</span></span> <span data-ttu-id="ea938-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea938-146">Read only.</span></span>     |
|  <span data-ttu-id="ea938-147">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="ea938-147">configuration</span></span>        |   [<span data-ttu-id="ea938-148">Теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ea938-148">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="ea938-149">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="ea938-149">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="ea938-150">Связи</span><span class="sxs-lookup"><span data-stu-id="ea938-150">Relationships</span></span>

| <span data-ttu-id="ea938-151">Отношение</span><span class="sxs-lookup"><span data-stu-id="ea938-151">Relationship</span></span> | <span data-ttu-id="ea938-152">Тип</span><span class="sxs-lookup"><span data-stu-id="ea938-152">Type</span></span>   | <span data-ttu-id="ea938-153">Описание</span><span class="sxs-lookup"><span data-stu-id="ea938-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ea938-154">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ea938-154">teamsApp</span></span>|[<span data-ttu-id="ea938-155">teamsApp</span><span class="sxs-lookup"><span data-stu-id="ea938-155">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="ea938-156">Приложение, связанное с вкладкой.</span><span class="sxs-lookup"><span data-stu-id="ea938-156">The application that is linked to the tab.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ea938-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ea938-157">JSON representation</span></span>

<span data-ttu-id="ea938-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea938-158">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="ea938-159">См. также</span><span class="sxs-lookup"><span data-stu-id="ea938-159">See also</span></span>

[<span data-ttu-id="ea938-160">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="ea938-160">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
