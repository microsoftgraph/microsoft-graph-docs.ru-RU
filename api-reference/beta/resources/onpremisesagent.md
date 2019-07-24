---
title: Тип ресурса Онпремисесажент
description: Тип ресурса Онпремисесажент.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1bcff659cf30b946654f14190b2cf5f693d27bc4
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841264"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="1043b-103">Тип ресурса Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="1043b-103">onPremisesAgent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1043b-104">Представляет локальный агент.</span><span class="sxs-lookup"><span data-stu-id="1043b-104">Represents on-premises agent.</span></span> <span data-ttu-id="1043b-105">Локальные агенты, установленные администратором клиента, можно настроить для доступа к определенному опубликованному ресурсу или [](publishedresource.md)обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="1043b-105">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1043b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="1043b-106">Methods</span></span>

| <span data-ttu-id="1043b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="1043b-107">Method</span></span>       | <span data-ttu-id="1043b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1043b-108">Return Type</span></span> | <span data-ttu-id="1043b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1043b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1043b-110">Список Онпремисесажентс</span><span class="sxs-lookup"><span data-stu-id="1043b-110">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="1043b-111">Коллекция [онпремисесажент](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="1043b-111">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="1043b-112">Получение коллекции объектов **онпремисесажентс** .</span><span class="sxs-lookup"><span data-stu-id="1043b-112">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="1043b-113">Получение Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="1043b-113">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="1043b-114">Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="1043b-114">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="1043b-115">Чтение свойств и связей объекта **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="1043b-115">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="1043b-116">Назначение Онпремисесажент для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="1043b-116">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="1043b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="1043b-117">None</span></span> | <span data-ttu-id="1043b-118">Назначение **онпремисесажент** для **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="1043b-118">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="1043b-119">Удаление Онпремисесажент из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="1043b-119">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="1043b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="1043b-120">None</span></span> | <span data-ttu-id="1043b-121">Удаление **онпремисесажент** из **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="1043b-121">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="1043b-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="1043b-122">Properties</span></span>

| <span data-ttu-id="1043b-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="1043b-123">Property</span></span>     | <span data-ttu-id="1043b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1043b-124">Type</span></span>        | <span data-ttu-id="1043b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1043b-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1043b-126">Екстерналип</span><span class="sxs-lookup"><span data-stu-id="1043b-126">externalIp</span></span>|<span data-ttu-id="1043b-127">String</span><span class="sxs-lookup"><span data-stu-id="1043b-127">String</span></span>|<span data-ttu-id="1043b-128">Внешний IP-адрес, обнаруженный службой для компьютера агента.</span><span class="sxs-lookup"><span data-stu-id="1043b-128">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="1043b-129">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="1043b-129">Read-only</span></span>|
|<span data-ttu-id="1043b-130">id</span><span class="sxs-lookup"><span data-stu-id="1043b-130">id</span></span>|<span data-ttu-id="1043b-131">Строка</span><span class="sxs-lookup"><span data-stu-id="1043b-131">String</span></span>| <span data-ttu-id="1043b-132">Идентификатор объекта Онпремисесажент.</span><span class="sxs-lookup"><span data-stu-id="1043b-132">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="1043b-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1043b-133">Read-only.</span></span>|
|<span data-ttu-id="1043b-134">ИмяКомпьютера</span><span class="sxs-lookup"><span data-stu-id="1043b-134">machineName</span></span>|<span data-ttu-id="1043b-135">String</span><span class="sxs-lookup"><span data-stu-id="1043b-135">String</span></span>|<span data-ttu-id="1043b-136">Имя компьютера, на котором выполняется агжент.</span><span class="sxs-lookup"><span data-stu-id="1043b-136">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="1043b-137">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="1043b-137">Read-only</span></span>|
|<span data-ttu-id="1043b-138">status</span><span class="sxs-lookup"><span data-stu-id="1043b-138">status</span></span>|<span data-ttu-id="1043b-139">string</span><span class="sxs-lookup"><span data-stu-id="1043b-139">string</span></span>| <span data-ttu-id="1043b-140">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="1043b-140">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="1043b-141">Публишингтипе</span><span class="sxs-lookup"><span data-stu-id="1043b-141">publishingType</span></span>|<span data-ttu-id="1043b-142">string</span><span class="sxs-lookup"><span data-stu-id="1043b-142">string</span></span>| <span data-ttu-id="1043b-143">Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="1043b-143">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1043b-144">Отношения</span><span class="sxs-lookup"><span data-stu-id="1043b-144">Relationships</span></span>

| <span data-ttu-id="1043b-145">Отношение</span><span class="sxs-lookup"><span data-stu-id="1043b-145">Relationship</span></span> | <span data-ttu-id="1043b-146">Тип</span><span class="sxs-lookup"><span data-stu-id="1043b-146">Type</span></span>        | <span data-ttu-id="1043b-147">Описание</span><span class="sxs-lookup"><span data-stu-id="1043b-147">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1043b-148">Ажентграупс</span><span class="sxs-lookup"><span data-stu-id="1043b-148">agentGroups</span></span>|<span data-ttu-id="1043b-149">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="1043b-149">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="1043b-150">Список **онпремисесажентграупс** , которым назначено **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="1043b-150">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="1043b-151">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1043b-151">Read-only.</span></span> <span data-ttu-id="1043b-152">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1043b-152">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1043b-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1043b-153">JSON representation</span></span>

<span data-ttu-id="1043b-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1043b-154">The following is a JSON representation of the resource.</span></span>

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
