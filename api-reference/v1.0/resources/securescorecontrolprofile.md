---
title: Тип ресурса Секурескореконтролпрофиле
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 7ea9550e7fc6417ac28e32acd1d95cb9178f7360
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629259"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="14f95-104">Тип ресурса Секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="14f95-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="14f95-105">Представляет уровень безопасности клиента для данных элемента управления.</span><span class="sxs-lookup"><span data-stu-id="14f95-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="14f95-106">По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="14f95-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="14f95-107">Методы</span><span class="sxs-lookup"><span data-stu-id="14f95-107">Methods</span></span>

| <span data-ttu-id="14f95-108">Метод</span><span class="sxs-lookup"><span data-stu-id="14f95-108">Method</span></span>   | <span data-ttu-id="14f95-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="14f95-109">Return Type</span></span>|<span data-ttu-id="14f95-110">Описание</span><span class="sxs-lookup"><span data-stu-id="14f95-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="14f95-111">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="14f95-111">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="14f95-112">Секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="14f95-112">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="14f95-113">Чтение свойств и метаданных объекта Секурескореконтролпрофилес.</span><span class="sxs-lookup"><span data-stu-id="14f95-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="14f95-114">Получение Секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="14f95-114">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="14f95-115">секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="14f95-115">securescorecontrolprofile</span></span>](secureScoreControlProfile.md) |<span data-ttu-id="14f95-116">Чтение свойств и метаданных объекта Секурескореконтролпрофилес.</span><span class="sxs-lookup"><span data-stu-id="14f95-116">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="14f95-117">Обновление секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="14f95-117">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="14f95-118">секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="14f95-118">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="14f95-119">Обновление объекта секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="14f95-119">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="14f95-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="14f95-120">Properties</span></span>

|<span data-ttu-id="14f95-121">Имя</span><span class="sxs-lookup"><span data-stu-id="14f95-121">Name</span></span> |<span data-ttu-id="14f95-122">Тип</span><span class="sxs-lookup"><span data-stu-id="14f95-122">Type</span></span> |<span data-ttu-id="14f95-123">Описание</span><span class="sxs-lookup"><span data-stu-id="14f95-123">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="14f95-124">id</span><span class="sxs-lookup"><span data-stu-id="14f95-124">id</span></span>|<span data-ttu-id="14f95-125">String</span><span class="sxs-lookup"><span data-stu-id="14f95-125">String</span></span>|<span data-ttu-id="14f95-126">GUID или уникальный идентификатор, созданный поставщиком.</span><span class="sxs-lookup"><span data-stu-id="14f95-126">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="14f95-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14f95-127">Read-only.</span></span> <span data-ttu-id="14f95-128">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="14f95-128">Required.</span></span>|
|<span data-ttu-id="14f95-129">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="14f95-129">azureTenantId</span></span>|<span data-ttu-id="14f95-130">String</span><span class="sxs-lookup"><span data-stu-id="14f95-130">String</span></span>|<span data-ttu-id="14f95-131">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="14f95-131">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="14f95-132">actionType</span><span class="sxs-lookup"><span data-stu-id="14f95-132">actionType</span></span>|<span data-ttu-id="14f95-133">String</span><span class="sxs-lookup"><span data-stu-id="14f95-133">String</span></span>|<span data-ttu-id="14f95-134">Тип действия управления (config, проверка, поведение).</span><span class="sxs-lookup"><span data-stu-id="14f95-134">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="14f95-135">Актионурл</span><span class="sxs-lookup"><span data-stu-id="14f95-135">actionUrl</span></span>|<span data-ttu-id="14f95-136">String</span><span class="sxs-lookup"><span data-stu-id="14f95-136">String</span></span>|<span data-ttu-id="14f95-137">URL-адрес, по которому можно выполнить действия с элементом управления.</span><span class="sxs-lookup"><span data-stu-id="14f95-137">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="14f95-138">Контролкатегори</span><span class="sxs-lookup"><span data-stu-id="14f95-138">controlCategory</span></span>|<span data-ttu-id="14f95-139">String</span><span class="sxs-lookup"><span data-stu-id="14f95-139">String</span></span>|<span data-ttu-id="14f95-140">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="14f95-140">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="14f95-141">title</span><span class="sxs-lookup"><span data-stu-id="14f95-141">title</span></span>|<span data-ttu-id="14f95-142">Строка</span><span class="sxs-lookup"><span data-stu-id="14f95-142">String</span></span>|<span data-ttu-id="14f95-143">Название элемента управления.</span><span class="sxs-lookup"><span data-stu-id="14f95-143">Title of the control.</span></span>|
|<span data-ttu-id="14f95-144">устаревшие</span><span class="sxs-lookup"><span data-stu-id="14f95-144">deprecated</span></span>|<span data-ttu-id="14f95-145">Логический</span><span class="sxs-lookup"><span data-stu-id="14f95-145">Boolean</span></span>|<span data-ttu-id="14f95-146">Флаг, указывающий, является ли элемент управления амортизировано.</span><span class="sxs-lookup"><span data-stu-id="14f95-146">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="14f95-147">Имплементатионкост</span><span class="sxs-lookup"><span data-stu-id="14f95-147">implementationCost</span></span>|<span data-ttu-id="14f95-148">String</span><span class="sxs-lookup"><span data-stu-id="14f95-148">String</span></span>|<span data-ttu-id="14f95-149">Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая).</span><span class="sxs-lookup"><span data-stu-id="14f95-149">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="14f95-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14f95-150">lastModifiedDateTime</span></span>|<span data-ttu-id="14f95-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14f95-151">DateTimeOffset</span></span>|<span data-ttu-id="14f95-152">Время последнего изменения объекта профиля элемента управления.</span><span class="sxs-lookup"><span data-stu-id="14f95-152">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="14f95-153">Тип timestamp представляет дату и время</span><span class="sxs-lookup"><span data-stu-id="14f95-153">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="14f95-154">Максскоре</span><span class="sxs-lookup"><span data-stu-id="14f95-154">maxScore</span></span>|<span data-ttu-id="14f95-155">Двойное</span><span class="sxs-lookup"><span data-stu-id="14f95-155">Double</span></span>|<span data-ttu-id="14f95-156">максимальный достижимый показатель для элемента управления.</span><span class="sxs-lookup"><span data-stu-id="14f95-156">max attainable score for the control.</span></span>|
|<span data-ttu-id="14f95-157">rank</span><span class="sxs-lookup"><span data-stu-id="14f95-157">rank</span></span>|<span data-ttu-id="14f95-158">Int32</span><span class="sxs-lookup"><span data-stu-id="14f95-158">Int32</span></span>|<span data-ttu-id="14f95-159">Ранжирование стека для элемента управления корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="14f95-159">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="14f95-160">исправления</span><span class="sxs-lookup"><span data-stu-id="14f95-160">remediation</span></span>|<span data-ttu-id="14f95-161">String</span><span class="sxs-lookup"><span data-stu-id="14f95-161">String</span></span>|<span data-ttu-id="14f95-162">Описание того, что будет исправлено элементом управления.</span><span class="sxs-lookup"><span data-stu-id="14f95-162">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="14f95-163">Ремедиатионимпакт</span><span class="sxs-lookup"><span data-stu-id="14f95-163">remediationImpact</span></span>|<span data-ttu-id="14f95-164">String</span><span class="sxs-lookup"><span data-stu-id="14f95-164">String</span></span>|<span data-ttu-id="14f95-165">Описание влияния на пользователей об исправлении.</span><span class="sxs-lookup"><span data-stu-id="14f95-165">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="14f95-166">service</span><span class="sxs-lookup"><span data-stu-id="14f95-166">service</span></span>|<span data-ttu-id="14f95-167">String</span><span class="sxs-lookup"><span data-stu-id="14f95-167">String</span></span>|<span data-ttu-id="14f95-168">Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="14f95-168">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="14f95-169">угроз</span><span class="sxs-lookup"><span data-stu-id="14f95-169">threats</span></span>|<span data-ttu-id="14f95-170">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="14f95-170">String collection</span></span>|<span data-ttu-id="14f95-171">Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, удаление, Датаексфилтратион, удаление)</span><span class="sxs-lookup"><span data-stu-id="14f95-171">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="14f95-172">elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена).</span><span class="sxs-lookup"><span data-stu-id="14f95-172">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="14f95-173">медленно</span><span class="sxs-lookup"><span data-stu-id="14f95-173">tier</span></span>|<span data-ttu-id="14f95-174">String</span><span class="sxs-lookup"><span data-stu-id="14f95-174">String</span></span>|<span data-ttu-id="14f95-175">Уровень управления (ядро, Глубокая защита, расширенная)</span><span class="sxs-lookup"><span data-stu-id="14f95-175">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="14f95-176">Усеримпакт</span><span class="sxs-lookup"><span data-stu-id="14f95-176">userImpact</span></span>|<span data-ttu-id="14f95-177">String</span><span class="sxs-lookup"><span data-stu-id="14f95-177">String</span></span>|<span data-ttu-id="14f95-178">Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="14f95-178">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="14f95-179">Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="14f95-179">complianceInformation</span></span>|<span data-ttu-id="14f95-180">Коллекция [комплианцеинформатион](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="14f95-180">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="14f95-181">Коллекция сведений о соответствии, связанных с контролем безопасности по показателю</span><span class="sxs-lookup"><span data-stu-id="14f95-181">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="14f95-182">Контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="14f95-182">controlStateUpdates</span></span>|<span data-ttu-id="14f95-183">Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="14f95-183">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="14f95-184">Флаг, указывающий, где клиент пометил элемент управления (игнорируется, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofile-update.md)).</span><span class="sxs-lookup"><span data-stu-id="14f95-184">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="14f95-185">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="14f95-185">vendorInformation</span></span>|[<span data-ttu-id="14f95-186">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="14f95-186">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="14f95-187">Сложный тип, содержащий сведения о продукте, поставщике, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре).</span><span class="sxs-lookup"><span data-stu-id="14f95-187">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="14f95-188">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="14f95-188">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14f95-189">Связи</span><span class="sxs-lookup"><span data-stu-id="14f95-189">Relationships</span></span>

<span data-ttu-id="14f95-190">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="14f95-190">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14f95-191">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="14f95-191">JSON representation</span></span>

<span data-ttu-id="14f95-192">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14f95-192">The following is a JSON representation of the resource.</span></span>

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
