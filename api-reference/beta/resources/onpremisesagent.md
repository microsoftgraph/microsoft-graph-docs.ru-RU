---
title: Тип ресурса Онпремисесажент
description: Тип ресурса Онпремисесажент.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ec125e52eaf9eba3423f70dd47cc7dd1562716bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052606"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="629a3-103">Тип ресурса Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="629a3-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="629a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="629a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="629a3-105">Представляет локальный агент.</span><span class="sxs-lookup"><span data-stu-id="629a3-105">Represents on-premises agent.</span></span> <span data-ttu-id="629a3-106">Локальные агенты, установленные администратором клиента, можно настроить для доступа к определенному [опубликованному ресурсу](publishedresource.md)или обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="629a3-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="629a3-107">Методы</span><span class="sxs-lookup"><span data-stu-id="629a3-107">Methods</span></span>

| <span data-ttu-id="629a3-108">Метод</span><span class="sxs-lookup"><span data-stu-id="629a3-108">Method</span></span>       | <span data-ttu-id="629a3-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="629a3-109">Return Type</span></span> | <span data-ttu-id="629a3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="629a3-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="629a3-111">Список Онпремисесажентс</span><span class="sxs-lookup"><span data-stu-id="629a3-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="629a3-112">Коллекция [онпремисесажент](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="629a3-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="629a3-113">Получение коллекции объектов **онпремисесажентс** .</span><span class="sxs-lookup"><span data-stu-id="629a3-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="629a3-114">Получение Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="629a3-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="629a3-115">онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="629a3-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="629a3-116">Чтение свойств и связей объекта **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="629a3-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="629a3-117">Назначение Онпремисесажент для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="629a3-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="629a3-118">Нет</span><span class="sxs-lookup"><span data-stu-id="629a3-118">None</span></span> | <span data-ttu-id="629a3-119">Назначение **онпремисесажент** для **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="629a3-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="629a3-120">Удаление Онпремисесажент из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="629a3-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="629a3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="629a3-121">None</span></span> | <span data-ttu-id="629a3-122">Удаление **онпремисесажент** из **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="629a3-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="629a3-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="629a3-123">Properties</span></span>

| <span data-ttu-id="629a3-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="629a3-124">Property</span></span>     | <span data-ttu-id="629a3-125">Тип</span><span class="sxs-lookup"><span data-stu-id="629a3-125">Type</span></span>        | <span data-ttu-id="629a3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="629a3-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="629a3-127">екстерналип</span><span class="sxs-lookup"><span data-stu-id="629a3-127">externalIp</span></span>|<span data-ttu-id="629a3-128">String</span><span class="sxs-lookup"><span data-stu-id="629a3-128">String</span></span>|<span data-ttu-id="629a3-129">Внешний IP-адрес, обнаруженный службой для компьютера агента.</span><span class="sxs-lookup"><span data-stu-id="629a3-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="629a3-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="629a3-130">Read-only</span></span>|
|<span data-ttu-id="629a3-131">id</span><span class="sxs-lookup"><span data-stu-id="629a3-131">id</span></span>|<span data-ttu-id="629a3-132">String</span><span class="sxs-lookup"><span data-stu-id="629a3-132">String</span></span>| <span data-ttu-id="629a3-133">Идентификатор объекта Онпремисесажент.</span><span class="sxs-lookup"><span data-stu-id="629a3-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="629a3-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="629a3-134">Read-only.</span></span>|
|<span data-ttu-id="629a3-135">ИмяКомпьютера</span><span class="sxs-lookup"><span data-stu-id="629a3-135">machineName</span></span>|<span data-ttu-id="629a3-136">String</span><span class="sxs-lookup"><span data-stu-id="629a3-136">String</span></span>|<span data-ttu-id="629a3-137">Имя компьютера, на котором выполняется агжент.</span><span class="sxs-lookup"><span data-stu-id="629a3-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="629a3-138">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="629a3-138">Read-only</span></span>|
|<span data-ttu-id="629a3-139">status</span><span class="sxs-lookup"><span data-stu-id="629a3-139">status</span></span>|<span data-ttu-id="629a3-140">string</span><span class="sxs-lookup"><span data-stu-id="629a3-140">string</span></span>| <span data-ttu-id="629a3-141">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="629a3-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="629a3-142">публишингтипе</span><span class="sxs-lookup"><span data-stu-id="629a3-142">publishingType</span></span>|<span data-ttu-id="629a3-143">string</span><span class="sxs-lookup"><span data-stu-id="629a3-143">string</span></span>| <span data-ttu-id="629a3-144">Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="629a3-144">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="629a3-145">Связи</span><span class="sxs-lookup"><span data-stu-id="629a3-145">Relationships</span></span>

| <span data-ttu-id="629a3-146">Связь</span><span class="sxs-lookup"><span data-stu-id="629a3-146">Relationship</span></span> | <span data-ttu-id="629a3-147">Тип</span><span class="sxs-lookup"><span data-stu-id="629a3-147">Type</span></span>        | <span data-ttu-id="629a3-148">Описание</span><span class="sxs-lookup"><span data-stu-id="629a3-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="629a3-149">ажентграупс</span><span class="sxs-lookup"><span data-stu-id="629a3-149">agentGroups</span></span>|<span data-ttu-id="629a3-150">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="629a3-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="629a3-151">Список **онпремисесажентграупс** , которым назначено **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="629a3-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="629a3-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="629a3-152">Read-only.</span></span> <span data-ttu-id="629a3-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="629a3-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="629a3-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="629a3-154">JSON representation</span></span>

<span data-ttu-id="629a3-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="629a3-155">The following is a JSON representation of the resource.</span></span>

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


