---
title: Тип ресурса Онпремисеспублишингпрофиле
description: Тип ресурса Онпремисеспублишингпрофиле.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ce99713637d7607caed40451a0716cb0acde14e4
ms.sourcegitcommit: e87be8765d7f2bc90c6244d84c4719468bb3fd25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2019
ms.locfileid: "37113921"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="5964b-103">Тип ресурса Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="5964b-103">onPremisesPublishingProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5964b-104">Различные службы Azure (например, сквозная проверка подлинности подключения Azure Active Directory, подготовка пользователей рабочего дня к Azure AD) обеспечивают условный доступ к различным локальным ресурсам извне корпоративной сети.</span><span class="sxs-lookup"><span data-stu-id="5964b-104">Various Azure services (for example, Azure Active Directory Connect Passthrough Authentication, Workday to Azure AD users provisioning) allow a conditional access to various on-premises resources from outside the corporate network.</span></span> <span data-ttu-id="5964b-105">[Локальные агенты](onpremisesagent.md) , установленные администратором клиента, можно настроить для доступа к определенному [опубликованному ресурсу](publishedresource.md)или обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="5964b-105">[On-premises agents](onpremisesagent.md) installed by a tenant administrator can be configured to access/handle requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="5964b-106">[Группы агентов](onpremisesagentgroup.md) позволяют администратору клиента назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5964b-106">[Agent groups](onpremisesagentgroup.md) enable a tenant admin to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="5964b-107">Администраторы клиентов могут объединить несколько агентов в группу, а затем назначить каждый опубликованный ресурс группе.</span><span class="sxs-lookup"><span data-stu-id="5964b-107">Tenant admins can group a number of agents together, and then assign each published resource to a group.</span></span> <span data-ttu-id="5964b-108">Весь набор сущностей одного локального типа публикации представлен **онпремисеспублишингпрофиле**.</span><span class="sxs-lookup"><span data-stu-id="5964b-108">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="5964b-109">Методы</span><span class="sxs-lookup"><span data-stu-id="5964b-109">Methods</span></span>

| <span data-ttu-id="5964b-110">Метод</span><span class="sxs-lookup"><span data-stu-id="5964b-110">Method</span></span>       | <span data-ttu-id="5964b-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5964b-111">Return Type</span></span> | <span data-ttu-id="5964b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5964b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5964b-113">Получение Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="5964b-113">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="5964b-114">онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="5964b-114">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="5964b-115">Чтение свойств и связей объекта **онпремисеспублишингпрофиле** .</span><span class="sxs-lookup"><span data-stu-id="5964b-115">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="5964b-116">Обновление Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="5964b-116">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="5964b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="5964b-117">None</span></span> | <span data-ttu-id="5964b-118">Обновление объекта [онпремисеспублишингпрофиле](onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5964b-118">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="5964b-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="5964b-119">Properties</span></span>

| <span data-ttu-id="5964b-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="5964b-120">Property</span></span>     | <span data-ttu-id="5964b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5964b-121">Type</span></span>        | <span data-ttu-id="5964b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5964b-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5964b-123">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5964b-123">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="5964b-124">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5964b-124">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="5964b-125">Представляет объект **хибридажентупдатерконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="5964b-125">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="5964b-126">id</span><span class="sxs-lookup"><span data-stu-id="5964b-126">id</span></span>|<span data-ttu-id="5964b-127">String</span><span class="sxs-lookup"><span data-stu-id="5964b-127">String</span></span>| <span data-ttu-id="5964b-128">Представляет тип публикации.</span><span class="sxs-lookup"><span data-stu-id="5964b-128">Represents a publishing type.</span></span> <span data-ttu-id="5964b-129">Возможные значения: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="5964b-129">Possible values are: `appProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="5964b-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5964b-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5964b-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="5964b-131">Relationships</span></span>

| <span data-ttu-id="5964b-132">Отношение</span><span class="sxs-lookup"><span data-stu-id="5964b-132">Relationship</span></span> | <span data-ttu-id="5964b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="5964b-133">Type</span></span>        | <span data-ttu-id="5964b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5964b-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5964b-135">ажентграупс</span><span class="sxs-lookup"><span data-stu-id="5964b-135">agentGroups</span></span>|<span data-ttu-id="5964b-136">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5964b-136">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="5964b-137">Список существующих объектов **онпремисесажентграуп** .</span><span class="sxs-lookup"><span data-stu-id="5964b-137">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="5964b-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5964b-138">Read-only.</span></span> <span data-ttu-id="5964b-139">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5964b-139">Nullable.</span></span>|
|<span data-ttu-id="5964b-140">агенты</span><span class="sxs-lookup"><span data-stu-id="5964b-140">agents</span></span>|<span data-ttu-id="5964b-141">Коллекция [онпремисесажент](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="5964b-141">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="5964b-142">Список существующих объектов **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="5964b-142">List of existed **onPremisesAgent** objects.</span></span> <span data-ttu-id="5964b-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5964b-143">Read-only.</span></span> <span data-ttu-id="5964b-144">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5964b-144">Nullable.</span></span>|
|<span data-ttu-id="5964b-145">публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="5964b-145">publishedResources</span></span>|<span data-ttu-id="5964b-146">Коллекция [публишедресаурце](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="5964b-146">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="5964b-147">Список существующих объектов **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="5964b-147">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="5964b-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5964b-148">Read-only.</span></span> <span data-ttu-id="5964b-149">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5964b-149">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5964b-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5964b-150">JSON representation</span></span>

<span data-ttu-id="5964b-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5964b-151">The following is a JSON representation of the resource.</span></span>

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
