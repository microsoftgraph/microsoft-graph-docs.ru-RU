---
title: Тип ресурса secureScoreControlProfiles
description: Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524431"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="516b8-104">Тип ресурса secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="516b8-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="516b8-105">Представляет безопасной счета клиента в данные элемента управления.</span><span class="sxs-lookup"><span data-stu-id="516b8-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="516b8-106">По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.</span><span class="sxs-lookup"><span data-stu-id="516b8-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="516b8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="516b8-107">Methods</span></span>

| <span data-ttu-id="516b8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="516b8-108">Method</span></span>   | <span data-ttu-id="516b8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="516b8-109">Return Type</span></span>|<span data-ttu-id="516b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="516b8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="516b8-111">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="516b8-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="516b8-112">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="516b8-112">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="516b8-113">Чтение свойства и метаданные объекта secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="516b8-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="516b8-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="516b8-114">Properties</span></span>

|<span data-ttu-id="516b8-115">Имя</span><span class="sxs-lookup"><span data-stu-id="516b8-115">Name</span></span> |<span data-ttu-id="516b8-116">Тип</span><span class="sxs-lookup"><span data-stu-id="516b8-116">Type</span></span> |<span data-ttu-id="516b8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="516b8-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="516b8-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="516b8-118">azureTenantId</span></span>   |   <span data-ttu-id="516b8-119">String</span><span class="sxs-lookup"><span data-stu-id="516b8-119">String</span></span>  |   <span data-ttu-id="516b8-120">Идентификатор GUID строки для клиента.</span><span class="sxs-lookup"><span data-stu-id="516b8-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="516b8-121">ИмяЭлементаУправления</span><span class="sxs-lookup"><span data-stu-id="516b8-121">controlName</span></span> |   <span data-ttu-id="516b8-122">String</span><span class="sxs-lookup"><span data-stu-id="516b8-122">String</span></span>  |   <span data-ttu-id="516b8-123">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="516b8-123">Name of the control.</span></span> |
|   <span data-ttu-id="516b8-124">title</span><span class="sxs-lookup"><span data-stu-id="516b8-124">title</span></span>   |   <span data-ttu-id="516b8-125">String</span><span class="sxs-lookup"><span data-stu-id="516b8-125">String</span></span>  |   <span data-ttu-id="516b8-126">Заголовок элемента управления.</span><span class="sxs-lookup"><span data-stu-id="516b8-126">Title of the control.</span></span>   |
| <span data-ttu-id="516b8-127">complianceInformation</span><span class="sxs-lookup"><span data-stu-id="516b8-127">complianceInformation</span></span> | <span data-ttu-id="516b8-128">[complianceInformation](complianceinformation.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="516b8-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="516b8-129">Коллекции данных соответствия требованиям, связанных с безопасного элемента управления счета</span><span class="sxs-lookup"><span data-stu-id="516b8-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="516b8-130">controlCategory</span><span class="sxs-lookup"><span data-stu-id="516b8-130">controlCategory</span></span> |   <span data-ttu-id="516b8-131">String</span><span class="sxs-lookup"><span data-stu-id="516b8-131">String</span></span>  |   <span data-ttu-id="516b8-132">Категория действие элемента управления (учетная запись, данные, устройства, приложения, инфраструктуры).</span><span class="sxs-lookup"><span data-stu-id="516b8-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="516b8-133">actionType</span><span class="sxs-lookup"><span data-stu-id="516b8-133">actionType</span></span>  |   <span data-ttu-id="516b8-134">String</span><span class="sxs-lookup"><span data-stu-id="516b8-134">String</span></span>  |   <span data-ttu-id="516b8-135">Действие типа (Config, просмотр, поведение) элемента управления.</span><span class="sxs-lookup"><span data-stu-id="516b8-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="516b8-136">service</span><span class="sxs-lookup"><span data-stu-id="516b8-136">service</span></span> |   <span data-ttu-id="516b8-137">String</span><span class="sxs-lookup"><span data-stu-id="516b8-137">String</span></span>  |   <span data-ttu-id="516b8-138">Службы, которому принадлежит элемент управления (Exchange, Sharepoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="516b8-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="516b8-139">maxScore</span><span class="sxs-lookup"><span data-stu-id="516b8-139">maxScore</span></span> |  <span data-ttu-id="516b8-140">String</span><span class="sxs-lookup"><span data-stu-id="516b8-140">String</span></span>  |   <span data-ttu-id="516b8-141">Текущая платформа получить максимальный показатель на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="516b8-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="516b8-142">Уровень</span><span class="sxs-lookup"><span data-stu-id="516b8-142">tier</span></span> |  <span data-ttu-id="516b8-143">String</span><span class="sxs-lookup"><span data-stu-id="516b8-143">String</span></span>  |   <span data-ttu-id="516b8-144">Уровень элемента управления (Core, защите подробно, Дополнительно.)</span><span class="sxs-lookup"><span data-stu-id="516b8-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="516b8-145">userImpact</span><span class="sxs-lookup"><span data-stu-id="516b8-145">userImpact</span></span> |    <span data-ttu-id="516b8-146">String</span><span class="sxs-lookup"><span data-stu-id="516b8-146">String</span></span>  | <span data-ttu-id="516b8-147">Влияние пользователей реализации управления (низкий, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="516b8-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="516b8-148">implementationCost</span><span class="sxs-lookup"><span data-stu-id="516b8-148">implementationCost</span></span> |    <span data-ttu-id="516b8-149">String</span><span class="sxs-lookup"><span data-stu-id="516b8-149">String</span></span>  |   <span data-ttu-id="516b8-150">Стоимость ресурса элемента управления implemmentating (низкий, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="516b8-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="516b8-151">rank</span><span class="sxs-lookup"><span data-stu-id="516b8-151">rank</span></span> |  <span data-ttu-id="516b8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="516b8-152">Int32</span></span>   |   <span data-ttu-id="516b8-153">Стек корпорации Майкрософт ранжирования элемента управления.</span><span class="sxs-lookup"><span data-stu-id="516b8-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="516b8-154">угрозы безопасности</span><span class="sxs-lookup"><span data-stu-id="516b8-154">threats</span></span> |   <span data-ttu-id="516b8-155">string collection</span><span class="sxs-lookup"><span data-stu-id="516b8-155">String Collection</span></span>   |   <span data-ttu-id="516b8-156">Список управления устраняет угрозы (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, спуфинг).</span><span class="sxs-lookup"><span data-stu-id="516b8-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="516b8-157">Нерекомендуемое</span><span class="sxs-lookup"><span data-stu-id="516b8-157">deprecated</span></span> |    <span data-ttu-id="516b8-158">Логическое</span><span class="sxs-lookup"><span data-stu-id="516b8-158">Boolean</span></span> |   <span data-ttu-id="516b8-159">Флаг, указывающий, если элемент управления амортизации.</span><span class="sxs-lookup"><span data-stu-id="516b8-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="516b8-160">исправление</span><span class="sxs-lookup"><span data-stu-id="516b8-160">remediation</span></span> |   <span data-ttu-id="516b8-161">String</span><span class="sxs-lookup"><span data-stu-id="516b8-161">String</span></span>  |   <span data-ttu-id="516b8-162">Описание элемента управления, какие представлены сведения о устранение.</span><span class="sxs-lookup"><span data-stu-id="516b8-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="516b8-163">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="516b8-163">remediationImpact</span></span> | <span data-ttu-id="516b8-164">String</span><span class="sxs-lookup"><span data-stu-id="516b8-164">String</span></span>  |   <span data-ttu-id="516b8-165">Описание влияния на пользователей исправлению.</span><span class="sxs-lookup"><span data-stu-id="516b8-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="516b8-166">ActionURL</span><span class="sxs-lookup"><span data-stu-id="516b8-166">actionUrl</span></span> | <span data-ttu-id="516b8-167">String</span><span class="sxs-lookup"><span data-stu-id="516b8-167">String</span></span>  |   <span data-ttu-id="516b8-168">URL-адрес, где элемент управления может быть actioned.</span><span class="sxs-lookup"><span data-stu-id="516b8-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="516b8-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="516b8-169">controlStateUpdates</span></span> |   <span data-ttu-id="516b8-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="516b8-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="516b8-171">Флаг, указывающий, где клиент отметил элемента управления (игнорировать, сторонних анализа) (поддерживает [обновление](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="516b8-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="516b8-172">Отношения</span><span class="sxs-lookup"><span data-stu-id="516b8-172">Relationships</span></span>

<span data-ttu-id="516b8-173">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="516b8-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="516b8-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="516b8-174">JSON representation</span></span>

<span data-ttu-id="516b8-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="516b8-175">The following is a JSON representation of the resource.</span></span>

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


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
