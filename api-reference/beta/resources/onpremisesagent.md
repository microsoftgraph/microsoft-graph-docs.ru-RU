---
title: Тип ресурса Онпремисесажент
description: Тип ресурса Онпремисесажент.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fdc6355b33539899ab51a4a6881a8109cb8d87a6
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199755"
---
# <a name="onpremisesagent-resource-type"></a><span data-ttu-id="e7dad-103">Тип ресурса Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="e7dad-103">onPremisesAgent resource type</span></span>

<span data-ttu-id="e7dad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7dad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7dad-105">Представляет локальный агент.</span><span class="sxs-lookup"><span data-stu-id="e7dad-105">Represents on-premises agent.</span></span> <span data-ttu-id="e7dad-106">Локальные агенты, установленные администратором клиента, можно настроить для доступа к определенному [опубликованному ресурсу](publishedresource.md)или обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="e7dad-106">On-premises agents installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e7dad-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e7dad-107">Methods</span></span>

| <span data-ttu-id="e7dad-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e7dad-108">Method</span></span>       | <span data-ttu-id="e7dad-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e7dad-109">Return Type</span></span> | <span data-ttu-id="e7dad-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e7dad-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e7dad-111">Список Онпремисесажентс</span><span class="sxs-lookup"><span data-stu-id="e7dad-111">List onPremisesAgents</span></span>](../api/onpremisesagent-list.md) | <span data-ttu-id="e7dad-112">Коллекция [онпремисесажент](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="e7dad-112">[onPremisesAgent](onpremisesagent.md) collection</span></span> | <span data-ttu-id="e7dad-113">Получение коллекции объектов **онпремисесажентс** .</span><span class="sxs-lookup"><span data-stu-id="e7dad-113">Get an **onPremisesAgents** object collection.</span></span> |
| [<span data-ttu-id="e7dad-114">Получение Онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="e7dad-114">Get onPremisesAgent</span></span>](../api/onpremisesagent-get.md) | [<span data-ttu-id="e7dad-115">онпремисесажент</span><span class="sxs-lookup"><span data-stu-id="e7dad-115">onPremisesAgent</span></span>](onpremisesagent.md) | <span data-ttu-id="e7dad-116">Чтение свойств и связей объекта **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="e7dad-116">Read the properties and relationships of an **onPremisesAgent** object.</span></span> |
| [<span data-ttu-id="e7dad-117">Назначение Онпремисесажент для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="e7dad-117">Assign onPremisesAgent to onPremisesAgentGroup</span></span>](../api/onpremisesagent-post-agentgroups.md) | <span data-ttu-id="e7dad-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e7dad-118">None</span></span> | <span data-ttu-id="e7dad-119">Назначение **онпремисесажент** для **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="e7dad-119">Assign an **onPremisesAgent** to an **onPremisesAgentGroup**.</span></span>|
| [<span data-ttu-id="e7dad-120">Удаление Онпремисесажент из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="e7dad-120">Remove onpremisesAgent from an onPremisesAgentGroup</span></span>](../api/onpremisesagent-delete-agentgroups.md) | <span data-ttu-id="e7dad-121">Нет</span><span class="sxs-lookup"><span data-stu-id="e7dad-121">None</span></span> | <span data-ttu-id="e7dad-122">Удаление **онпремисесажент** из **онпремисесажентграуп**.</span><span class="sxs-lookup"><span data-stu-id="e7dad-122">Remove an **onPremisesAgent** from an **onPremisesAgentGroup**.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7dad-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7dad-123">Properties</span></span>

| <span data-ttu-id="e7dad-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7dad-124">Property</span></span>     | <span data-ttu-id="e7dad-125">Тип</span><span class="sxs-lookup"><span data-stu-id="e7dad-125">Type</span></span>        | <span data-ttu-id="e7dad-126">Описание</span><span class="sxs-lookup"><span data-stu-id="e7dad-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7dad-127">екстерналип</span><span class="sxs-lookup"><span data-stu-id="e7dad-127">externalIp</span></span>|<span data-ttu-id="e7dad-128">String</span><span class="sxs-lookup"><span data-stu-id="e7dad-128">String</span></span>|<span data-ttu-id="e7dad-129">Внешний IP-адрес, обнаруженный службой для компьютера агента.</span><span class="sxs-lookup"><span data-stu-id="e7dad-129">The external IP address as detected by the service for the agent machine.</span></span> <span data-ttu-id="e7dad-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="e7dad-130">Read-only</span></span>|
|<span data-ttu-id="e7dad-131">id</span><span class="sxs-lookup"><span data-stu-id="e7dad-131">id</span></span>|<span data-ttu-id="e7dad-132">Строка</span><span class="sxs-lookup"><span data-stu-id="e7dad-132">String</span></span>| <span data-ttu-id="e7dad-133">Идентификатор объекта Онпремисесажент.</span><span class="sxs-lookup"><span data-stu-id="e7dad-133">The object id of the onPremisesAgent.</span></span> <span data-ttu-id="e7dad-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7dad-134">Read-only.</span></span>|
|<span data-ttu-id="e7dad-135">ИмяКомпьютера</span><span class="sxs-lookup"><span data-stu-id="e7dad-135">machineName</span></span>|<span data-ttu-id="e7dad-136">String</span><span class="sxs-lookup"><span data-stu-id="e7dad-136">String</span></span>|<span data-ttu-id="e7dad-137">Имя компьютера, на котором выполняется агжент.</span><span class="sxs-lookup"><span data-stu-id="e7dad-137">The name of the machine that the aggent is running on.</span></span> <span data-ttu-id="e7dad-138">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="e7dad-138">Read-only</span></span>|
|<span data-ttu-id="e7dad-139">status</span><span class="sxs-lookup"><span data-stu-id="e7dad-139">status</span></span>|<span data-ttu-id="e7dad-140">string</span><span class="sxs-lookup"><span data-stu-id="e7dad-140">string</span></span>| <span data-ttu-id="e7dad-141">Возможные значения: `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="e7dad-141">Possible values are: `active`, `inactive`.</span></span>|
|<span data-ttu-id="e7dad-142">публишингтипе</span><span class="sxs-lookup"><span data-stu-id="e7dad-142">publishingType</span></span>|<span data-ttu-id="e7dad-143">string</span><span class="sxs-lookup"><span data-stu-id="e7dad-143">string</span></span>| <span data-ttu-id="e7dad-144">Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="e7dad-144">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7dad-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="e7dad-145">Relationships</span></span>

| <span data-ttu-id="e7dad-146">Связь</span><span class="sxs-lookup"><span data-stu-id="e7dad-146">Relationship</span></span> | <span data-ttu-id="e7dad-147">Тип</span><span class="sxs-lookup"><span data-stu-id="e7dad-147">Type</span></span>        | <span data-ttu-id="e7dad-148">Описание</span><span class="sxs-lookup"><span data-stu-id="e7dad-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7dad-149">ажентграупс</span><span class="sxs-lookup"><span data-stu-id="e7dad-149">agentGroups</span></span>|<span data-ttu-id="e7dad-150">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="e7dad-150">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="e7dad-151">Список **онпремисесажентграупс** , которым назначено **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="e7dad-151">List of **onPremisesAgentGroups** that an **onPremisesAgent** is assigned to.</span></span> <span data-ttu-id="e7dad-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7dad-152">Read-only.</span></span> <span data-ttu-id="e7dad-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e7dad-153">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7dad-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7dad-154">JSON representation</span></span>

<span data-ttu-id="e7dad-155">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7dad-155">The following is a JSON representation of the resource.</span></span>

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
