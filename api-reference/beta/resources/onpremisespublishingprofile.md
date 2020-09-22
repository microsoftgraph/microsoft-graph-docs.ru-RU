---
title: Тип ресурса Онпремисеспублишингпрофиле
description: Тип ресурса Онпремисеспублишингпрофиле.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b0f2bf125593c72ba72ae4109baffcae46e88f33
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998655"
---
# <a name="onpremisespublishingprofile-resource-type"></a><span data-ttu-id="74663-103">Тип ресурса Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="74663-103">onPremisesPublishingProfile resource type</span></span>

<span data-ttu-id="74663-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74663-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74663-105">Различные службы Azure (например, [сквозная проверка подлинности](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta)подключения Azure Active Directory, подключение [рабочего дня к пользователям Azure AD](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)и [прокси приложения](https://aka.ms/whyappproxy) — предоставление доступа к различным локальным ресурсам извне корпоративной сети).</span><span class="sxs-lookup"><span data-stu-id="74663-105">Various Azure services (for example, Azure Active Directory Connect [Passthrough Authentication](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta), [Workday to Azure AD users provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial), and [Application Proxy](https://aka.ms/whyappproxy) allow access to various on-premises resources from outside the corporate network.</span></span>

<span data-ttu-id="74663-106">[Локальные агенты](onpremisesagent.md) (или [соединители](connector.md) для прокси-сервера приложения), установленные администратором, могут быть настроены на маршрутизацию запросов на конкретный [опубликованный ресурс](publishedresource.md).</span><span class="sxs-lookup"><span data-stu-id="74663-106">[On-premises agents](onpremisesagent.md) (or [connectors](connector.md) for Application Proxy) installed by an administrator can be configured to route requests to a particular [published resource](publishedresource.md).</span></span>
<span data-ttu-id="74663-107">[Группы агентов](onpremisesagentgroup.md) (или [группы соединителей](connectorgroup.md) для прокси приложения) позволяют администратору назначать определенные агенты для обслуживания определенных опубликованных локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="74663-107">[Agent groups](onpremisesagentgroup.md) (or [connector groups](connectorgroup.md) for Application Proxy) enable an administrator to assign specific agents to serve specific published on-premises resources.</span></span> <span data-ttu-id="74663-108">Администраторы также могут группировать несколько агентов вместе, а затем назначать каждый опубликованный ресурс группе агентов.</span><span class="sxs-lookup"><span data-stu-id="74663-108">Administrators can also group multiple agents together, and then assign each published resource to an agent group.</span></span> <span data-ttu-id="74663-109">Весь набор сущностей одного локального типа публикации представлен **онпремисеспублишингпрофиле**.</span><span class="sxs-lookup"><span data-stu-id="74663-109">The entire set of entities of the same on-premises publishing type is represented by **onPremisesPublishingProfile**.</span></span>

## <a name="methods"></a><span data-ttu-id="74663-110">Методы</span><span class="sxs-lookup"><span data-stu-id="74663-110">Methods</span></span>

| <span data-ttu-id="74663-111">Метод</span><span class="sxs-lookup"><span data-stu-id="74663-111">Method</span></span>       | <span data-ttu-id="74663-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74663-112">Return Type</span></span> | <span data-ttu-id="74663-113">Описание</span><span class="sxs-lookup"><span data-stu-id="74663-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="74663-114">Получение Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="74663-114">Get onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-get.md) | [<span data-ttu-id="74663-115">онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="74663-115">onPremisesPublishingProfile</span></span>](onpremisespublishingprofile.md) | <span data-ttu-id="74663-116">Чтение свойств и связей объекта **онпремисеспублишингпрофиле** .</span><span class="sxs-lookup"><span data-stu-id="74663-116">Read the properties and relationships of an **onPremisesPublishingProfile** object.</span></span> |
| [<span data-ttu-id="74663-117">Обновление Онпремисеспублишингпрофиле</span><span class="sxs-lookup"><span data-stu-id="74663-117">Update onPremisesPublishingProfile</span></span>](../api/onpremisespublishingprofile-update.md) | <span data-ttu-id="74663-118">Нет</span><span class="sxs-lookup"><span data-stu-id="74663-118">None</span></span> | <span data-ttu-id="74663-119">Обновление объекта [онпремисеспублишингпрофиле](onpremisespublishingprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="74663-119">Update an [onPremisesPublishingProfile](onpremisespublishingprofile.md) object.</span></span> |

## <a name="properties"></a><span data-ttu-id="74663-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="74663-120">Properties</span></span>

| <span data-ttu-id="74663-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="74663-121">Property</span></span>     | <span data-ttu-id="74663-122">Тип</span><span class="sxs-lookup"><span data-stu-id="74663-122">Type</span></span>        | <span data-ttu-id="74663-123">Описание</span><span class="sxs-lookup"><span data-stu-id="74663-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74663-124">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="74663-124">hybridAgentUpdaterConfiguration</span></span>|[<span data-ttu-id="74663-125">хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="74663-125">hybridAgentUpdaterConfiguration</span></span>](hybridagentupdaterconfiguration.md)| <span data-ttu-id="74663-126">Представляет объект **хибридажентупдатерконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="74663-126">Represents a **hybridAgentUpdaterConfiguration** object.</span></span>|
|<span data-ttu-id="74663-127">id</span><span class="sxs-lookup"><span data-stu-id="74663-127">id</span></span>|<span data-ttu-id="74663-128">String</span><span class="sxs-lookup"><span data-stu-id="74663-128">String</span></span>| <span data-ttu-id="74663-129">Представляет тип публикации.</span><span class="sxs-lookup"><span data-stu-id="74663-129">Represents a publishing type.</span></span> <span data-ttu-id="74663-130">Возможные значения: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span><span class="sxs-lookup"><span data-stu-id="74663-130">Possible values are: `applicationProxy`, `exchangeOnline`, `authentication`, `provisioning`, `adAdministration`.</span></span> <span data-ttu-id="74663-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74663-131">Read-only.</span></span>|
|<span data-ttu-id="74663-132">isEnabled</span><span class="sxs-lookup"><span data-stu-id="74663-132">isEnabled</span></span>|<span data-ttu-id="74663-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="74663-133">Boolean</span></span>| <span data-ttu-id="74663-134">Указывает, включен ли [прокси приложения Azure AD](https://aka.ms/whyappproxy) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74663-134">Represents if [Azure AD Application Proxy](https://aka.ms/whyappproxy) is enabled for the tenant.</span></span> |

## <a name="relationships"></a><span data-ttu-id="74663-135">Связи</span><span class="sxs-lookup"><span data-stu-id="74663-135">Relationships</span></span>

| <span data-ttu-id="74663-136">Связь</span><span class="sxs-lookup"><span data-stu-id="74663-136">Relationship</span></span> | <span data-ttu-id="74663-137">Тип</span><span class="sxs-lookup"><span data-stu-id="74663-137">Type</span></span>        | <span data-ttu-id="74663-138">Описание</span><span class="sxs-lookup"><span data-stu-id="74663-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74663-139">ажентграупс</span><span class="sxs-lookup"><span data-stu-id="74663-139">agentGroups</span></span>|<span data-ttu-id="74663-140">Коллекция [онпремисесажентграуп](onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="74663-140">[onPremisesAgentGroup](onpremisesagentgroup.md) collection</span></span>| <span data-ttu-id="74663-141">Список существующих объектов **онпремисесажентграуп** .</span><span class="sxs-lookup"><span data-stu-id="74663-141">List of existing **onPremisesAgentGroup** objects.</span></span> <span data-ttu-id="74663-142">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74663-142">Read-only.</span></span> <span data-ttu-id="74663-143">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="74663-143">Nullable.</span></span>|
|<span data-ttu-id="74663-144">агенты</span><span class="sxs-lookup"><span data-stu-id="74663-144">agents</span></span>|<span data-ttu-id="74663-145">Коллекция [онпремисесажент](onpremisesagent.md)</span><span class="sxs-lookup"><span data-stu-id="74663-145">[onPremisesAgent](onpremisesagent.md) collection</span></span>| <span data-ttu-id="74663-146">Список существующих объектов **онпремисесажент** .</span><span class="sxs-lookup"><span data-stu-id="74663-146">List of existing **onPremisesAgent** objects.</span></span> <span data-ttu-id="74663-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74663-147">Read-only.</span></span> <span data-ttu-id="74663-148">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="74663-148">Nullable.</span></span>|
|<span data-ttu-id="74663-149">коннекторграупс</span><span class="sxs-lookup"><span data-stu-id="74663-149">connectorGroups</span></span>|<span data-ttu-id="74663-150">Коллекция [коннекторграуп](connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="74663-150">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="74663-151">Список существующих объектов **коннекторграуп** для приложений, опубликованных через прокси приложения.</span><span class="sxs-lookup"><span data-stu-id="74663-151">List of existing **connectorGroup** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="74663-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74663-152">Read-only.</span></span> <span data-ttu-id="74663-153">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="74663-153">Nullable.</span></span>|
|<span data-ttu-id="74663-154">аудиовыход</span><span class="sxs-lookup"><span data-stu-id="74663-154">connectors</span></span>|<span data-ttu-id="74663-155">Коллекция [соединителей](connector.md)</span><span class="sxs-lookup"><span data-stu-id="74663-155">[connector](connector.md) collection</span></span>| <span data-ttu-id="74663-156">Список существующих объектов **Connector** для приложений, опубликованных через прокси приложения.</span><span class="sxs-lookup"><span data-stu-id="74663-156">List of existing **connector** objects for applications published through Application Proxy.</span></span> <span data-ttu-id="74663-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74663-157">Read-only.</span></span> <span data-ttu-id="74663-158">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="74663-158">Nullable.</span></span>|
|<span data-ttu-id="74663-159">публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="74663-159">publishedResources</span></span>|<span data-ttu-id="74663-160">Коллекция [публишедресаурце](publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="74663-160">[publishedResource](publishedresource.md) collection</span></span>| <span data-ttu-id="74663-161">Список существующих объектов **публишедресаурце** .</span><span class="sxs-lookup"><span data-stu-id="74663-161">List of existing **publishedResource** objects.</span></span> <span data-ttu-id="74663-162">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74663-162">Read-only.</span></span> <span data-ttu-id="74663-163">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="74663-163">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74663-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74663-164">JSON representation</span></span>

<span data-ttu-id="74663-165">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74663-165">The following is a JSON representation of the resource.</span></span>

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


