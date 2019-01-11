---
title: Тип ресурса secureScoreControlProfiles
description: Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.
localization_priority: Normal
ms.openlocfilehash: 866b2086ff5160744f848292cedf30c3cedf6daa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866222"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="8bdee-104">Тип ресурса secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8bdee-104">secureScoreControlProfiles resource type</span></span>

> <span data-ttu-id="8bdee-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8bdee-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bdee-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bdee-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8bdee-107">Представляет безопасной счета клиента в данные элемента управления.</span><span class="sxs-lookup"><span data-stu-id="8bdee-107">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="8bdee-108">По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.</span><span class="sxs-lookup"><span data-stu-id="8bdee-108">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="8bdee-109">Методы</span><span class="sxs-lookup"><span data-stu-id="8bdee-109">Methods</span></span>

| <span data-ttu-id="8bdee-110">Метод</span><span class="sxs-lookup"><span data-stu-id="8bdee-110">Method</span></span>   | <span data-ttu-id="8bdee-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8bdee-111">Return Type</span></span>|<span data-ttu-id="8bdee-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8bdee-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8bdee-113">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8bdee-113">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="8bdee-114">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8bdee-114">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="8bdee-115">Чтение свойства и метаданные объекта secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="8bdee-115">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="8bdee-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bdee-116">Properties</span></span>

|<span data-ttu-id="8bdee-117">Имя</span><span class="sxs-lookup"><span data-stu-id="8bdee-117">Name</span></span> |<span data-ttu-id="8bdee-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8bdee-118">Type</span></span> |<span data-ttu-id="8bdee-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8bdee-119">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="8bdee-120">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="8bdee-120">azureTenantId</span></span>   |   <span data-ttu-id="8bdee-121">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-121">String</span></span>  |   <span data-ttu-id="8bdee-122">Идентификатор GUID строки для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bdee-122">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="8bdee-123">ИмяЭлементаУправления</span><span class="sxs-lookup"><span data-stu-id="8bdee-123">controlName</span></span> |   <span data-ttu-id="8bdee-124">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-124">String</span></span>  |   <span data-ttu-id="8bdee-125">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="8bdee-125">Name of the control.</span></span> |
|   <span data-ttu-id="8bdee-126">title</span><span class="sxs-lookup"><span data-stu-id="8bdee-126">title</span></span>   |   <span data-ttu-id="8bdee-127">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-127">String</span></span>  |   <span data-ttu-id="8bdee-128">Заголовок элемента управления.</span><span class="sxs-lookup"><span data-stu-id="8bdee-128">Title of the control.</span></span>   |
| <span data-ttu-id="8bdee-129">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="8bdee-129">complianceInformation</span></span> | <span data-ttu-id="8bdee-130">[complianceInformation](complianceinformation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8bdee-130">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="8bdee-131">Коллекции данных соответствия требованиям, связанных с безопасного элемента управления счета</span><span class="sxs-lookup"><span data-stu-id="8bdee-131">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="8bdee-132">controlCategory</span><span class="sxs-lookup"><span data-stu-id="8bdee-132">controlCategory</span></span> |   <span data-ttu-id="8bdee-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-133">String</span></span>  |   <span data-ttu-id="8bdee-134">Категория действие элемента управления (учетная запись, данные, устройства, приложения, инфраструктуры).</span><span class="sxs-lookup"><span data-stu-id="8bdee-134">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="8bdee-135">actionType</span><span class="sxs-lookup"><span data-stu-id="8bdee-135">actionType</span></span>  |   <span data-ttu-id="8bdee-136">String</span><span class="sxs-lookup"><span data-stu-id="8bdee-136">String</span></span>  |   <span data-ttu-id="8bdee-137">Действие типа (Config, просмотр, поведение) элемента управления.</span><span class="sxs-lookup"><span data-stu-id="8bdee-137">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="8bdee-138">service</span><span class="sxs-lookup"><span data-stu-id="8bdee-138">service</span></span> |   <span data-ttu-id="8bdee-139">String</span><span class="sxs-lookup"><span data-stu-id="8bdee-139">String</span></span>  |   <span data-ttu-id="8bdee-140">Службы, которому принадлежит элемент управления (Exchange, Sharepoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8bdee-140">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="8bdee-141">maxScore</span><span class="sxs-lookup"><span data-stu-id="8bdee-141">maxScore</span></span> |  <span data-ttu-id="8bdee-142">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-142">String</span></span>  |   <span data-ttu-id="8bdee-143">Текущая платформа получить максимальный показатель на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="8bdee-143">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="8bdee-144">уровень</span><span class="sxs-lookup"><span data-stu-id="8bdee-144">tier</span></span> |  <span data-ttu-id="8bdee-145">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-145">String</span></span>  |   <span data-ttu-id="8bdee-146">Уровень элемента управления (Core, защите подробно, Дополнительно.)</span><span class="sxs-lookup"><span data-stu-id="8bdee-146">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="8bdee-147">userImpact</span><span class="sxs-lookup"><span data-stu-id="8bdee-147">userImpact</span></span> |    <span data-ttu-id="8bdee-148">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-148">String</span></span>  | <span data-ttu-id="8bdee-149">Влияние пользователей реализации управления (низкий, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="8bdee-149">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="8bdee-150">implementationCost</span><span class="sxs-lookup"><span data-stu-id="8bdee-150">implementationCost</span></span> |    <span data-ttu-id="8bdee-151">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-151">String</span></span>  |   <span data-ttu-id="8bdee-152">Стоимость ресурса элемента управления implemmentating (низкий, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="8bdee-152">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="8bdee-153">rank</span><span class="sxs-lookup"><span data-stu-id="8bdee-153">rank</span></span> |  <span data-ttu-id="8bdee-154">Int32</span><span class="sxs-lookup"><span data-stu-id="8bdee-154">Int32</span></span>   |   <span data-ttu-id="8bdee-155">Стек корпорации Майкрософт ранжирования элемента управления.</span><span class="sxs-lookup"><span data-stu-id="8bdee-155">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="8bdee-156">угрозы безопасности</span><span class="sxs-lookup"><span data-stu-id="8bdee-156">threats</span></span> |   <span data-ttu-id="8bdee-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8bdee-157">String Collection</span></span>   |   <span data-ttu-id="8bdee-158">Список управления устраняет угрозы (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, спуфинг).</span><span class="sxs-lookup"><span data-stu-id="8bdee-158">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="8bdee-159">устаревшие</span><span class="sxs-lookup"><span data-stu-id="8bdee-159">deprecated</span></span> |    <span data-ttu-id="8bdee-160">Логический</span><span class="sxs-lookup"><span data-stu-id="8bdee-160">Boolean</span></span> |   <span data-ttu-id="8bdee-161">Флаг, указывающий, если элемент управления амортизации.</span><span class="sxs-lookup"><span data-stu-id="8bdee-161">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="8bdee-162">исправление</span><span class="sxs-lookup"><span data-stu-id="8bdee-162">remediation</span></span> |   <span data-ttu-id="8bdee-163">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-163">String</span></span>  |   <span data-ttu-id="8bdee-164">Описание элемента управления, какие представлены сведения о устранение.</span><span class="sxs-lookup"><span data-stu-id="8bdee-164">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="8bdee-165">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="8bdee-165">remediationImpact</span></span> | <span data-ttu-id="8bdee-166">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-166">String</span></span>  |   <span data-ttu-id="8bdee-167">Описание влияния на пользователей исправлению.</span><span class="sxs-lookup"><span data-stu-id="8bdee-167">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="8bdee-168">actionUrl</span><span class="sxs-lookup"><span data-stu-id="8bdee-168">actionUrl</span></span> | <span data-ttu-id="8bdee-169">Строка</span><span class="sxs-lookup"><span data-stu-id="8bdee-169">String</span></span>  |   <span data-ttu-id="8bdee-170">URL-адрес, где элемент управления может быть actioned.</span><span class="sxs-lookup"><span data-stu-id="8bdee-170">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="8bdee-171">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="8bdee-171">controlStateUpdates</span></span> |   <span data-ttu-id="8bdee-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8bdee-172">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="8bdee-173">Флаг, указывающий, где клиент отметил элемента управления (игнорировать, сторонних анализа) (поддерживает [обновление](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="8bdee-173">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="8bdee-174">Связи</span><span class="sxs-lookup"><span data-stu-id="8bdee-174">Relationships</span></span>

<span data-ttu-id="8bdee-175">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8bdee-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bdee-176">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8bdee-176">JSON representation</span></span>

<span data-ttu-id="8bdee-177">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bdee-177">The following is a JSON representation of the resource.</span></span>

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
