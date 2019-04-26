---
title: Тип ресурса Секурескореконтролпрофиле
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
ms.openlocfilehash: 41a74af0de47bbe77b8ea04cbea011a6f085d1bb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343413"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="c98a9-104">Тип ресурса Секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="c98a9-104">secureScoreControlProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c98a9-105">Представляет уровень безопасности клиента для данных элемента управления.</span><span class="sxs-lookup"><span data-stu-id="c98a9-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="c98a9-106">По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="c98a9-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="c98a9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c98a9-107">Methods</span></span>

| <span data-ttu-id="c98a9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c98a9-108">Method</span></span>   | <span data-ttu-id="c98a9-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c98a9-109">Return Type</span></span>|<span data-ttu-id="c98a9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c98a9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c98a9-111">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="c98a9-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | <span data-ttu-id="c98a9-112">Коллекция [секурескореконтролпрофиле](securescorecontrolprofiles.md)</span><span class="sxs-lookup"><span data-stu-id="c98a9-112">[secureScoreControlProfile](securescorecontrolprofiles.md) collection</span></span> |<span data-ttu-id="c98a9-113">Получение коллекции объектов Секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="c98a9-113">Get a collection of secureScoreControlProfile objects.</span></span>|


## <a name="properties"></a><span data-ttu-id="c98a9-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="c98a9-114">Properties</span></span>

|<span data-ttu-id="c98a9-115">Имя</span><span class="sxs-lookup"><span data-stu-id="c98a9-115">Name</span></span> |<span data-ttu-id="c98a9-116">Тип</span><span class="sxs-lookup"><span data-stu-id="c98a9-116">Type</span></span> |<span data-ttu-id="c98a9-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c98a9-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="c98a9-118">Азуретенантид</span><span class="sxs-lookup"><span data-stu-id="c98a9-118">azureTenantId</span></span>   |   <span data-ttu-id="c98a9-119">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-119">String</span></span>  |   <span data-ttu-id="c98a9-120">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="c98a9-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="c98a9-121">Контролнаме</span><span class="sxs-lookup"><span data-stu-id="c98a9-121">controlName</span></span> |   <span data-ttu-id="c98a9-122">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-122">String</span></span>  |   <span data-ttu-id="c98a9-123">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="c98a9-123">Name of the control.</span></span> |
|   <span data-ttu-id="c98a9-124">title</span><span class="sxs-lookup"><span data-stu-id="c98a9-124">title</span></span>   |   <span data-ttu-id="c98a9-125">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-125">String</span></span>  |   <span data-ttu-id="c98a9-126">Название элемента управления.</span><span class="sxs-lookup"><span data-stu-id="c98a9-126">Title of the control.</span></span>   |
| <span data-ttu-id="c98a9-127">Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="c98a9-127">complianceInformation</span></span> | <span data-ttu-id="c98a9-128">Коллекция [комплианцеинформатион](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="c98a9-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="c98a9-129">Коллекция сведений о соответствии, связанных с контролем безопасности по показателю</span><span class="sxs-lookup"><span data-stu-id="c98a9-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="c98a9-130">Контролкатегори</span><span class="sxs-lookup"><span data-stu-id="c98a9-130">controlCategory</span></span> |   <span data-ttu-id="c98a9-131">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-131">String</span></span>  |   <span data-ttu-id="c98a9-132">Категория действий управления (учетная запись, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="c98a9-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="c98a9-133">actionType</span><span class="sxs-lookup"><span data-stu-id="c98a9-133">actionType</span></span>  |   <span data-ttu-id="c98a9-134">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-134">String</span></span>  |   <span data-ttu-id="c98a9-135">Тип действия управления (config, проверка, поведение).</span><span class="sxs-lookup"><span data-stu-id="c98a9-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="c98a9-136">service</span><span class="sxs-lookup"><span data-stu-id="c98a9-136">service</span></span> |   <span data-ttu-id="c98a9-137">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-137">String</span></span>  |   <span data-ttu-id="c98a9-138">Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c98a9-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="c98a9-139">Максскоре</span><span class="sxs-lookup"><span data-stu-id="c98a9-139">maxScore</span></span> |  <span data-ttu-id="c98a9-140">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-140">String</span></span>  |   <span data-ttu-id="c98a9-141">Текущий полученный максимальный показатель на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="c98a9-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="c98a9-142">медленно</span><span class="sxs-lookup"><span data-stu-id="c98a9-142">tier</span></span> |  <span data-ttu-id="c98a9-143">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-143">String</span></span>  |   <span data-ttu-id="c98a9-144">Уровень управления (ядро, Глубокая защита, расширенная)</span><span class="sxs-lookup"><span data-stu-id="c98a9-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="c98a9-145">Усеримпакт</span><span class="sxs-lookup"><span data-stu-id="c98a9-145">userImpact</span></span> |    <span data-ttu-id="c98a9-146">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-146">String</span></span>  | <span data-ttu-id="c98a9-147">Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="c98a9-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="c98a9-148">Имплементатионкост</span><span class="sxs-lookup"><span data-stu-id="c98a9-148">implementationCost</span></span> |    <span data-ttu-id="c98a9-149">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-149">String</span></span>  |   <span data-ttu-id="c98a9-150">Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая).</span><span class="sxs-lookup"><span data-stu-id="c98a9-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="c98a9-151">rank</span><span class="sxs-lookup"><span data-stu-id="c98a9-151">rank</span></span> |  <span data-ttu-id="c98a9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c98a9-152">Int32</span></span>   |   <span data-ttu-id="c98a9-153">Ранжирование стека для элемента управления корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="c98a9-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="c98a9-154">угроз</span><span class="sxs-lookup"><span data-stu-id="c98a9-154">threats</span></span> |   <span data-ttu-id="c98a9-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c98a9-155">String Collection</span></span>   |   <span data-ttu-id="c98a9-156">Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, Датаексфилтратион,,, elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена).</span><span class="sxs-lookup"><span data-stu-id="c98a9-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="c98a9-157">устаревшие</span><span class="sxs-lookup"><span data-stu-id="c98a9-157">deprecated</span></span> |    <span data-ttu-id="c98a9-158">Логический</span><span class="sxs-lookup"><span data-stu-id="c98a9-158">Boolean</span></span> |   <span data-ttu-id="c98a9-159">Флаг, указывающий, является ли элемент управления амортизировано.</span><span class="sxs-lookup"><span data-stu-id="c98a9-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="c98a9-160">исправления</span><span class="sxs-lookup"><span data-stu-id="c98a9-160">remediation</span></span> |   <span data-ttu-id="c98a9-161">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-161">String</span></span>  |   <span data-ttu-id="c98a9-162">Описание того, что будет исправлено элементом управления.</span><span class="sxs-lookup"><span data-stu-id="c98a9-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="c98a9-163">Ремедиатионимпакт</span><span class="sxs-lookup"><span data-stu-id="c98a9-163">remediationImpact</span></span> | <span data-ttu-id="c98a9-164">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-164">String</span></span>  |   <span data-ttu-id="c98a9-165">Описание влияния на пользователей об исправлении.</span><span class="sxs-lookup"><span data-stu-id="c98a9-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="c98a9-166">Актионурл</span><span class="sxs-lookup"><span data-stu-id="c98a9-166">actionUrl</span></span> | <span data-ttu-id="c98a9-167">String</span><span class="sxs-lookup"><span data-stu-id="c98a9-167">String</span></span>  |   <span data-ttu-id="c98a9-168">URL-адрес, по которому можно выполнить действия с элементом управления.</span><span class="sxs-lookup"><span data-stu-id="c98a9-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="c98a9-169">Контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="c98a9-169">controlStateUpdates</span></span> | <span data-ttu-id="c98a9-170">Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="c98a9-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |    <span data-ttu-id="c98a9-171">Флаг, указывающий, где клиент пометил элемент управления (Ignore, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="c98a9-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="c98a9-172">Вендоринформатион</span><span class="sxs-lookup"><span data-stu-id="c98a9-172">vendorInformation</span></span> | [<span data-ttu-id="c98a9-173">Секуритивендоринформатион</span><span class="sxs-lookup"><span data-stu-id="c98a9-173">securityVendorInformation</span></span>](securityvendorinformation.md) |

## <a name="relationships"></a><span data-ttu-id="c98a9-174">Связи</span><span class="sxs-lookup"><span data-stu-id="c98a9-174">Relationships</span></span>

<span data-ttu-id="c98a9-175">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c98a9-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c98a9-176">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c98a9-176">JSON representation</span></span>

<span data-ttu-id="c98a9-177">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c98a9-177">The following is a JSON representation of the resource.</span></span>

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
  "maxScore": 1024.13,
  "actionType": "String",
  "service": "String",
  "tier": "String",
  "userImpact": "string",
  "implementationCost ": "String",
  "rank ": 100,
  "threats": ["string"],
  "deprecated ": false,
  "remediation": "String",
  "remediationImpact ": "String",
  "actionUrl": "String",
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}],
  "controlCategory": "string",
  "lastModifiedDateTime": "String (timestamp)"
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
