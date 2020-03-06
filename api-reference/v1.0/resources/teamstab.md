---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c62905699b8986d9594ccad06d154d93b71313fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533475"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="cf27d-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="cf27d-103">teamsTab resource type</span></span>

<span data-ttu-id="cf27d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf27d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="cf27d-105">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="cf27d-105">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="cf27d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cf27d-106">Methods</span></span>

| <span data-ttu-id="cf27d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cf27d-107">Method</span></span>       | <span data-ttu-id="cf27d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cf27d-108">Return Type</span></span>  |<span data-ttu-id="cf27d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cf27d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf27d-110">Перечисление вкладок</span><span class="sxs-lookup"><span data-stu-id="cf27d-110">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="cf27d-111">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cf27d-111">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cf27d-112">Перечисление вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="cf27d-112">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="cf27d-113">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="cf27d-113">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="cf27d-114">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cf27d-114">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cf27d-115">Чтение вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="cf27d-115">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="cf27d-116">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="cf27d-116">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="cf27d-117">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cf27d-117">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cf27d-118">Добавление (закрепление) вкладки в канал.</span><span class="sxs-lookup"><span data-stu-id="cf27d-118">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="cf27d-119">Удаление вкладки</span><span class="sxs-lookup"><span data-stu-id="cf27d-119">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="cf27d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="cf27d-120">None</span></span> | <span data-ttu-id="cf27d-121">Удаление (открепление) вкладки из канала.</span><span class="sxs-lookup"><span data-stu-id="cf27d-121">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="cf27d-122">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="cf27d-122">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="cf27d-123">teamsTab</span><span class="sxs-lookup"><span data-stu-id="cf27d-123">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="cf27d-124">Обновление свойств вкладки.</span><span class="sxs-lookup"><span data-stu-id="cf27d-124">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="cf27d-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf27d-125">Properties</span></span>

|<span data-ttu-id="cf27d-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf27d-126">Property</span></span>|<span data-ttu-id="cf27d-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cf27d-127">Type</span></span>|<span data-ttu-id="cf27d-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cf27d-128">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="cf27d-129">id</span><span class="sxs-lookup"><span data-stu-id="cf27d-129">id</span></span>              |   <span data-ttu-id="cf27d-130">string</span><span class="sxs-lookup"><span data-stu-id="cf27d-130">string</span></span>                  |  <span data-ttu-id="cf27d-131">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="cf27d-131">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="cf27d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="cf27d-132">displayName</span></span>            |   <span data-ttu-id="cf27d-133">string</span><span class="sxs-lookup"><span data-stu-id="cf27d-133">string</span></span>                  |  <span data-ttu-id="cf27d-134">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="cf27d-134">Name of the tab.</span></span>     |
|  <span data-ttu-id="cf27d-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="cf27d-135">webUrl</span></span>          |   <span data-ttu-id="cf27d-136">string</span><span class="sxs-lookup"><span data-stu-id="cf27d-136">string</span></span>                  |  <span data-ttu-id="cf27d-137">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="cf27d-137">Deep link url of the tab instance.</span></span> <span data-ttu-id="cf27d-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cf27d-138">Read only.</span></span>     |
|  <span data-ttu-id="cf27d-139">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="cf27d-139">configuration</span></span>        |   [<span data-ttu-id="cf27d-140">теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="cf27d-140">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="cf27d-141">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="cf27d-141">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="cf27d-142">Связи</span><span class="sxs-lookup"><span data-stu-id="cf27d-142">Relationships</span></span>

| <span data-ttu-id="cf27d-143">Связь</span><span class="sxs-lookup"><span data-stu-id="cf27d-143">Relationship</span></span> | <span data-ttu-id="cf27d-144">Тип</span><span class="sxs-lookup"><span data-stu-id="cf27d-144">Type</span></span>   | <span data-ttu-id="cf27d-145">Описание</span><span class="sxs-lookup"><span data-stu-id="cf27d-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cf27d-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cf27d-146">teamsApp</span></span>|[<span data-ttu-id="cf27d-147">teamsApp</span><span class="sxs-lookup"><span data-stu-id="cf27d-147">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="cf27d-148">Приложение, связанное с вкладкой. Его нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="cf27d-148">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cf27d-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf27d-149">JSON representation</span></span>

<span data-ttu-id="cf27d-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf27d-150">The following is a JSON representation of the resource.</span></span>


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{  
  "id": "string",
  "displayName": "string",
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

## <a name="see-also"></a><span data-ttu-id="cf27d-151">См. также</span><span class="sxs-lookup"><span data-stu-id="cf27d-151">See also</span></span>

[<span data-ttu-id="cf27d-152">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="cf27d-152">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
