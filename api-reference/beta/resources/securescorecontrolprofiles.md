---
title: Тип ресурса secureScoreControlProfiles
description: Представляет безопасной счета клиента в данные элемента управления. По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576061"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="32d60-104">Тип ресурса secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="32d60-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32d60-105">Представляет безопасной счета клиента в данные элемента управления.</span><span class="sxs-lookup"><span data-stu-id="32d60-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="32d60-106">По умолчанию он возвращает все элементы управления для клиента, а можно явно по запросу отдельных элементов управления.</span><span class="sxs-lookup"><span data-stu-id="32d60-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="32d60-107">Методы</span><span class="sxs-lookup"><span data-stu-id="32d60-107">Methods</span></span>

| <span data-ttu-id="32d60-108">Метод</span><span class="sxs-lookup"><span data-stu-id="32d60-108">Method</span></span>   | <span data-ttu-id="32d60-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="32d60-109">Return Type</span></span>|<span data-ttu-id="32d60-110">Описание</span><span class="sxs-lookup"><span data-stu-id="32d60-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32d60-111">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="32d60-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="32d60-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="32d60-112">secureScoreControlProfile</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="32d60-113">Чтение свойства и метаданные объекта secureScoreControlProfiles.</span><span class="sxs-lookup"><span data-stu-id="32d60-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="32d60-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="32d60-114">Properties</span></span>

|<span data-ttu-id="32d60-115">Имя</span><span class="sxs-lookup"><span data-stu-id="32d60-115">Name</span></span> |<span data-ttu-id="32d60-116">Тип</span><span class="sxs-lookup"><span data-stu-id="32d60-116">Type</span></span> |<span data-ttu-id="32d60-117">Описание</span><span class="sxs-lookup"><span data-stu-id="32d60-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="32d60-118">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="32d60-118">azureTenantId</span></span>   |   <span data-ttu-id="32d60-119">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-119">String</span></span>  |   <span data-ttu-id="32d60-120">Идентификатор GUID строки для клиента.</span><span class="sxs-lookup"><span data-stu-id="32d60-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="32d60-121">ИмяЭлементаУправления</span><span class="sxs-lookup"><span data-stu-id="32d60-121">controlName</span></span> |   <span data-ttu-id="32d60-122">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-122">String</span></span>  |   <span data-ttu-id="32d60-123">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="32d60-123">Name of the control.</span></span> |
|   <span data-ttu-id="32d60-124">title</span><span class="sxs-lookup"><span data-stu-id="32d60-124">title</span></span>   |   <span data-ttu-id="32d60-125">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-125">String</span></span>  |   <span data-ttu-id="32d60-126">Заголовок элемента управления.</span><span class="sxs-lookup"><span data-stu-id="32d60-126">Title of the control.</span></span>   |
|   <span data-ttu-id="32d60-127">controlCategory</span><span class="sxs-lookup"><span data-stu-id="32d60-127">controlCategory</span></span> |   <span data-ttu-id="32d60-128">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-128">String</span></span>  |   <span data-ttu-id="32d60-129">Категория действие элемента управления (учетная запись, данные, устройства, приложения, инфраструктуры).</span><span class="sxs-lookup"><span data-stu-id="32d60-129">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="32d60-130">actionType</span><span class="sxs-lookup"><span data-stu-id="32d60-130">actionType</span></span>  |   <span data-ttu-id="32d60-131">String</span><span class="sxs-lookup"><span data-stu-id="32d60-131">String</span></span>  |   <span data-ttu-id="32d60-132">Действие типа (Config, просмотр, поведение) элемента управления.</span><span class="sxs-lookup"><span data-stu-id="32d60-132">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="32d60-133">service</span><span class="sxs-lookup"><span data-stu-id="32d60-133">service</span></span> |   <span data-ttu-id="32d60-134">String</span><span class="sxs-lookup"><span data-stu-id="32d60-134">String</span></span>  |   <span data-ttu-id="32d60-135">Службы, которому принадлежит элемент управления (Exchange, Sharepoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="32d60-135">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="32d60-136">maxScore</span><span class="sxs-lookup"><span data-stu-id="32d60-136">maxScore</span></span> |  <span data-ttu-id="32d60-137">Double</span><span class="sxs-lookup"><span data-stu-id="32d60-137">Double</span></span>  |   <span data-ttu-id="32d60-138">Текущая платформа получить максимальный показатель на указанной даты.</span><span class="sxs-lookup"><span data-stu-id="32d60-138">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="32d60-139">уровень</span><span class="sxs-lookup"><span data-stu-id="32d60-139">tier</span></span> |  <span data-ttu-id="32d60-140">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-140">String</span></span>  |   <span data-ttu-id="32d60-141">Уровень элемента управления (Core, защите подробно, Дополнительно.)</span><span class="sxs-lookup"><span data-stu-id="32d60-141">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="32d60-142">userImpact</span><span class="sxs-lookup"><span data-stu-id="32d60-142">userImpact</span></span> |    <span data-ttu-id="32d60-143">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-143">String</span></span>  | <span data-ttu-id="32d60-144">Влияние пользователей реализации управления (низкий, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="32d60-144">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="32d60-145">implementationCost</span><span class="sxs-lookup"><span data-stu-id="32d60-145">implementationCost</span></span> |    <span data-ttu-id="32d60-146">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-146">String</span></span>  |   <span data-ttu-id="32d60-147">Стоимость ресурса элемента управления implemmentating (низкий, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="32d60-147">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="32d60-148">rank</span><span class="sxs-lookup"><span data-stu-id="32d60-148">rank</span></span> |  <span data-ttu-id="32d60-149">Int32</span><span class="sxs-lookup"><span data-stu-id="32d60-149">Int32</span></span>   |   <span data-ttu-id="32d60-150">Стек корпорации Майкрософт ранжирования элемента управления.</span><span class="sxs-lookup"><span data-stu-id="32d60-150">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="32d60-151">угрозы безопасности</span><span class="sxs-lookup"><span data-stu-id="32d60-151">threats</span></span> |   <span data-ttu-id="32d60-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="32d60-152">String Collection</span></span>   |   <span data-ttu-id="32d60-153">Список управления устраняет угрозы (accountBreach, dataDeletion, dataExfiltration, dataSpillage, elevationOfPrivilege, maliciousInsider, passwordCracking, phishingOrWhaling, спуфинг).</span><span class="sxs-lookup"><span data-stu-id="32d60-153">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="32d60-154">устаревшие</span><span class="sxs-lookup"><span data-stu-id="32d60-154">deprecated</span></span> |    <span data-ttu-id="32d60-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="32d60-155">Boolean</span></span> |   <span data-ttu-id="32d60-156">Флаг, указывающий, если элемент управления амортизации.</span><span class="sxs-lookup"><span data-stu-id="32d60-156">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="32d60-157">исправление</span><span class="sxs-lookup"><span data-stu-id="32d60-157">remediation</span></span> |   <span data-ttu-id="32d60-158">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-158">String</span></span>  |   <span data-ttu-id="32d60-159">Описание элемента управления, какие представлены сведения о устранение.</span><span class="sxs-lookup"><span data-stu-id="32d60-159">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="32d60-160">remediationImpact</span><span class="sxs-lookup"><span data-stu-id="32d60-160">remediationImpact</span></span> | <span data-ttu-id="32d60-161">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-161">String</span></span>  |   <span data-ttu-id="32d60-162">Описание влияния на пользователей исправлению.</span><span class="sxs-lookup"><span data-stu-id="32d60-162">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="32d60-163">actionUrl</span><span class="sxs-lookup"><span data-stu-id="32d60-163">actionUrl</span></span> | <span data-ttu-id="32d60-164">Строка</span><span class="sxs-lookup"><span data-stu-id="32d60-164">String</span></span>  |   <span data-ttu-id="32d60-165">URL-адрес, где элемент управления может быть actioned.</span><span class="sxs-lookup"><span data-stu-id="32d60-165">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="32d60-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32d60-166">lastModifiedDateTime</span></span> |  <span data-ttu-id="32d60-167">String (DateTimeOffset)</span><span class="sxs-lookup"><span data-stu-id="32d60-167">String (DateTimeOffset)</span></span> |   <span data-ttu-id="32d60-168">Дата последнего изменения</span><span class="sxs-lookup"><span data-stu-id="32d60-168">Date last modified</span></span> |
|   <span data-ttu-id="32d60-169">controlStateUpdates</span><span class="sxs-lookup"><span data-stu-id="32d60-169">controlStateUpdates</span></span> |   <span data-ttu-id="32d60-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="32d60-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |  <span data-ttu-id="32d60-171">Флаг, указывающий, где клиент отметил элемента управления (игнорировать, сторонних анализа) (поддерживает [обновление](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="32d60-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="32d60-172">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="32d60-172">vendorInformation</span></span> | [<span data-ttu-id="32d60-173">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="32d60-173">securityVendorInformation</span></span>](securityvendorinformation.md) | <span data-ttu-id="32d60-174">Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="32d60-174">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="32d60-175">Связи</span><span class="sxs-lookup"><span data-stu-id="32d60-175">Relationships</span></span>

<span data-ttu-id="32d60-176">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="32d60-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="32d60-177">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="32d60-177">JSON representation</span></span>

<span data-ttu-id="32d60-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32d60-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
    "title": "String", 
    "azureTenantId": "String (identifier)", 
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
