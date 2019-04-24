---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 181d2fd23ff922709b3e098f6069adf300ad3928
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456985"
---
# <a name="teamstab-resource-type"></a><span data-ttu-id="deb7e-103">Тип ресурса teamsTab</span><span class="sxs-lookup"><span data-stu-id="deb7e-103">teamsTab resource type</span></span>



<span data-ttu-id="deb7e-104">TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md).</span><span class="sxs-lookup"><span data-stu-id="deb7e-104">A teamsTab is a [tab](../resources/teamstab.md) that's pinned (attached) to a [channel](channel.md) within a [team](team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="deb7e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="deb7e-105">Methods</span></span>

| <span data-ttu-id="deb7e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="deb7e-106">Method</span></span>       | <span data-ttu-id="deb7e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="deb7e-107">Return Type</span></span>  |<span data-ttu-id="deb7e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="deb7e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="deb7e-109">Список вкладок</span><span class="sxs-lookup"><span data-stu-id="deb7e-109">List tabs</span></span>](../api/teamstab-list.md) | [<span data-ttu-id="deb7e-110">teamsTab</span><span class="sxs-lookup"><span data-stu-id="deb7e-110">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="deb7e-111">Список вкладок, закрепленных в канале.</span><span class="sxs-lookup"><span data-stu-id="deb7e-111">Lists tabs pinned to a channel.</span></span>|
|[<span data-ttu-id="deb7e-112">Получение вкладки</span><span class="sxs-lookup"><span data-stu-id="deb7e-112">Get tab</span></span>](../api/teamstab-get.md) | [<span data-ttu-id="deb7e-113">teamsTab</span><span class="sxs-lookup"><span data-stu-id="deb7e-113">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="deb7e-114">Считывает вкладку, закрепленную в канале.</span><span class="sxs-lookup"><span data-stu-id="deb7e-114">Reads a tab pinned to a channel.</span></span>|
|[<span data-ttu-id="deb7e-115">Добавление вкладки</span><span class="sxs-lookup"><span data-stu-id="deb7e-115">Add tab</span></span>](../api/teamstab-add.md) | [<span data-ttu-id="deb7e-116">teamsTab</span><span class="sxs-lookup"><span data-stu-id="deb7e-116">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="deb7e-117">Добавляет в канал вкладку (ПИН-код).</span><span class="sxs-lookup"><span data-stu-id="deb7e-117">Adds (pins) a tab to a channel.</span></span>|
|[<span data-ttu-id="deb7e-118">Удалить вкладку</span><span class="sxs-lookup"><span data-stu-id="deb7e-118">Remove tab</span></span>](../api/teamstab-delete.md) | <span data-ttu-id="deb7e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="deb7e-119">None</span></span> | <span data-ttu-id="deb7e-120">Удаляет (открепляет) вкладку из канала.</span><span class="sxs-lookup"><span data-stu-id="deb7e-120">Removes (unpins) a tab from a channel.</span></span>|
|[<span data-ttu-id="deb7e-121">Обновление вкладки</span><span class="sxs-lookup"><span data-stu-id="deb7e-121">Update tab</span></span>](../api/teamstab-update.md) | [<span data-ttu-id="deb7e-122">teamsTab</span><span class="sxs-lookup"><span data-stu-id="deb7e-122">teamsTab</span></span>](teamstab.md) | <span data-ttu-id="deb7e-123">Обновляет свойства вкладки.</span><span class="sxs-lookup"><span data-stu-id="deb7e-123">Updates the tab properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="deb7e-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="deb7e-124">Properties</span></span>

|<span data-ttu-id="deb7e-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="deb7e-125">Property</span></span>|<span data-ttu-id="deb7e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="deb7e-126">Type</span></span>|<span data-ttu-id="deb7e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="deb7e-127">Description</span></span>|
|:---------------|:--------|:----------|
|  <span data-ttu-id="deb7e-128">id</span><span class="sxs-lookup"><span data-stu-id="deb7e-128">id</span></span>              |   <span data-ttu-id="deb7e-129">строка</span><span class="sxs-lookup"><span data-stu-id="deb7e-129">string</span></span>                  |  <span data-ttu-id="deb7e-130">Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.</span><span class="sxs-lookup"><span data-stu-id="deb7e-130">Identifier that uniquely identifies a specific instance of a channel tab. Read only.</span></span>     |
|  <span data-ttu-id="deb7e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="deb7e-131">displayName</span></span>            |   <span data-ttu-id="deb7e-132">string</span><span class="sxs-lookup"><span data-stu-id="deb7e-132">string</span></span>                  |  <span data-ttu-id="deb7e-133">Имя вкладки.</span><span class="sxs-lookup"><span data-stu-id="deb7e-133">Name of the tab.</span></span>     |
|  <span data-ttu-id="deb7e-134">webUrl</span><span class="sxs-lookup"><span data-stu-id="deb7e-134">webUrl</span></span>          |   <span data-ttu-id="deb7e-135">string</span><span class="sxs-lookup"><span data-stu-id="deb7e-135">string</span></span>                  |  <span data-ttu-id="deb7e-136">URL-адрес глубокой ссылки для экземпляра вкладки.</span><span class="sxs-lookup"><span data-stu-id="deb7e-136">Deep link url of the tab instance.</span></span> <span data-ttu-id="deb7e-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="deb7e-137">Read only.</span></span>     |
|  <span data-ttu-id="deb7e-138">конфигурацион</span><span class="sxs-lookup"><span data-stu-id="deb7e-138">configuration</span></span>        |   [<span data-ttu-id="deb7e-139">Теамстабконфигуратион</span><span class="sxs-lookup"><span data-stu-id="deb7e-139">teamsTabConfiguration</span></span>](teamstabconfiguration.md) |  <span data-ttu-id="deb7e-140">Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.</span><span class="sxs-lookup"><span data-stu-id="deb7e-140">Container for custom settings applied to a tab. The tab is considered configured only once this property is set.</span></span>     |

## <a name="relationships"></a><span data-ttu-id="deb7e-141">Связи</span><span class="sxs-lookup"><span data-stu-id="deb7e-141">Relationships</span></span>

| <span data-ttu-id="deb7e-142">Отношение</span><span class="sxs-lookup"><span data-stu-id="deb7e-142">Relationship</span></span> | <span data-ttu-id="deb7e-143">Тип</span><span class="sxs-lookup"><span data-stu-id="deb7e-143">Type</span></span>   | <span data-ttu-id="deb7e-144">Описание</span><span class="sxs-lookup"><span data-stu-id="deb7e-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="deb7e-145">teamsApp</span><span class="sxs-lookup"><span data-stu-id="deb7e-145">teamsApp</span></span>|[<span data-ttu-id="deb7e-146">teamsApp</span><span class="sxs-lookup"><span data-stu-id="deb7e-146">teamsApp</span></span>](teamsapp.md) | <span data-ttu-id="deb7e-147">Приложение, связанное с вкладкой. Его нельзя изменить после создания вкладки.</span><span class="sxs-lookup"><span data-stu-id="deb7e-147">The application that is linked to the tab. This cannot be changed after tab creation.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="deb7e-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="deb7e-148">JSON representation</span></span>

<span data-ttu-id="deb7e-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="deb7e-149">The following is a JSON representation of the resource.</span></span>


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

## <a name="see-also"></a><span data-ttu-id="deb7e-150">См. также</span><span class="sxs-lookup"><span data-stu-id="deb7e-150">See also</span></span>

[<span data-ttu-id="deb7e-151">Настройка встроенных типов вкладок</span><span class="sxs-lookup"><span data-stu-id="deb7e-151">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)
