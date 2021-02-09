---
title: Тип ресурса onPremisesAgent
description: Тип ресурса onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 59ee11bb952c85695b8c20daa1e040c8899740b9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158354"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="c67d3-103">Тип ресурса onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="c67d3-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="c67d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c67d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c67d3-105">Представляет локального агента.</span><span class="sxs-lookup"><span data-stu-id="c67d3-105">Represents on-premises agent.</span></span> <span data-ttu-id="c67d3-106">Для локального агента, установленного администратором клиента, можно настроить доступ и обработку запросов к определенному [опубликованного ресурса.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="c67d3-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c67d3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c67d3-107">Methods</span></span>

| <span data-ttu-id="c67d3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c67d3-108">Method</span></span>       | <span data-ttu-id="c67d3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c67d3-109">Return Type</span></span> | <span data-ttu-id="c67d3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c67d3-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c67d3-111">Список onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="c67d3-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="c67d3-112">[Коллекция onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="c67d3-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="c67d3-113">Получите **коллекцию объектов onPremisesAgents.**</span><span class="sxs-lookup"><span data-stu-id="c67d3-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="c67d3-114">Get onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="c67d3-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="c67d3-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="c67d3-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="c67d3-116">Чтение свойств и связей объекта **onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="c67d3-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="c67d3-117">Назначение onPremisesAgent onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="c67d3-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="c67d3-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c67d3-118">None</span></span> | <span data-ttu-id="c67d3-119">**Назначьте onPremisesAgent** для **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="c67d3-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="c67d3-120">Удаление onpremisesAgent из onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="c67d3-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="c67d3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c67d3-121">None</span></span> | <span data-ttu-id="c67d3-122">Удалите **onPremisesAgent** из **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="c67d3-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="c67d3-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="c67d3-123">Properties</span></span>

| <span data-ttu-id="c67d3-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="c67d3-124">Property</span></span>     | <span data-ttu-id="c67d3-125">Тип</span><span class="sxs-lookup"><span data-stu-id="c67d3-125">Type</span></span>        | <span data-ttu-id="c67d3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c67d3-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c67d3-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="c67d3-127">externalIp</span></span>|<span data-ttu-id="c67d3-128">String</span><span class="sxs-lookup"><span data-stu-id="c67d3-128">String</span></span>|<span data-ttu-id="c67d3-129">Внешний IP-адрес, обнаруженный службой для компьютера агента.</span><span class="sxs-lookup"><span data-stu-id="c67d3-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="c67d3-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c67d3-130">Read-only</span></span>|
|<span data-ttu-id="c67d3-131">id</span><span class="sxs-lookup"><span data-stu-id="c67d3-131">id</span></span>|<span data-ttu-id="c67d3-132">String</span><span class="sxs-lookup"><span data-stu-id="c67d3-132">String</span></span>| <span data-ttu-id="c67d3-133">ИД объекта onPremisesAgent.</span><span class="sxs-lookup"><span data-stu-id="c67d3-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="c67d3-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c67d3-134">Read-only.</span></span>|
|<span data-ttu-id="c67d3-135">machineName</span><span class="sxs-lookup"><span data-stu-id="c67d3-135">machineName</span></span>|<span data-ttu-id="c67d3-136">String</span><span class="sxs-lookup"><span data-stu-id="c67d3-136">String</span></span>|<span data-ttu-id="c67d3-137">Имя компьютера, на которого работает aggent.</span><span class="sxs-lookup"><span data-stu-id="c67d3-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="c67d3-138">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c67d3-138">Read-only</span></span>|
|<span data-ttu-id="c67d3-139">status</span><span class="sxs-lookup"><span data-stu-id="c67d3-139">status</span></span>|<span data-ttu-id="c67d3-140">string</span><span class="sxs-lookup"><span data-stu-id="c67d3-140">string</span></span>| <span data-ttu-id="c67d3-141">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="c67d3-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="c67d3-142">publishingType</span><span class="sxs-lookup"><span data-stu-id="c67d3-142">publishingType</span></span>|<span data-ttu-id="c67d3-143">string</span><span class="sxs-lookup"><span data-stu-id="c67d3-143">string</span></span>| <span data-ttu-id="c67d3-144">Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="c67d3-144">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c67d3-145">Связи</span><span class="sxs-lookup"><span data-stu-id="c67d3-145">Relationships</span></span>

| <span data-ttu-id="c67d3-146">Связь</span><span class="sxs-lookup"><span data-stu-id="c67d3-146">Relationship</span></span> | <span data-ttu-id="c67d3-147">Тип</span><span class="sxs-lookup"><span data-stu-id="c67d3-147">Type</span></span>        | <span data-ttu-id="c67d3-148">Описание</span><span class="sxs-lookup"><span data-stu-id="c67d3-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c67d3-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="c67d3-149">agentGroups</span></span>|<span data-ttu-id="c67d3-150">[Коллекция onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="c67d3-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="c67d3-151">Список **onPremisesAgentGroups,** которые **назначены onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="c67d3-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="c67d3-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c67d3-152">Read-only.</span></span> <span data-ttu-id="c67d3-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c67d3-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c67d3-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c67d3-154">JSON representation</span></span>

<span data-ttu-id="c67d3-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c67d3-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "keyProperty": "id"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string",
  "supportedPublishingTypes": ["string"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



