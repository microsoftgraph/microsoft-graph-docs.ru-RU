---
title: onPremisesAgent type
description: onPremisesAgent типа ресурса.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 74128ab48e023f066f259fea5f326d5e1642eb14
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956934"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="645dd-103">onPremisesAgent type</span><span class="sxs-lookup"><span data-stu-id="645dd-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="645dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="645dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="645dd-105">Представляет локального агента.</span><span class="sxs-lookup"><span data-stu-id="645dd-105">Represents on-premises agent.</span></span> <span data-ttu-id="645dd-106">Агенты локального использования, установленные администратором клиента, могут быть настроены для доступа и обработки запросов к определенному [опубликованому ресурсу.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="645dd-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="645dd-107">Методы</span><span class="sxs-lookup"><span data-stu-id="645dd-107">Methods</span></span>

| <span data-ttu-id="645dd-108">Метод</span><span class="sxs-lookup"><span data-stu-id="645dd-108">Method</span></span>       | <span data-ttu-id="645dd-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="645dd-109">Return Type</span></span> | <span data-ttu-id="645dd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="645dd-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="645dd-111">Список onPremisesAgents</span><span class="sxs-lookup"><span data-stu-id="645dd-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="645dd-112">[коллекция onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="645dd-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="645dd-113">Получите **коллекцию объектов onPremisesAgents.**</span><span class="sxs-lookup"><span data-stu-id="645dd-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="645dd-114">Get onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="645dd-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="645dd-115">onPremisesAgent</span><span class="sxs-lookup"><span data-stu-id="645dd-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="645dd-116">Ознакомьтесь с свойствами и отношениями **объекта onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="645dd-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="645dd-117">Назначение onPremisesAgent onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="645dd-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="645dd-118">Нет</span><span class="sxs-lookup"><span data-stu-id="645dd-118">None</span></span> | <span data-ttu-id="645dd-119">Назначение **onPremisesAgent** для **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="645dd-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="645dd-120">Удаление onpremisesAgent из onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="645dd-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="645dd-121">Нет</span><span class="sxs-lookup"><span data-stu-id="645dd-121">None</span></span> | <span data-ttu-id="645dd-122">Удалите **onPremisesAgent** из **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="645dd-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="645dd-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="645dd-123">Properties</span></span>

| <span data-ttu-id="645dd-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="645dd-124">Property</span></span>     | <span data-ttu-id="645dd-125">Тип</span><span class="sxs-lookup"><span data-stu-id="645dd-125">Type</span></span>        | <span data-ttu-id="645dd-126">Описание</span><span class="sxs-lookup"><span data-stu-id="645dd-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="645dd-127">externalIp</span><span class="sxs-lookup"><span data-stu-id="645dd-127">externalIp</span></span>|<span data-ttu-id="645dd-128">Строка</span><span class="sxs-lookup"><span data-stu-id="645dd-128">String</span></span>|<span data-ttu-id="645dd-129">Внешний IP-адрес, обнаруженный службой для машины агента.</span><span class="sxs-lookup"><span data-stu-id="645dd-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="645dd-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="645dd-130">Read-only</span></span>|
|<span data-ttu-id="645dd-131">id</span><span class="sxs-lookup"><span data-stu-id="645dd-131">id</span></span>|<span data-ttu-id="645dd-132">Строка</span><span class="sxs-lookup"><span data-stu-id="645dd-132">String</span></span>| <span data-ttu-id="645dd-133">ID объекта onPremisesAgent.</span><span class="sxs-lookup"><span data-stu-id="645dd-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="645dd-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="645dd-134">Read-only.</span></span>|
|<span data-ttu-id="645dd-135">machineName</span><span class="sxs-lookup"><span data-stu-id="645dd-135">machineName</span></span>|<span data-ttu-id="645dd-136">Строка</span><span class="sxs-lookup"><span data-stu-id="645dd-136">String</span></span>|<span data-ttu-id="645dd-137">Имя машины, на которую работает aggent.</span><span class="sxs-lookup"><span data-stu-id="645dd-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="645dd-138">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="645dd-138">Read-only</span></span>|
|<span data-ttu-id="645dd-139">status</span><span class="sxs-lookup"><span data-stu-id="645dd-139">status</span></span>|<span data-ttu-id="645dd-140">agentStatus</span><span class="sxs-lookup"><span data-stu-id="645dd-140">agentStatus</span></span>| <span data-ttu-id="645dd-141">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="645dd-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="645dd-142">publishingType</span><span class="sxs-lookup"><span data-stu-id="645dd-142">publishingType</span></span>|<span data-ttu-id="645dd-143">Строка</span><span class="sxs-lookup"><span data-stu-id="645dd-143">String</span></span>| <span data-ttu-id="645dd-144">Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="645dd-144">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="645dd-145">Связи</span><span class="sxs-lookup"><span data-stu-id="645dd-145">Relationships</span></span>

| <span data-ttu-id="645dd-146">Связь</span><span class="sxs-lookup"><span data-stu-id="645dd-146">Relationship</span></span> | <span data-ttu-id="645dd-147">Тип</span><span class="sxs-lookup"><span data-stu-id="645dd-147">Type</span></span>        | <span data-ttu-id="645dd-148">Описание</span><span class="sxs-lookup"><span data-stu-id="645dd-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="645dd-149">agentGroups</span><span class="sxs-lookup"><span data-stu-id="645dd-149">agentGroups</span></span>|<span data-ttu-id="645dd-150">[коллекция onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="645dd-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="645dd-151">Список **onPremisesAgentGroups,** который назначен **onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="645dd-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="645dd-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="645dd-152">Read-only.</span></span> <span data-ttu-id="645dd-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="645dd-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="645dd-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="645dd-154">JSON representation</span></span>

<span data-ttu-id="645dd-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="645dd-155">The following is a JSON representation of the resource.</span></span>

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



