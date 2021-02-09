---
title: Тип ресурса onPremisesPublishingProfile
description: Тип ресурса onPremisesPublishingProfile.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: a7dc65f0640d2bfde9a46595b04fc24fc7512475
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156714"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="6c439-103">Тип ресурса onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="6c439-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="6c439-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c439-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c439-105">Различные службы Azure (например, azure Active Directory Connect [Passthrough Authentication,](/azure/active-directory/hybrid/how-to-connect-pta) [Workday to Azure AD users provisioning,](/azure/active-directory/saas-apps/workday-inbound-tutorial)and [Application Proxy](https://aka.ms/whyappproxy) allow access to various on-premises resources from outside the corporate network.</span><span class="sxs-lookup"><span data-stu-id="6c439-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy) allow access to various on-premises resources from outside the corporate network.</span></span>

<span data-ttu-id="6c439-106">[Установленные](onpremisesagent.md) администратором локально агенты [(или](connector.md) соединители для прокси приложения) могут быть настроены для маршрутов запросов на [определенный опубликованный ресурс.](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="6c439-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by an administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="6c439-107">[Группы агентов](onpremisesagentgroup.md) (или группы [соединители](connectorgroup.md) для прокси приложения) позволяют администратору назначать определенных агентов для обслуживания определенных опубликованных локального ресурса.</span><span class="sxs-lookup"><span data-stu-id="6c439-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable an administrator to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="6c439-108">Администраторы также могут сгруппить несколько агентов, а затем назначить каждый опубликованный ресурс группе агентов.</span><span class="sxs-lookup"><span data-stu-id="6c439-108">Administrators can also group multiple agents together, and then assign each published resource to an agent group.</span></span> <span data-ttu-id="6c439-109">Весь набор сущностями того же локального типа публикации представлен **onPremisesPublishingProfile.**</span><span class="sxs-lookup"><span data-stu-id="6c439-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="6c439-110">Методы</span><span class="sxs-lookup"><span data-stu-id="6c439-110">Methods</span></span>

| <span data-ttu-id="6c439-111">Метод</span><span class="sxs-lookup"><span data-stu-id="6c439-111">Method</span></span>       | <span data-ttu-id="6c439-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6c439-112">Return Type</span></span> | <span data-ttu-id="6c439-113">Описание</span><span class="sxs-lookup"><span data-stu-id="6c439-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6c439-114">Get onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="6c439-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="6c439-115">onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="6c439-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="6c439-116">Чтение свойств и связей объекта **onPremisesPublishingProfile.**</span><span class="sxs-lookup"><span data-stu-id="6c439-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="6c439-117">Обновление onPremisesPublishingProfile</span><span class="sxs-lookup"><span data-stu-id="6c439-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="6c439-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6c439-118">None</span></span> | <span data-ttu-id="6c439-119">Обновление объекта [onPremisesPublishingProfile.](onpremisespublishingprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6c439-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6c439-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c439-120">Properties</span></span>

| <span data-ttu-id="6c439-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c439-121">Property</span></span>     | <span data-ttu-id="6c439-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6c439-122">Type</span></span>        | <span data-ttu-id="6c439-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6c439-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c439-124">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c439-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="6c439-125">hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c439-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="6c439-126">Представляет объект **hybridAgentUpdaterConfiguration.**</span><span class="sxs-lookup"><span data-stu-id="6c439-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="6c439-127">id</span><span class="sxs-lookup"><span data-stu-id="6c439-127">id</span></span>|<span data-ttu-id="6c439-128">String</span><span class="sxs-lookup"><span data-stu-id="6c439-128">String</span></span>| <span data-ttu-id="6c439-129">Представляет тип публикации.</span><span class="sxs-lookup"><span data-stu-id="6c439-129">Represents a publishing type.</span></span> <span data-ttu-id="6c439-130">Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="6c439-130">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="6c439-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c439-131">Read-only.</span></span>|
|<span data-ttu-id="6c439-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6c439-132">isEnabled</span></span>|<span data-ttu-id="6c439-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c439-133">Boolean</span></span>| <span data-ttu-id="6c439-134">Представляет, включен ли прокси приложения [Azure AD](https://aka.ms/whyappproxy) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c439-134">Represents if [Azure AD Application Proxy](https://aka.ms/whyappproxy) is enabled for the tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6c439-135">Связи</span><span class="sxs-lookup"><span data-stu-id="6c439-135">Relationships</span></span>

| <span data-ttu-id="6c439-136">Связь</span><span class="sxs-lookup"><span data-stu-id="6c439-136">Relationship</span></span> | <span data-ttu-id="6c439-137">Тип</span><span class="sxs-lookup"><span data-stu-id="6c439-137">Type</span></span>        | <span data-ttu-id="6c439-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6c439-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c439-139">agentGroups</span><span class="sxs-lookup"><span data-stu-id="6c439-139">agentGroups</span></span>|<span data-ttu-id="6c439-140">[Коллекция onPremisesAgentGroup](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="6c439-140">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="6c439-141">Список существующих объектов **onPremisesAgentGroup.**</span><span class="sxs-lookup"><span data-stu-id="6c439-141">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="6c439-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c439-142">Read-only.</span></span> <span data-ttu-id="6c439-143">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6c439-143">Nullable.</span></span>|
|<span data-ttu-id="6c439-144">агенты</span><span class="sxs-lookup"><span data-stu-id="6c439-144">agents</span></span>|<span data-ttu-id="6c439-145">[Коллекция onPremisesAgent](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="6c439-145">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="6c439-146">Список существующих **объектов onPremisesAgent.**</span><span class="sxs-lookup"><span data-stu-id="6c439-146">List of existing **onPremisesAgent** objects.</span></span> <span data-ttu-id="6c439-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c439-147">Read-only.</span></span> <span data-ttu-id="6c439-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6c439-148">Nullable.</span></span>|
|<span data-ttu-id="6c439-149">connectorGroups</span><span class="sxs-lookup"><span data-stu-id="6c439-149">connectorGroups</span></span>|<span data-ttu-id="6c439-150">[Коллекция connectorGroup](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="6c439-150">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="6c439-151">Список существующих объектов **connectorGroup для** приложений, опубликованных через прокси приложения.</span><span class="sxs-lookup"><span data-stu-id="6c439-151">List of existing **connectorGroup** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="6c439-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c439-152">Read-only.</span></span> <span data-ttu-id="6c439-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6c439-153">Nullable.</span></span>|
|<span data-ttu-id="6c439-154">соединители</span><span class="sxs-lookup"><span data-stu-id="6c439-154">connectors</span></span>|<span data-ttu-id="6c439-155">[коллекция соединители](connector.md)</span><span class="sxs-lookup"><span data-stu-id="6c439-155">[connector](connector.md) collection</span></span>| <span data-ttu-id="6c439-156">Список существующих объектов **соединитений** для приложений, опубликованных через прокси приложения.</span><span class="sxs-lookup"><span data-stu-id="6c439-156">List of existing **connector** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="6c439-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c439-157">Read-only.</span></span> <span data-ttu-id="6c439-158">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6c439-158">Nullable.</span></span>|
|<span data-ttu-id="6c439-159">publishedResources</span><span class="sxs-lookup"><span data-stu-id="6c439-159">publishedResources</span></span>|<span data-ttu-id="6c439-160">[Коллекция publishedResource](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="6c439-160">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="6c439-161">Список существующих **объектов publishedResource.**</span><span class="sxs-lookup"><span data-stu-id="6c439-161">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="6c439-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6c439-162">Read-only.</span></span> <span data-ttu-id="6c439-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6c439-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c439-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c439-164">JSON representation</span></span>

<span data-ttu-id="6c439-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c439-165">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingProfile",
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



