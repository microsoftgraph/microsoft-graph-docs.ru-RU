---
title: Тип ресурса Онпремисеспублишингпрофиле
description: Тип ресурса Онпремисеспублишингпрофиле.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 94d09955ad20af1117b156e433c95f2914df7348
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522202"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="a5dea-103">Тип ресурса Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="a5dea-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="a5dea-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a5dea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5dea-105">Различные службы Azure (например, сквозная проверка подлинности подключения Azure Active Directory, подготовка пользователей рабочего дня к Azure AD) обеспечивают условный доступ к различным локальным ресурсам извне корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="a5dea-105">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="a5dea-106">[Локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному [опубликованному ресурсу](publishedresource.md)или обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="a5dea-106">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="a5dea-107">[Группы агентов](onpremisesagentgroup.md) позволяют администратору клиента назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a5dea-107">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="a5dea-108">Администраторы клиентов могут объединить несколько агентов в группу, а затем назначить каждый опубликованный ресурс группе.</span><span class="sxs-lookup"><span data-stu-id="a5dea-108">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="a5dea-109">Весь набор сущностей одного локального типа публикации представлен **онпремисеспублишингпрофиле**.</span><span class="sxs-lookup"><span data-stu-id="a5dea-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="a5dea-110">Методы</span><span class="sxs-lookup"><span data-stu-id="a5dea-110">Methods</span></span>

| <span data-ttu-id="a5dea-111">Метод</span><span class="sxs-lookup"><span data-stu-id="a5dea-111">Method</span></span>       | <span data-ttu-id="a5dea-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a5dea-112">Return Type</span></span> | <span data-ttu-id="a5dea-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a5dea-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a5dea-114">Получение Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="a5dea-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="a5dea-115">онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="a5dea-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="a5dea-116">Чтение свойств и связей объекта **онпремисеспублишингпрофиле** .</span><span class="sxs-lookup"><span data-stu-id="a5dea-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="a5dea-117">Обновление Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="a5dea-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="a5dea-118">Нет</span><span class="sxs-lookup"><span data-stu-id="a5dea-118">None</span></span> | <span data-ttu-id="a5dea-119">Обновление объекта [онпремисеспублишингпрофиле](onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a5dea-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="a5dea-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5dea-120">Properties</span></span>

| <span data-ttu-id="a5dea-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5dea-121">Property</span></span>     | <span data-ttu-id="a5dea-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a5dea-122">Type</span></span>        | <span data-ttu-id="a5dea-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a5dea-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5dea-124">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a5dea-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="a5dea-125">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="a5dea-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="a5dea-126">Представляет объект **хибридажентупдатерконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="a5dea-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="a5dea-127">id</span><span class="sxs-lookup"><span data-stu-id="a5dea-127">id</span></span>|<span data-ttu-id="a5dea-128">String</span><span class="sxs-lookup"><span data-stu-id="a5dea-128">String</span></span>| <span data-ttu-id="a5dea-129">Представляет тип публикации.</span><span class="sxs-lookup"><span data-stu-id="a5dea-129">Represents a publishing type.</span></span> <span data-ttu-id="a5dea-130">Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="a5dea-130">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="a5dea-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5dea-131">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5dea-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="a5dea-132">Relationships</span></span>

| <span data-ttu-id="a5dea-133">Связь</span><span class="sxs-lookup"><span data-stu-id="a5dea-133">Relationship</span></span> | <span data-ttu-id="a5dea-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a5dea-134">Type</span></span>        | <span data-ttu-id="a5dea-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a5dea-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5dea-136">ажентграупс</span><span class="sxs-lookup"><span data-stu-id="a5dea-136">agentGroups</span></span>|<span data-ttu-id="a5dea-137">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="a5dea-137">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="a5dea-138">Список существующих объектов **онпремисесажентграуп** .</span><span class="sxs-lookup"><span data-stu-id="a5dea-138">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="a5dea-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5dea-139">Read-only.</span></span> <span data-ttu-id="a5dea-140">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a5dea-140">Nullable.</span></span>|
|<span data-ttu-id="a5dea-141">агенты</span><span class="sxs-lookup"><span data-stu-id="a5dea-141">agents</span></span>|<span data-ttu-id="a5dea-142">Коллекция [онпремисесажент](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="a5dea-142">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="a5dea-143">Список существующих объектов **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="a5dea-143">List of existed **onPremisesAgent** objects.</span></span> <span data-ttu-id="a5dea-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5dea-144">Read-only.</span></span> <span data-ttu-id="a5dea-145">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a5dea-145">Nullable.</span></span>|
|<span data-ttu-id="a5dea-146">публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="a5dea-146">publishedResources</span></span>|<span data-ttu-id="a5dea-147">Коллекция [публишедресаурце](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="a5dea-147">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="a5dea-148">Список существующих объектов **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="a5dea-148">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="a5dea-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5dea-149">Read-only.</span></span> <span data-ttu-id="a5dea-150">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a5dea-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5dea-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5dea-151">JSON representation</span></span>

<span data-ttu-id="a5dea-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5dea-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "hybridAgentUpdaterConfiguration": {"@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
