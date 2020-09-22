---
title: Тип ресурса Секурескореконтролпрофиле
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7af5b2ab614dae57ef7c18aee80133cd7a2096a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984070"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="4db8e-104">Тип ресурса Секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="4db8e-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="4db8e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4db8e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4db8e-106">Представляет уровень безопасности клиента для данных элемента управления.</span><span class="sxs-lookup"><span data-stu-id="4db8e-106">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="4db8e-107">По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="4db8e-107">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="4db8e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4db8e-108">Methods</span></span>

| <span data-ttu-id="4db8e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4db8e-109">Method</span></span>   | <span data-ttu-id="4db8e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4db8e-110">Return Type</span></span>|<span data-ttu-id="4db8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4db8e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4db8e-112">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="4db8e-112">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="4db8e-113">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="4db8e-113">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="4db8e-114">Чтение свойств и метаданных объекта Секурескореконтролпрофилес.</span><span class="sxs-lookup"><span data-stu-id="4db8e-114">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="4db8e-115">Получение объектов secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="4db8e-115">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="4db8e-116">секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="4db8e-116">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="4db8e-117">Чтение свойств и метаданных объекта Секурескореконтролпрофилес.</span><span class="sxs-lookup"><span data-stu-id="4db8e-117">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="4db8e-118">Обновление секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="4db8e-118">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="4db8e-119">секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="4db8e-119">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="4db8e-120">Обновление объекта секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="4db8e-120">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="4db8e-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="4db8e-121">Properties</span></span>

|<span data-ttu-id="4db8e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4db8e-122">Name</span></span> |<span data-ttu-id="4db8e-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4db8e-123">Type</span></span> |<span data-ttu-id="4db8e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4db8e-124">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="4db8e-125">id</span><span class="sxs-lookup"><span data-stu-id="4db8e-125">id</span></span>|<span data-ttu-id="4db8e-126">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-126">String</span></span>|<span data-ttu-id="4db8e-127">GUID или уникальный идентификатор, созданный поставщиком.</span><span class="sxs-lookup"><span data-stu-id="4db8e-127">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="4db8e-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4db8e-128">Read-only.</span></span> <span data-ttu-id="4db8e-129">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="4db8e-129">Required.</span></span>|
|<span data-ttu-id="4db8e-130">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="4db8e-130">azureTenantId</span></span>|<span data-ttu-id="4db8e-131">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-131">String</span></span>|<span data-ttu-id="4db8e-132">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="4db8e-132">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="4db8e-133">actionType</span><span class="sxs-lookup"><span data-stu-id="4db8e-133">actionType</span></span>|<span data-ttu-id="4db8e-134">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-134">String</span></span>|<span data-ttu-id="4db8e-135">Тип действия управления (config, проверка, поведение).</span><span class="sxs-lookup"><span data-stu-id="4db8e-135">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="4db8e-136">актионурл</span><span class="sxs-lookup"><span data-stu-id="4db8e-136">actionUrl</span></span>|<span data-ttu-id="4db8e-137">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-137">String</span></span>|<span data-ttu-id="4db8e-138">URL-адрес, по которому можно выполнить действия с элементом управления.</span><span class="sxs-lookup"><span data-stu-id="4db8e-138">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="4db8e-139">контролкатегори</span><span class="sxs-lookup"><span data-stu-id="4db8e-139">controlCategory</span></span>|<span data-ttu-id="4db8e-140">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-140">String</span></span>|<span data-ttu-id="4db8e-141">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="4db8e-141">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="4db8e-142">title</span><span class="sxs-lookup"><span data-stu-id="4db8e-142">title</span></span>|<span data-ttu-id="4db8e-143">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-143">String</span></span>|<span data-ttu-id="4db8e-144">Название элемента управления.</span><span class="sxs-lookup"><span data-stu-id="4db8e-144">Title of the control.</span></span>|
|<span data-ttu-id="4db8e-145">устаревшие</span><span class="sxs-lookup"><span data-stu-id="4db8e-145">deprecated</span></span>|<span data-ttu-id="4db8e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db8e-146">Boolean</span></span>|<span data-ttu-id="4db8e-147">Флаг, указывающий, является ли элемент управления амортизировано.</span><span class="sxs-lookup"><span data-stu-id="4db8e-147">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="4db8e-148">имплементатионкост</span><span class="sxs-lookup"><span data-stu-id="4db8e-148">implementationCost</span></span>|<span data-ttu-id="4db8e-149">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-149">String</span></span>|<span data-ttu-id="4db8e-150">Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая).</span><span class="sxs-lookup"><span data-stu-id="4db8e-150">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="4db8e-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4db8e-151">lastModifiedDateTime</span></span>|<span data-ttu-id="4db8e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4db8e-152">DateTimeOffset</span></span>|<span data-ttu-id="4db8e-153">Время последнего изменения объекта профиля элемента управления.</span><span class="sxs-lookup"><span data-stu-id="4db8e-153">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="4db8e-154">Тип timestamp представляет дату и время</span><span class="sxs-lookup"><span data-stu-id="4db8e-154">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="4db8e-155">максскоре</span><span class="sxs-lookup"><span data-stu-id="4db8e-155">maxScore</span></span>|<span data-ttu-id="4db8e-156">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4db8e-156">Double</span></span>|<span data-ttu-id="4db8e-157">максимальный достижимый показатель для элемента управления.</span><span class="sxs-lookup"><span data-stu-id="4db8e-157">max attainable score for the control.</span></span>|
|<span data-ttu-id="4db8e-158">rank</span><span class="sxs-lookup"><span data-stu-id="4db8e-158">rank</span></span>|<span data-ttu-id="4db8e-159">Int32</span><span class="sxs-lookup"><span data-stu-id="4db8e-159">Int32</span></span>|<span data-ttu-id="4db8e-160">Ранжирование стека для элемента управления корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="4db8e-160">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="4db8e-161">исправления</span><span class="sxs-lookup"><span data-stu-id="4db8e-161">remediation</span></span>|<span data-ttu-id="4db8e-162">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-162">String</span></span>|<span data-ttu-id="4db8e-163">Описание того, что будет исправлено элементом управления.</span><span class="sxs-lookup"><span data-stu-id="4db8e-163">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="4db8e-164">ремедиатионимпакт</span><span class="sxs-lookup"><span data-stu-id="4db8e-164">remediationImpact</span></span>|<span data-ttu-id="4db8e-165">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-165">String</span></span>|<span data-ttu-id="4db8e-166">Описание влияния на пользователей об исправлении.</span><span class="sxs-lookup"><span data-stu-id="4db8e-166">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="4db8e-167">service</span><span class="sxs-lookup"><span data-stu-id="4db8e-167">service</span></span>|<span data-ttu-id="4db8e-168">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-168">String</span></span>|<span data-ttu-id="4db8e-169">Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="4db8e-169">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="4db8e-170">угроз</span><span class="sxs-lookup"><span data-stu-id="4db8e-170">threats</span></span>|<span data-ttu-id="4db8e-171">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4db8e-171">String collection</span></span>|<span data-ttu-id="4db8e-172">Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, удаление, Датаексфилтратион, удаление)</span><span class="sxs-lookup"><span data-stu-id="4db8e-172">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="4db8e-173">elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена).</span><span class="sxs-lookup"><span data-stu-id="4db8e-173">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="4db8e-174">медленно</span><span class="sxs-lookup"><span data-stu-id="4db8e-174">tier</span></span>|<span data-ttu-id="4db8e-175">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-175">String</span></span>|<span data-ttu-id="4db8e-176">Уровень управления (ядро, Глубокая защита, расширенная)</span><span class="sxs-lookup"><span data-stu-id="4db8e-176">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="4db8e-177">усеримпакт</span><span class="sxs-lookup"><span data-stu-id="4db8e-177">userImpact</span></span>|<span data-ttu-id="4db8e-178">String</span><span class="sxs-lookup"><span data-stu-id="4db8e-178">String</span></span>|<span data-ttu-id="4db8e-179">Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="4db8e-179">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="4db8e-180">комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="4db8e-180">complianceInformation</span></span>|<span data-ttu-id="4db8e-181">Коллекция [комплианцеинформатион](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="4db8e-181">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="4db8e-182">Коллекция сведений о соответствии, связанных с контролем безопасности по показателю</span><span class="sxs-lookup"><span data-stu-id="4db8e-182">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="4db8e-183">контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="4db8e-183">controlStateUpdates</span></span>|<span data-ttu-id="4db8e-184">Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="4db8e-184">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="4db8e-185">Флаг, указывающий, где клиент пометил элемент управления (игнорируется, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofile-update.md)).</span><span class="sxs-lookup"><span data-stu-id="4db8e-185">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="4db8e-186">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="4db8e-186">vendorInformation</span></span>|[<span data-ttu-id="4db8e-187">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="4db8e-187">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="4db8e-188">Сложный тип, содержащий сведения о продукте, поставщике, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре).</span><span class="sxs-lookup"><span data-stu-id="4db8e-188">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="4db8e-189">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4db8e-189">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4db8e-190">Связи</span><span class="sxs-lookup"><span data-stu-id="4db8e-190">Relationships</span></span>

<span data-ttu-id="4db8e-191">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4db8e-191">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4db8e-192">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4db8e-192">JSON representation</span></span>

<span data-ttu-id="4db8e-193">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4db8e-193">The following is a JSON representation of the resource.</span></span>

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

