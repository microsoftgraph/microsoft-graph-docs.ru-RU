---
title: Тип ресурса Секурескореконтролпрофиле
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 40bee951d3030772973911510ebba7cc90f412ae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034491"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="d10d5-104">Тип ресурса Секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="d10d5-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="d10d5-105">Представляет уровень безопасности клиента для данных элемента управления.</span><span class="sxs-lookup"><span data-stu-id="d10d5-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="d10d5-106">По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="d10d5-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="d10d5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d10d5-107">Methods</span></span>

| <span data-ttu-id="d10d5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d10d5-108">Method</span></span>   | <span data-ttu-id="d10d5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d10d5-109">Return Type</span></span>|<span data-ttu-id="d10d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d10d5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d10d5-111">Список объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="d10d5-111">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="d10d5-112">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="d10d5-112">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="d10d5-113">Чтение свойств и метаданных объекта Секурескореконтролпрофилес.</span><span class="sxs-lookup"><span data-stu-id="d10d5-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="d10d5-114">Получение объектов secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="d10d5-114">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="d10d5-115">секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="d10d5-115">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="d10d5-116">Чтение свойств и метаданных объекта Секурескореконтролпрофилес.</span><span class="sxs-lookup"><span data-stu-id="d10d5-116">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="d10d5-117">Обновление секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="d10d5-117">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="d10d5-118">секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="d10d5-118">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="d10d5-119">Обновление объекта секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="d10d5-119">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="d10d5-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="d10d5-120">Properties</span></span>

|<span data-ttu-id="d10d5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d10d5-121">Name</span></span> |<span data-ttu-id="d10d5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d10d5-122">Type</span></span> |<span data-ttu-id="d10d5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d10d5-123">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="d10d5-124">id</span><span class="sxs-lookup"><span data-stu-id="d10d5-124">id</span></span>|<span data-ttu-id="d10d5-125">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-125">String</span></span>|<span data-ttu-id="d10d5-126">GUID или уникальный идентификатор, созданный поставщиком.</span><span class="sxs-lookup"><span data-stu-id="d10d5-126">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="d10d5-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d10d5-127">Read-only.</span></span> <span data-ttu-id="d10d5-128">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="d10d5-128">Required.</span></span>|
|<span data-ttu-id="d10d5-129">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="d10d5-129">azureTenantId</span></span>|<span data-ttu-id="d10d5-130">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-130">String</span></span>|<span data-ttu-id="d10d5-131">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="d10d5-131">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="d10d5-132">actionType</span><span class="sxs-lookup"><span data-stu-id="d10d5-132">actionType</span></span>|<span data-ttu-id="d10d5-133">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-133">String</span></span>|<span data-ttu-id="d10d5-134">Тип действия управления (config, проверка, поведение).</span><span class="sxs-lookup"><span data-stu-id="d10d5-134">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="d10d5-135">Актионурл</span><span class="sxs-lookup"><span data-stu-id="d10d5-135">actionUrl</span></span>|<span data-ttu-id="d10d5-136">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-136">String</span></span>|<span data-ttu-id="d10d5-137">URL-адрес, по которому можно выполнить действия с элементом управления.</span><span class="sxs-lookup"><span data-stu-id="d10d5-137">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="d10d5-138">Контролкатегори</span><span class="sxs-lookup"><span data-stu-id="d10d5-138">controlCategory</span></span>|<span data-ttu-id="d10d5-139">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-139">String</span></span>|<span data-ttu-id="d10d5-140">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="d10d5-140">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="d10d5-141">title</span><span class="sxs-lookup"><span data-stu-id="d10d5-141">title</span></span>|<span data-ttu-id="d10d5-142">Строка</span><span class="sxs-lookup"><span data-stu-id="d10d5-142">String</span></span>|<span data-ttu-id="d10d5-143">Название элемента управления.</span><span class="sxs-lookup"><span data-stu-id="d10d5-143">Title of the control.</span></span>|
|<span data-ttu-id="d10d5-144">устаревшие</span><span class="sxs-lookup"><span data-stu-id="d10d5-144">deprecated</span></span>|<span data-ttu-id="d10d5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d10d5-145">Boolean</span></span>|<span data-ttu-id="d10d5-146">Флаг, указывающий, является ли элемент управления амортизировано.</span><span class="sxs-lookup"><span data-stu-id="d10d5-146">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="d10d5-147">Имплементатионкост</span><span class="sxs-lookup"><span data-stu-id="d10d5-147">implementationCost</span></span>|<span data-ttu-id="d10d5-148">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-148">String</span></span>|<span data-ttu-id="d10d5-149">Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая).</span><span class="sxs-lookup"><span data-stu-id="d10d5-149">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="d10d5-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d10d5-150">lastModifiedDateTime</span></span>|<span data-ttu-id="d10d5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d10d5-151">DateTimeOffset</span></span>|<span data-ttu-id="d10d5-152">Время последнего изменения объекта профиля элемента управления.</span><span class="sxs-lookup"><span data-stu-id="d10d5-152">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="d10d5-153">Тип timestamp представляет дату и время</span><span class="sxs-lookup"><span data-stu-id="d10d5-153">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="d10d5-154">Максскоре</span><span class="sxs-lookup"><span data-stu-id="d10d5-154">maxScore</span></span>|<span data-ttu-id="d10d5-155">Двойное</span><span class="sxs-lookup"><span data-stu-id="d10d5-155">Double</span></span>|<span data-ttu-id="d10d5-156">максимальный достижимый показатель для элемента управления.</span><span class="sxs-lookup"><span data-stu-id="d10d5-156">max attainable score for the control.</span></span>|
|<span data-ttu-id="d10d5-157">rank</span><span class="sxs-lookup"><span data-stu-id="d10d5-157">rank</span></span>|<span data-ttu-id="d10d5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d10d5-158">Int32</span></span>|<span data-ttu-id="d10d5-159">Ранжирование стека для элемента управления корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d10d5-159">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="d10d5-160">исправления</span><span class="sxs-lookup"><span data-stu-id="d10d5-160">remediation</span></span>|<span data-ttu-id="d10d5-161">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-161">String</span></span>|<span data-ttu-id="d10d5-162">Описание того, что будет исправлено элементом управления.</span><span class="sxs-lookup"><span data-stu-id="d10d5-162">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="d10d5-163">Ремедиатионимпакт</span><span class="sxs-lookup"><span data-stu-id="d10d5-163">remediationImpact</span></span>|<span data-ttu-id="d10d5-164">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-164">String</span></span>|<span data-ttu-id="d10d5-165">Описание влияния на пользователей об исправлении.</span><span class="sxs-lookup"><span data-stu-id="d10d5-165">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="d10d5-166">service</span><span class="sxs-lookup"><span data-stu-id="d10d5-166">service</span></span>|<span data-ttu-id="d10d5-167">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-167">String</span></span>|<span data-ttu-id="d10d5-168">Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="d10d5-168">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="d10d5-169">угроз</span><span class="sxs-lookup"><span data-stu-id="d10d5-169">threats</span></span>|<span data-ttu-id="d10d5-170">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d10d5-170">String collection</span></span>|<span data-ttu-id="d10d5-171">Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, удаление, Датаексфилтратион, удаление)</span><span class="sxs-lookup"><span data-stu-id="d10d5-171">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="d10d5-172">elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена).</span><span class="sxs-lookup"><span data-stu-id="d10d5-172">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="d10d5-173">медленно</span><span class="sxs-lookup"><span data-stu-id="d10d5-173">tier</span></span>|<span data-ttu-id="d10d5-174">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-174">String</span></span>|<span data-ttu-id="d10d5-175">Уровень управления (ядро, Глубокая защита, расширенная)</span><span class="sxs-lookup"><span data-stu-id="d10d5-175">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="d10d5-176">Усеримпакт</span><span class="sxs-lookup"><span data-stu-id="d10d5-176">userImpact</span></span>|<span data-ttu-id="d10d5-177">String</span><span class="sxs-lookup"><span data-stu-id="d10d5-177">String</span></span>|<span data-ttu-id="d10d5-178">Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="d10d5-178">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="d10d5-179">Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="d10d5-179">complianceInformation</span></span>|<span data-ttu-id="d10d5-180">Коллекция [комплианцеинформатион](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="d10d5-180">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="d10d5-181">Коллекция сведений о соответствии, связанных с контролем безопасности по показателю</span><span class="sxs-lookup"><span data-stu-id="d10d5-181">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="d10d5-182">Контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="d10d5-182">controlStateUpdates</span></span>|<span data-ttu-id="d10d5-183">Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="d10d5-183">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="d10d5-184">Флаг, указывающий, где клиент пометил элемент управления (игнорируется, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofile-update.md)).</span><span class="sxs-lookup"><span data-stu-id="d10d5-184">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="d10d5-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="d10d5-185">vendorInformation</span></span>|[<span data-ttu-id="d10d5-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="d10d5-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="d10d5-187">Сложный тип, содержащий сведения о продукте, поставщике, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре).</span><span class="sxs-lookup"><span data-stu-id="d10d5-187">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="d10d5-188">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d10d5-188">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d10d5-189">Отношения</span><span class="sxs-lookup"><span data-stu-id="d10d5-189">Relationships</span></span>

<span data-ttu-id="d10d5-190">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d10d5-190">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d10d5-191">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d10d5-191">JSON representation</span></span>

<span data-ttu-id="d10d5-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d10d5-192">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "id": "String (identifier)",
  "azureTenantId": "String",
  "actionType": "String",
  "actionUrl": "String",
  "controlCategory": "String",
  "title": "String", 
  "deprecated": "Boolean",
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": "Int32",
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": ["String"],
  "tier": "String",
  "userImpact": "String",
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}], 
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
