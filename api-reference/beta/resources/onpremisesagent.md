---
title: Тип ресурса onPremisesAgent
description: Тип ресурса onPremisesAgent.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 8269c2d2273df385c4815e2276f320a7e4f5b813
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135886"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="3cbfe-103">Тип ресурса onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="3cbfe-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="3cbfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cbfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cbfe-105">Представляет локального агента.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-105">Represents on-premises agent.</span></span> <span data-ttu-id="3cbfe-106">Для локального агента, установленного администратором клиента, можно настроить доступ и обработку запросов к определенному [опубликованного ресурса.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="3cbfe-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3cbfe-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3cbfe-107">Methods</span></span>

| <span data-ttu-id="3cbfe-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3cbfe-108">Method</span></span>       | <span data-ttu-id="3cbfe-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3cbfe-109">Return Type</span></span> | <span data-ttu-id="3cbfe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3cbfe-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3cbfe-111">Список onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="3cbfe-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="3cbfe-112">[Коллекция onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="3cbfe-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="3cbfe-113">Получите **коллекцию объектов onPremisesAgents.**</span><span class="sxs-lookup"><span data-stu-id="3cbfe-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="3cbfe-114">Get onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="3cbfe-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="3cbfe-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="3cbfe-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="3cbfe-116">Чтение свойств и связей объекта **onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="3cbfe-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="3cbfe-117">Назначение onPremisesAgent для onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3cbfe-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="3cbfe-118">Нет</span><span class="sxs-lookup"><span data-stu-id="3cbfe-118">None</span></span> | <span data-ttu-id="3cbfe-119">**Назначьте onPremisesAgent** для **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="3cbfe-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="3cbfe-120">Удаление onpremisesAgent из onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="3cbfe-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="3cbfe-121">Нет</span><span class="sxs-lookup"><span data-stu-id="3cbfe-121">None</span></span> | <span data-ttu-id="3cbfe-122">Удалите **onPremisesAgent** из **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="3cbfe-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="3cbfe-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="3cbfe-123">Properties</span></span>

| <span data-ttu-id="3cbfe-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="3cbfe-124">Property</span></span>     | <span data-ttu-id="3cbfe-125">Тип</span><span class="sxs-lookup"><span data-stu-id="3cbfe-125">Type</span></span>        | <span data-ttu-id="3cbfe-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3cbfe-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3cbfe-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="3cbfe-127">externalIp</span></span>|<span data-ttu-id="3cbfe-128">Строка</span><span class="sxs-lookup"><span data-stu-id="3cbfe-128">String</span></span>|<span data-ttu-id="3cbfe-129">Внешний IP-адрес, обнаруженный службой для компьютера агента.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="3cbfe-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="3cbfe-130">Read-only</span></span>|
|<span data-ttu-id="3cbfe-131">id</span><span class="sxs-lookup"><span data-stu-id="3cbfe-131">id</span></span>|<span data-ttu-id="3cbfe-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3cbfe-132">String</span></span>| <span data-ttu-id="3cbfe-133">ИД объекта onPremisesAgent.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="3cbfe-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-134">Read-only.</span></span>|
|<span data-ttu-id="3cbfe-135">machineName</span><span class="sxs-lookup"><span data-stu-id="3cbfe-135">machineName</span></span>|<span data-ttu-id="3cbfe-136">Строка</span><span class="sxs-lookup"><span data-stu-id="3cbfe-136">String</span></span>|<span data-ttu-id="3cbfe-137">Имя компьютера, на которого работает aggent.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="3cbfe-138">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="3cbfe-138">Read-only</span></span>|
|<span data-ttu-id="3cbfe-139">status</span><span class="sxs-lookup"><span data-stu-id="3cbfe-139">status</span></span>|<span data-ttu-id="3cbfe-140">string</span><span class="sxs-lookup"><span data-stu-id="3cbfe-140">string</span></span>| <span data-ttu-id="3cbfe-141">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="3cbfe-142">publishingType</span><span class="sxs-lookup"><span data-stu-id="3cbfe-142">publishingType</span></span>|<span data-ttu-id="3cbfe-143">string</span><span class="sxs-lookup"><span data-stu-id="3cbfe-143">string</span></span>| <span data-ttu-id="3cbfe-144">Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-144">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cbfe-145">Связи</span><span class="sxs-lookup"><span data-stu-id="3cbfe-145">Relationships</span></span>

| <span data-ttu-id="3cbfe-146">Связь</span><span class="sxs-lookup"><span data-stu-id="3cbfe-146">Relationship</span></span> | <span data-ttu-id="3cbfe-147">Тип</span><span class="sxs-lookup"><span data-stu-id="3cbfe-147">Type</span></span>        | <span data-ttu-id="3cbfe-148">Описание</span><span class="sxs-lookup"><span data-stu-id="3cbfe-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3cbfe-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="3cbfe-149">agentGroups</span></span>|<span data-ttu-id="3cbfe-150">[Коллекция onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="3cbfe-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="3cbfe-151">Список **onPremisesAgentGroups,** которые **назначены onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="3cbfe-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="3cbfe-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-152">Read-only.</span></span> <span data-ttu-id="3cbfe-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3cbfe-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3cbfe-154">JSON representation</span></span>

<span data-ttu-id="3cbfe-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3cbfe-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesAgent",
  "baseType": "",
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



