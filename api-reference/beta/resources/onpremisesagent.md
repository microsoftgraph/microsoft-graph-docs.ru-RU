---
title: Тип ресурса Онпремисесажент
description: Тип ресурса Онпремисесажент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff30f427c2aac754ba3cfda4082d590e95f5edd3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522244"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="334c7-103">Тип ресурса Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="334c7-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="334c7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="334c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="334c7-105">Представляет локальный агент.</span><span class="sxs-lookup"><span data-stu-id="334c7-105">Represents on-premises agent.</span></span> <span data-ttu-id="334c7-106">Локальные агенты, установленные администратором клиента, можно настроить для доступа к определенному [опубликованному ресурсу](publishedresource.md)или обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="334c7-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="334c7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="334c7-107">Methods</span></span>

| <span data-ttu-id="334c7-108">Метод</span><span class="sxs-lookup"><span data-stu-id="334c7-108">Method</span></span>       | <span data-ttu-id="334c7-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="334c7-109">Return Type</span></span> | <span data-ttu-id="334c7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="334c7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="334c7-111">Список Онпремисесажентс</span><span class="sxs-lookup"><span data-stu-id="334c7-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="334c7-112">Коллекция [онпремисесажент](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="334c7-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="334c7-113">Получение коллекции объектов **онпремисесажентс** .</span><span class="sxs-lookup"><span data-stu-id="334c7-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="334c7-114">Получение Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="334c7-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="334c7-115">онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="334c7-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="334c7-116">Чтение свойств и связей объекта **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="334c7-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="334c7-117">Назначение Онпремисесажент для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="334c7-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="334c7-118">Нет</span><span class="sxs-lookup"><span data-stu-id="334c7-118">None</span></span> | <span data-ttu-id="334c7-119">Назначение **онпремисесажент** для **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="334c7-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="334c7-120">Удаление Онпремисесажент из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="334c7-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="334c7-121">Нет</span><span class="sxs-lookup"><span data-stu-id="334c7-121">None</span></span> | <span data-ttu-id="334c7-122">Удаление **онпремисесажент** из **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="334c7-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="334c7-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="334c7-123">Properties</span></span>

| <span data-ttu-id="334c7-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="334c7-124">Property</span></span>     | <span data-ttu-id="334c7-125">Тип</span><span class="sxs-lookup"><span data-stu-id="334c7-125">Type</span></span>        | <span data-ttu-id="334c7-126">Описание</span><span class="sxs-lookup"><span data-stu-id="334c7-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="334c7-127">екстерналип</span><span class="sxs-lookup"><span data-stu-id="334c7-127">externalIp</span></span>|<span data-ttu-id="334c7-128">String</span><span class="sxs-lookup"><span data-stu-id="334c7-128">String</span></span>|<span data-ttu-id="334c7-129">Внешний IP-адрес, обнаруженный службой для компьютера агента.</span><span class="sxs-lookup"><span data-stu-id="334c7-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="334c7-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="334c7-130">Read-only</span></span>|
|<span data-ttu-id="334c7-131">id</span><span class="sxs-lookup"><span data-stu-id="334c7-131">id</span></span>|<span data-ttu-id="334c7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="334c7-132">String</span></span>| <span data-ttu-id="334c7-133">Идентификатор объекта Онпремисесажент.</span><span class="sxs-lookup"><span data-stu-id="334c7-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="334c7-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="334c7-134">Read-only.</span></span>|
|<span data-ttu-id="334c7-135">ИмяКомпьютера</span><span class="sxs-lookup"><span data-stu-id="334c7-135">machineName</span></span>|<span data-ttu-id="334c7-136">String</span><span class="sxs-lookup"><span data-stu-id="334c7-136">String</span></span>|<span data-ttu-id="334c7-137">Имя компьютера, на котором выполняется агжент.</span><span class="sxs-lookup"><span data-stu-id="334c7-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="334c7-138">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="334c7-138">Read-only</span></span>|
|<span data-ttu-id="334c7-139">status</span><span class="sxs-lookup"><span data-stu-id="334c7-139">status</span></span>|<span data-ttu-id="334c7-140">string</span><span class="sxs-lookup"><span data-stu-id="334c7-140">string</span></span>| <span data-ttu-id="334c7-141">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="334c7-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="334c7-142">публишингтипе</span><span class="sxs-lookup"><span data-stu-id="334c7-142">publishingType</span></span>|<span data-ttu-id="334c7-143">строка</span><span class="sxs-lookup"><span data-stu-id="334c7-143">string</span></span>| <span data-ttu-id="334c7-144">Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="334c7-144">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="334c7-145">Связи</span><span class="sxs-lookup"><span data-stu-id="334c7-145">Relationships</span></span>

| <span data-ttu-id="334c7-146">Связь</span><span class="sxs-lookup"><span data-stu-id="334c7-146">Relationship</span></span> | <span data-ttu-id="334c7-147">Тип</span><span class="sxs-lookup"><span data-stu-id="334c7-147">Type</span></span>        | <span data-ttu-id="334c7-148">Описание</span><span class="sxs-lookup"><span data-stu-id="334c7-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="334c7-149">ажентграупс</span><span class="sxs-lookup"><span data-stu-id="334c7-149">agentGroups</span></span>|<span data-ttu-id="334c7-150">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="334c7-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="334c7-151">Список **онпремисесажентграупс** , которым назначено **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="334c7-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="334c7-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="334c7-152">Read-only.</span></span> <span data-ttu-id="334c7-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="334c7-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="334c7-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="334c7-154">JSON representation</span></span>

<span data-ttu-id="334c7-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="334c7-155">The following is a JSON representation of the resource.</span></span>

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
