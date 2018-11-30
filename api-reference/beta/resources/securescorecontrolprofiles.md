---
title: Тип ресурса secureScoreControlProfiles
description: Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.
ms.openlocfilehash: e02c9ae3b1431b131576e2e0e115377dd3480bc2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080212"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="25626-104">Тип ресурса secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="25626-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="25626-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="25626-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25626-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25626-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25626-107">Представляет безопасной счета клиента в данные элемента управления.</span><span class="sxs-lookup"><span data-stu-id="25626-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="25626-108">По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.</span><span class="sxs-lookup"><span data-stu-id="25626-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="25626-109">Методы</span><span class="sxs-lookup"><span data-stu-id="25626-109">Methods</span></span>

| <span data-ttu-id="25626-110">Метод</span><span class="sxs-lookup"><span data-stu-id="25626-110">Method</span></span>   | <span data-ttu-id="25626-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="25626-111">Return Type</span></span>|<span data-ttu-id="25626-112">Описание</span><span class="sxs-lookup"><span data-stu-id="25626-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25626-113">Список secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="25626-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="25626-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="25626-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="25626-115">Чтение свойства и метаданные объекта secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="25626-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="25626-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="25626-116">Properties</span></span>

|<span data-ttu-id="25626-117">Имя</span><span class="sxs-lookup"><span data-stu-id="25626-117">Name</span></span> |<span data-ttu-id="25626-118">Тип</span><span class="sxs-lookup"><span data-stu-id="25626-118">Type</span></span> |<span data-ttu-id="25626-119">Description</span><span class="sxs-lookup"><span data-stu-id="25626-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="25626-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="25626-120">azureTenantId</span></span>   |   <span data-ttu-id="25626-121">String</span><span class="sxs-lookup"><span data-stu-id="25626-121">String</span></span>  |   <span data-ttu-id="25626-122">Идентификатор GUID строки для клиента.</span><span class="sxs-lookup"><span data-stu-id="25626-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="25626-123">ИмяЭлементаУправления</span><span class="sxs-lookup"><span data-stu-id="25626-123">controlName</span></span> |   <span data-ttu-id="25626-124">String</span><span class="sxs-lookup"><span data-stu-id="25626-124">String</span></span>  |   <span data-ttu-id="25626-125">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="25626-125">Name of the control.</span></span> |
|   <span data-ttu-id="25626-126">title</span><span class="sxs-lookup"><span data-stu-id="25626-126">title</span></span>   |   <span data-ttu-id="25626-127">String</span><span class="sxs-lookup"><span data-stu-id="25626-127">String</span></span>  |   <span data-ttu-id="25626-128">Заголовок элемента управления.</span><span class="sxs-lookup"><span data-stu-id="25626-128">Title of the control.</span></span>   |
|   <span data-ttu-id="25626-129">controlCategory</span><span class="sxs-lookup"><span data-stu-id="25626-129">controlCategory</span></span> |   <span data-ttu-id="25626-130">String</span><span class="sxs-lookup"><span data-stu-id="25626-130">String</span></span>  |   <span data-ttu-id="25626-131">Категория действие элемента управления (учетная запись, данные, устройства, приложения, инфраструктуры).</span><span class="sxs-lookup"><span data-stu-id="25626-131">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="25626-132">actionType</span><span class="sxs-lookup"><span data-stu-id="25626-132">actionType</span></span>  |   <span data-ttu-id="25626-133">String</span><span class="sxs-lookup"><span data-stu-id="25626-133">String</span></span>  |   <span data-ttu-id="25626-134">Действие типа (Config, просмотр, поведение) элемента управления.</span><span class="sxs-lookup"><span data-stu-id="25626-134">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="25626-135">service</span><span class="sxs-lookup"><span data-stu-id="25626-135">service</span></span> |   <span data-ttu-id="25626-136">String</span><span class="sxs-lookup"><span data-stu-id="25626-136">String</span></span>  |   <span data-ttu-id="25626-137">Службы, которому принадлежит элемент управления (Exchange, Sharepoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="25626-137">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="25626-138">maxScore</span><span class="sxs-lookup"><span data-stu-id="25626-138">maxScore</span></span> |  <span data-ttu-id="25626-139">String</span><span class="sxs-lookup"><span data-stu-id="25626-139">String</span></span>  |   <span data-ttu-id="25626-140">Текущая платформа получить максимальный показатель на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="25626-140">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="25626-141">уровень</span><span class="sxs-lookup"><span data-stu-id="25626-141">tier</span></span> |  <span data-ttu-id="25626-142">String</span><span class="sxs-lookup"><span data-stu-id="25626-142">String</span></span>  |   <span data-ttu-id="25626-143">Уровень элемента управления (Core, защите подробно, Дополнительно.)</span><span class="sxs-lookup"><span data-stu-id="25626-143">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="25626-144">userImpact</span><span class="sxs-lookup"><span data-stu-id="25626-144">userImpact</span></span> |    <span data-ttu-id="25626-145">String</span><span class="sxs-lookup"><span data-stu-id="25626-145">String</span></span>  | <span data-ttu-id="25626-146">Влияние пользователей реализации управления (низкий, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="25626-146">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="25626-147">implementationCost</span><span class="sxs-lookup"><span data-stu-id="25626-147">implementationCost</span></span> |    <span data-ttu-id="25626-148">String</span><span class="sxs-lookup"><span data-stu-id="25626-148">String</span></span>  |   <span data-ttu-id="25626-149">Стоимость ресурса элемента управления implemmentating (низкий, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="25626-149">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="25626-150">rank</span><span class="sxs-lookup"><span data-stu-id="25626-150">rank</span></span> |  <span data-ttu-id="25626-151">Int32</span><span class="sxs-lookup"><span data-stu-id="25626-151">Int32</span></span>   |   <span data-ttu-id="25626-152">Стек корпорации Майкрософт ранжирования элемента управления.</span><span class="sxs-lookup"><span data-stu-id="25626-152">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="25626-153">угрозы безопасности</span><span class="sxs-lookup"><span data-stu-id="25626-153">threats</span></span> |   <span data-ttu-id="25626-154">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="25626-154">String Collection</span></span>   |   <span data-ttu-id="25626-155">Список управления устраняет угрозы (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, спуфинг).</span><span class="sxs-lookup"><span data-stu-id="25626-155">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="25626-156">устаревшие</span><span class="sxs-lookup"><span data-stu-id="25626-156">deprecated</span></span> |    <span data-ttu-id="25626-157">Логический</span><span class="sxs-lookup"><span data-stu-id="25626-157">Boolean</span></span> |   <span data-ttu-id="25626-158">Флаг, указывающий, если элемент управления амортизации.</span><span class="sxs-lookup"><span data-stu-id="25626-158">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="25626-159">исправление</span><span class="sxs-lookup"><span data-stu-id="25626-159">remediation</span></span> |   <span data-ttu-id="25626-160">String</span><span class="sxs-lookup"><span data-stu-id="25626-160">String</span></span>  |   <span data-ttu-id="25626-161">Описание элемента управления, какие представлены сведения о устранение.</span><span class="sxs-lookup"><span data-stu-id="25626-161">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="25626-162">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="25626-162">remediationImpact</span></span> | <span data-ttu-id="25626-163">String</span><span class="sxs-lookup"><span data-stu-id="25626-163">String</span></span>  |   <span data-ttu-id="25626-164">Описание влияния на пользователей исправлению.</span><span class="sxs-lookup"><span data-stu-id="25626-164">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="25626-165">actionUrl</span><span class="sxs-lookup"><span data-stu-id="25626-165">actionUrl</span></span> | <span data-ttu-id="25626-166">String</span><span class="sxs-lookup"><span data-stu-id="25626-166">String</span></span>  |   <span data-ttu-id="25626-167">URL-адрес, где элемент управления может быть actioned.</span><span class="sxs-lookup"><span data-stu-id="25626-167">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="25626-168">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="25626-168">controlStateUpdates</span></span> |   <span data-ttu-id="25626-169">String</span><span class="sxs-lookup"><span data-stu-id="25626-169">String</span></span>  |   <span data-ttu-id="25626-170">Флаг, указывающий, где клиент отметил элемента управления (игнорировать, сторонних анализа) (поддерживает [обновление](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="25626-170">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="25626-171">tenantNote</span><span class="sxs-lookup"><span data-stu-id="25626-171">tenantNote</span></span> |    <span data-ttu-id="25626-172">String</span><span class="sxs-lookup"><span data-stu-id="25626-172">String</span></span>  |   <span data-ttu-id="25626-173">Клиент может устанавливать каждого элемента управления комментариев (поддерживает [обновление](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="25626-173">Tenant can set per control comments (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="25626-174">assignedTo</span><span class="sxs-lookup"><span data-stu-id="25626-174">assignedTo</span></span> |    <span data-ttu-id="25626-175">String</span><span class="sxs-lookup"><span data-stu-id="25626-175">String</span></span>  |   <span data-ttu-id="25626-176">Клиента можно назначить элемент управления пользователю (поддерживает [обновление](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="25626-176">Tenant can assign the control to a individual (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="25626-177">updatedBy</span><span class="sxs-lookup"><span data-stu-id="25626-177">updatedBy</span></span> | <span data-ttu-id="25626-178">String</span><span class="sxs-lookup"><span data-stu-id="25626-178">String</span></span>  |   <span data-ttu-id="25626-179">Имя участника-пользователя для пользователей, которые внесены изменения состояния элемента управления.</span><span class="sxs-lookup"><span data-stu-id="25626-179">User principal name of who made changes to a control's state.</span></span> |

## <a name="relationships"></a><span data-ttu-id="25626-180">Связи</span><span class="sxs-lookup"><span data-stu-id="25626-180">Relationships</span></span>

<span data-ttu-id="25626-181">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="25626-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25626-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25626-182">JSON representation</span></span>

<span data-ttu-id="25626-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25626-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
}


```


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
