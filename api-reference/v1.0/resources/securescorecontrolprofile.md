---
title: Тип ресурса Секурескореконтролпрофиле
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0a643411ab75aa352e3c672f94f6e8259e931b6c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533769"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="8fbdc-104">Тип ресурса Секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="8fbdc-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="8fbdc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fbdc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8fbdc-106">Представляет уровень безопасности клиента для данных элемента управления.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-106">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="8fbdc-107">По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-107">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="8fbdc-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8fbdc-108">Methods</span></span>

| <span data-ttu-id="8fbdc-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8fbdc-109">Method</span></span>   | <span data-ttu-id="8fbdc-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8fbdc-110">Return Type</span></span>|<span data-ttu-id="8fbdc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8fbdc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8fbdc-112">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="8fbdc-112">List secureScoreControlProfiles</span></span>](../api/security-list-securescorecontrolprofiles.md) | [<span data-ttu-id="8fbdc-113">secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="8fbdc-113">secureScoreControlProfile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="8fbdc-114">Чтение свойств и метаданных объекта Секурескореконтролпрофилес.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-114">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="8fbdc-115">Получение объектов secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="8fbdc-115">Get secureScoreControlProfile</span></span>](../api/securescorecontrolprofile-get.md) | [<span data-ttu-id="8fbdc-116">секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="8fbdc-116">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="8fbdc-117">Чтение свойств и метаданных объекта Секурескореконтролпрофилес.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-117">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|
|[<span data-ttu-id="8fbdc-118">Обновление секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="8fbdc-118">Update securescorecontrolprofile</span></span>](../api/securescorecontrolprofile-update.md) | [<span data-ttu-id="8fbdc-119">секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="8fbdc-119">securescorecontrolprofile</span></span>](securescorecontrolprofile.md) |<span data-ttu-id="8fbdc-120">Обновление объекта секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-120">Update an securescorecontrolprofile object.</span></span> |


## <a name="properties"></a><span data-ttu-id="8fbdc-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fbdc-121">Properties</span></span>

|<span data-ttu-id="8fbdc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8fbdc-122">Name</span></span> |<span data-ttu-id="8fbdc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8fbdc-123">Type</span></span> |<span data-ttu-id="8fbdc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8fbdc-124">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="8fbdc-125">id</span><span class="sxs-lookup"><span data-stu-id="8fbdc-125">id</span></span>|<span data-ttu-id="8fbdc-126">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-126">String</span></span>|<span data-ttu-id="8fbdc-127">GUID или уникальный идентификатор, созданный поставщиком.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-127">Provider-generated GUID/unique identifier.</span></span> <span data-ttu-id="8fbdc-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-128">Read-only.</span></span> <span data-ttu-id="8fbdc-129">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-129">Required.</span></span>|
|<span data-ttu-id="8fbdc-130">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="8fbdc-130">azureTenantId</span></span>|<span data-ttu-id="8fbdc-131">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-131">String</span></span>|<span data-ttu-id="8fbdc-132">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-132">GUID string for tenant ID.</span></span>|
|<span data-ttu-id="8fbdc-133">actionType</span><span class="sxs-lookup"><span data-stu-id="8fbdc-133">actionType</span></span>|<span data-ttu-id="8fbdc-134">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-134">String</span></span>|<span data-ttu-id="8fbdc-135">Тип действия управления (config, проверка, поведение).</span><span class="sxs-lookup"><span data-stu-id="8fbdc-135">Control action type (Config, Review, Behavior).</span></span>|
|<span data-ttu-id="8fbdc-136">актионурл</span><span class="sxs-lookup"><span data-stu-id="8fbdc-136">actionUrl</span></span>|<span data-ttu-id="8fbdc-137">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-137">String</span></span>|<span data-ttu-id="8fbdc-138">URL-адрес, по которому можно выполнить действия с элементом управления.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-138">URL to where the control can be actioned.</span></span> |
|<span data-ttu-id="8fbdc-139">контролкатегори</span><span class="sxs-lookup"><span data-stu-id="8fbdc-139">controlCategory</span></span>|<span data-ttu-id="8fbdc-140">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-140">String</span></span>|<span data-ttu-id="8fbdc-141">Категория действий управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="8fbdc-141">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="8fbdc-142">title</span><span class="sxs-lookup"><span data-stu-id="8fbdc-142">title</span></span>|<span data-ttu-id="8fbdc-143">Строка</span><span class="sxs-lookup"><span data-stu-id="8fbdc-143">String</span></span>|<span data-ttu-id="8fbdc-144">Название элемента управления.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-144">Title of the control.</span></span>|
|<span data-ttu-id="8fbdc-145">устаревшие</span><span class="sxs-lookup"><span data-stu-id="8fbdc-145">deprecated</span></span>|<span data-ttu-id="8fbdc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fbdc-146">Boolean</span></span>|<span data-ttu-id="8fbdc-147">Флаг, указывающий, является ли элемент управления амортизировано.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-147">Flag to indicate if a control is depreciated.</span></span>|
|<span data-ttu-id="8fbdc-148">имплементатионкост</span><span class="sxs-lookup"><span data-stu-id="8fbdc-148">implementationCost</span></span>|<span data-ttu-id="8fbdc-149">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-149">String</span></span>|<span data-ttu-id="8fbdc-150">Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая).</span><span class="sxs-lookup"><span data-stu-id="8fbdc-150">Resource cost of implemmentating control (low, moderate, high).</span></span>|
|<span data-ttu-id="8fbdc-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fbdc-151">lastModifiedDateTime</span></span>|<span data-ttu-id="8fbdc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fbdc-152">DateTimeOffset</span></span>|<span data-ttu-id="8fbdc-153">Время последнего изменения объекта профиля элемента управления.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-153">Time at which the control profile entity was last modified.</span></span> <span data-ttu-id="8fbdc-154">Тип timestamp представляет дату и время</span><span class="sxs-lookup"><span data-stu-id="8fbdc-154">The Timestamp type represents date and time</span></span>| 
|<span data-ttu-id="8fbdc-155">максскоре</span><span class="sxs-lookup"><span data-stu-id="8fbdc-155">maxScore</span></span>|<span data-ttu-id="8fbdc-156">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8fbdc-156">Double</span></span>|<span data-ttu-id="8fbdc-157">максимальный достижимый показатель для элемента управления.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-157">max attainable score for the control.</span></span>|
|<span data-ttu-id="8fbdc-158">rank</span><span class="sxs-lookup"><span data-stu-id="8fbdc-158">rank</span></span>|<span data-ttu-id="8fbdc-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8fbdc-159">Int32</span></span>|<span data-ttu-id="8fbdc-160">Ранжирование стека для элемента управления корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-160">Microsoft's stack ranking of control.</span></span>|
|<span data-ttu-id="8fbdc-161">исправления</span><span class="sxs-lookup"><span data-stu-id="8fbdc-161">remediation</span></span>|<span data-ttu-id="8fbdc-162">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-162">String</span></span>|<span data-ttu-id="8fbdc-163">Описание того, что будет исправлено элементом управления.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-163">Description of what the control will help remediate.</span></span>|
|<span data-ttu-id="8fbdc-164">ремедиатионимпакт</span><span class="sxs-lookup"><span data-stu-id="8fbdc-164">remediationImpact</span></span>|<span data-ttu-id="8fbdc-165">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-165">String</span></span>|<span data-ttu-id="8fbdc-166">Описание влияния на пользователей об исправлении.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-166">Description of the impact on users of the remediation.</span></span>|
|<span data-ttu-id="8fbdc-167">service</span><span class="sxs-lookup"><span data-stu-id="8fbdc-167">service</span></span>|<span data-ttu-id="8fbdc-168">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-168">String</span></span>|<span data-ttu-id="8fbdc-169">Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8fbdc-169">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span>|
|<span data-ttu-id="8fbdc-170">угроз</span><span class="sxs-lookup"><span data-stu-id="8fbdc-170">threats</span></span>|<span data-ttu-id="8fbdc-171">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8fbdc-171">String collection</span></span>|<span data-ttu-id="8fbdc-172">Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, удаление, Датаексфилтратион, удаление)</span><span class="sxs-lookup"><span data-stu-id="8fbdc-172">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,</span></span>
<span data-ttu-id="8fbdc-173">elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена).</span><span class="sxs-lookup"><span data-stu-id="8fbdc-173">elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span>|
|<span data-ttu-id="8fbdc-174">медленно</span><span class="sxs-lookup"><span data-stu-id="8fbdc-174">tier</span></span>|<span data-ttu-id="8fbdc-175">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-175">String</span></span>|<span data-ttu-id="8fbdc-176">Уровень управления (ядро, Глубокая защита, расширенная)</span><span class="sxs-lookup"><span data-stu-id="8fbdc-176">Control tier (Core, Defense in Depth, Advanced.)</span></span>   |
|<span data-ttu-id="8fbdc-177">усеримпакт</span><span class="sxs-lookup"><span data-stu-id="8fbdc-177">userImpact</span></span>|<span data-ttu-id="8fbdc-178">String</span><span class="sxs-lookup"><span data-stu-id="8fbdc-178">String</span></span>|<span data-ttu-id="8fbdc-179">Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="8fbdc-179">User impact of implementing control (low, moderate, high).</span></span>   |
|<span data-ttu-id="8fbdc-180">комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="8fbdc-180">complianceInformation</span></span>|<span data-ttu-id="8fbdc-181">Коллекция [комплианцеинформатион](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="8fbdc-181">[complianceInformation](complianceinformation.md) collection</span></span>|<span data-ttu-id="8fbdc-182">Коллекция сведений о соответствии, связанных с контролем безопасности по показателю</span><span class="sxs-lookup"><span data-stu-id="8fbdc-182">The collection of compliance information associated with secure score control</span></span>|
|<span data-ttu-id="8fbdc-183">контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="8fbdc-183">controlStateUpdates</span></span>|<span data-ttu-id="8fbdc-184">Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="8fbdc-184">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span>|<span data-ttu-id="8fbdc-185">Флаг, указывающий, где клиент пометил элемент управления (игнорируется, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofile-update.md)).</span><span class="sxs-lookup"><span data-stu-id="8fbdc-185">Flag to indicate where the tenant has marked a control (ignored, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofile-update.md)).</span></span>|
|<span data-ttu-id="8fbdc-186">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="8fbdc-186">vendorInformation</span></span>|[<span data-ttu-id="8fbdc-187">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="8fbdc-187">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="8fbdc-188">Сложный тип, содержащий сведения о продукте, поставщике, поставщике и подобеспечении безопасности (например, Vendor = Microsoft; Provider = Секурескоре).</span><span class="sxs-lookup"><span data-stu-id="8fbdc-188">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=SecureScore).</span></span> <span data-ttu-id="8fbdc-189">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-189">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fbdc-190">Связи</span><span class="sxs-lookup"><span data-stu-id="8fbdc-190">Relationships</span></span>

<span data-ttu-id="8fbdc-191">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-191">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fbdc-192">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8fbdc-192">JSON representation</span></span>

<span data-ttu-id="8fbdc-193">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fbdc-193">The following is a JSON representation of the resource.</span></span>

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
