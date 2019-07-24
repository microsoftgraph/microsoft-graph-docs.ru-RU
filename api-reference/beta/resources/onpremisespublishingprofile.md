---
title: Тип ресурса Онпремисеспублишингпрофиле
description: Тип ресурса Онпремисеспублишингпрофиле.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1eb442b6f3317ac7c0e2f130442e4a62c7f9c152
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841327"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="ce195-103">Тип ресурса Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="ce195-103">onPremisesPublishingProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce195-104">Различные службы Azure (например, Азуе, сквозная проверка подлинности подключения Active Directory, подготовка пользователей к работе в Azure AD) разрешает условный доступ к различным локальным ресурсам извне корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="ce195-104">Various Azure services (for example, Azue Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="ce195-105">[Локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному опубликованному ресурсу или [](publishedresource.md)обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="ce195-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="ce195-106">[Группы агентов](onpremisesagentgroup.md) позволяют администратору клиента назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ce195-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="ce195-107">Администраторы клиентов могут объединить несколько агентов в группу, а затем назначить каждый опубликованный ресурс группе.</span><span class="sxs-lookup"><span data-stu-id="ce195-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="ce195-108">Весь набор сущностей одного локального типа публикации представлен **онпремисеспублишингпрофиле**.</span><span class="sxs-lookup"><span data-stu-id="ce195-108">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="ce195-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ce195-109">Methods</span></span>

| <span data-ttu-id="ce195-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ce195-110">Method</span></span>       | <span data-ttu-id="ce195-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ce195-111">Return Type</span></span> | <span data-ttu-id="ce195-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ce195-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ce195-113">Получение Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="ce195-113">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="ce195-114">Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="ce195-114">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="ce195-115">Чтение свойств и связей объекта **онпремисеспублишингпрофиле** .</span><span class="sxs-lookup"><span data-stu-id="ce195-115">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="ce195-116">Обновление Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="ce195-116">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="ce195-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ce195-117">None</span></span> | <span data-ttu-id="ce195-118">Обновление объекта [онпремисеспублишингпрофиле](onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ce195-118">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="ce195-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce195-119">Properties</span></span>

| <span data-ttu-id="ce195-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce195-120">Property</span></span>     | <span data-ttu-id="ce195-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ce195-121">Type</span></span>        | <span data-ttu-id="ce195-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ce195-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce195-123">Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ce195-123">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="ce195-124">Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ce195-124">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="ce195-125">Представляет объект **хибридажентупдатерконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="ce195-125">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="ce195-126">id</span><span class="sxs-lookup"><span data-stu-id="ce195-126">id</span></span>|<span data-ttu-id="ce195-127">String</span><span class="sxs-lookup"><span data-stu-id="ce195-127">String</span></span>| <span data-ttu-id="ce195-128">Представляет тип публикации.</span><span class="sxs-lookup"><span data-stu-id="ce195-128">Represents a publishing type.</span></span> <span data-ttu-id="ce195-129">Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="ce195-129">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="ce195-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce195-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce195-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="ce195-131">Relationships</span></span>

| <span data-ttu-id="ce195-132">Отношение</span><span class="sxs-lookup"><span data-stu-id="ce195-132">Relationship</span></span> | <span data-ttu-id="ce195-133">Тип</span><span class="sxs-lookup"><span data-stu-id="ce195-133">Type</span></span>        | <span data-ttu-id="ce195-134">Описание</span><span class="sxs-lookup"><span data-stu-id="ce195-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce195-135">Ажентграупс</span><span class="sxs-lookup"><span data-stu-id="ce195-135">agentGroups</span></span>|<span data-ttu-id="ce195-136">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="ce195-136">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="ce195-137">Список существующих объектов **онпремисесажентграуп** .</span><span class="sxs-lookup"><span data-stu-id="ce195-137">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="ce195-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce195-138">Read-only.</span></span> <span data-ttu-id="ce195-139">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ce195-139">Nullable.</span></span>|
|<span data-ttu-id="ce195-140">агенты</span><span class="sxs-lookup"><span data-stu-id="ce195-140">agents</span></span>|<span data-ttu-id="ce195-141">Коллекция [онпремисесажент](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="ce195-141">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="ce195-142">Список существующих объектов **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="ce195-142">List of existed **onPremisesAgent** objects.</span></span> <span data-ttu-id="ce195-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce195-143">Read-only.</span></span> <span data-ttu-id="ce195-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ce195-144">Nullable.</span></span>|
|<span data-ttu-id="ce195-145">Публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="ce195-145">publishedResources</span></span>|<span data-ttu-id="ce195-146">Коллекция [публишедресаурце](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="ce195-146">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="ce195-147">Список существующих объектов **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="ce195-147">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="ce195-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ce195-148">Read-only.</span></span> <span data-ttu-id="ce195-149">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ce195-149">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce195-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce195-150">JSON representation</span></span>

<span data-ttu-id="ce195-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce195-151">The following is a JSON representation of the resource.</span></span>

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
