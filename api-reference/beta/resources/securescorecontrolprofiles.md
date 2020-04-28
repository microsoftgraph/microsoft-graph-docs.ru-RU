---
title: Тип ресурса Секурескореконтролпрофиле
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7dfca5eedebe7f2fe524c79cee52e5855af7f291
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520866"
---
# <a name="securescorecontrolprofile-resource-type"></a><span data-ttu-id="2340a-104">Тип ресурса Секурескореконтролпрофиле</span><span class="sxs-lookup"><span data-stu-id="2340a-104">secureScoreControlProfile resource type</span></span>

<span data-ttu-id="2340a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2340a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2340a-106">Представляет уровень безопасности клиента для данных элемента управления.</span><span class="sxs-lookup"><span data-stu-id="2340a-106">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="2340a-107">По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="2340a-107">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="2340a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2340a-108">Methods</span></span>

| <span data-ttu-id="2340a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2340a-109">Method</span></span>   | <span data-ttu-id="2340a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2340a-110">Return Type</span></span>|<span data-ttu-id="2340a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2340a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2340a-112">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="2340a-112">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | <span data-ttu-id="2340a-113">Коллекция [секурескореконтролпрофиле](securescorecontrolprofiles.md)</span><span class="sxs-lookup"><span data-stu-id="2340a-113">[secureScoreControlProfile](securescorecontrolprofiles.md) collection</span></span> |<span data-ttu-id="2340a-114">Получение коллекции объектов Секурескореконтролпрофиле.</span><span class="sxs-lookup"><span data-stu-id="2340a-114">Get a collection of secureScoreControlProfile objects.</span></span>|


## <a name="properties"></a><span data-ttu-id="2340a-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="2340a-115">Properties</span></span>

|<span data-ttu-id="2340a-116">Имя</span><span class="sxs-lookup"><span data-stu-id="2340a-116">Name</span></span> |<span data-ttu-id="2340a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="2340a-117">Type</span></span> |<span data-ttu-id="2340a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="2340a-118">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="2340a-119">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="2340a-119">azureTenantId</span></span>   |   <span data-ttu-id="2340a-120">String</span><span class="sxs-lookup"><span data-stu-id="2340a-120">String</span></span>  |   <span data-ttu-id="2340a-121">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="2340a-121">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="2340a-122">контролнаме</span><span class="sxs-lookup"><span data-stu-id="2340a-122">controlName</span></span> |   <span data-ttu-id="2340a-123">String</span><span class="sxs-lookup"><span data-stu-id="2340a-123">String</span></span>  |   <span data-ttu-id="2340a-124">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="2340a-124">Name of the control.</span></span> |
|   <span data-ttu-id="2340a-125">title</span><span class="sxs-lookup"><span data-stu-id="2340a-125">title</span></span>   |   <span data-ttu-id="2340a-126">Строка</span><span class="sxs-lookup"><span data-stu-id="2340a-126">String</span></span>  |   <span data-ttu-id="2340a-127">Название элемента управления.</span><span class="sxs-lookup"><span data-stu-id="2340a-127">Title of the control.</span></span>   |
| <span data-ttu-id="2340a-128">комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="2340a-128">complianceInformation</span></span> | <span data-ttu-id="2340a-129">Коллекция [комплианцеинформатион](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="2340a-129">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="2340a-130">Коллекция сведений о соответствии, связанных с контролем безопасности по показателю</span><span class="sxs-lookup"><span data-stu-id="2340a-130">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="2340a-131">контролкатегори</span><span class="sxs-lookup"><span data-stu-id="2340a-131">controlCategory</span></span> |   <span data-ttu-id="2340a-132">String</span><span class="sxs-lookup"><span data-stu-id="2340a-132">String</span></span>  |   <span data-ttu-id="2340a-133">Категория действий управления (учетная запись, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="2340a-133">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="2340a-134">actionType</span><span class="sxs-lookup"><span data-stu-id="2340a-134">actionType</span></span>  |   <span data-ttu-id="2340a-135">String</span><span class="sxs-lookup"><span data-stu-id="2340a-135">String</span></span>  |   <span data-ttu-id="2340a-136">Тип действия управления (config, проверка, поведение).</span><span class="sxs-lookup"><span data-stu-id="2340a-136">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="2340a-137">service</span><span class="sxs-lookup"><span data-stu-id="2340a-137">service</span></span> |   <span data-ttu-id="2340a-138">String</span><span class="sxs-lookup"><span data-stu-id="2340a-138">String</span></span>  |   <span data-ttu-id="2340a-139">Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2340a-139">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="2340a-140">максскоре</span><span class="sxs-lookup"><span data-stu-id="2340a-140">maxScore</span></span> |  <span data-ttu-id="2340a-141">String</span><span class="sxs-lookup"><span data-stu-id="2340a-141">String</span></span>  |   <span data-ttu-id="2340a-142">Текущий полученный максимальный показатель на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="2340a-142">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="2340a-143">медленно</span><span class="sxs-lookup"><span data-stu-id="2340a-143">tier</span></span> |  <span data-ttu-id="2340a-144">String</span><span class="sxs-lookup"><span data-stu-id="2340a-144">String</span></span>  |   <span data-ttu-id="2340a-145">Уровень управления (ядро, Глубокая защита, расширенная)</span><span class="sxs-lookup"><span data-stu-id="2340a-145">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="2340a-146">усеримпакт</span><span class="sxs-lookup"><span data-stu-id="2340a-146">userImpact</span></span> |    <span data-ttu-id="2340a-147">String</span><span class="sxs-lookup"><span data-stu-id="2340a-147">String</span></span>  | <span data-ttu-id="2340a-148">Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="2340a-148">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="2340a-149">имплементатионкост</span><span class="sxs-lookup"><span data-stu-id="2340a-149">implementationCost</span></span> |    <span data-ttu-id="2340a-150">String</span><span class="sxs-lookup"><span data-stu-id="2340a-150">String</span></span>  |   <span data-ttu-id="2340a-151">Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая).</span><span class="sxs-lookup"><span data-stu-id="2340a-151">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="2340a-152">rank</span><span class="sxs-lookup"><span data-stu-id="2340a-152">rank</span></span> |  <span data-ttu-id="2340a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2340a-153">Int32</span></span>   |   <span data-ttu-id="2340a-154">Ранжирование стека для элемента управления корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2340a-154">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="2340a-155">угроз</span><span class="sxs-lookup"><span data-stu-id="2340a-155">threats</span></span> |   <span data-ttu-id="2340a-156">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2340a-156">String Collection</span></span>   |   <span data-ttu-id="2340a-157">Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, Датаексфилтратион,,, elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена).</span><span class="sxs-lookup"><span data-stu-id="2340a-157">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="2340a-158">устаревшие</span><span class="sxs-lookup"><span data-stu-id="2340a-158">deprecated</span></span> |    <span data-ttu-id="2340a-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="2340a-159">Boolean</span></span> |   <span data-ttu-id="2340a-160">Флаг, указывающий, является ли элемент управления амортизировано.</span><span class="sxs-lookup"><span data-stu-id="2340a-160">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="2340a-161">исправления</span><span class="sxs-lookup"><span data-stu-id="2340a-161">remediation</span></span> |   <span data-ttu-id="2340a-162">String</span><span class="sxs-lookup"><span data-stu-id="2340a-162">String</span></span>  |   <span data-ttu-id="2340a-163">Описание того, что будет исправлено элементом управления.</span><span class="sxs-lookup"><span data-stu-id="2340a-163">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="2340a-164">ремедиатионимпакт</span><span class="sxs-lookup"><span data-stu-id="2340a-164">remediationImpact</span></span> | <span data-ttu-id="2340a-165">String</span><span class="sxs-lookup"><span data-stu-id="2340a-165">String</span></span>  |   <span data-ttu-id="2340a-166">Описание влияния на пользователей об исправлении.</span><span class="sxs-lookup"><span data-stu-id="2340a-166">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="2340a-167">актионурл</span><span class="sxs-lookup"><span data-stu-id="2340a-167">actionUrl</span></span> | <span data-ttu-id="2340a-168">String</span><span class="sxs-lookup"><span data-stu-id="2340a-168">String</span></span>  |   <span data-ttu-id="2340a-169">URL-адрес, по которому можно выполнить действия с элементом управления.</span><span class="sxs-lookup"><span data-stu-id="2340a-169">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="2340a-170">контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="2340a-170">controlStateUpdates</span></span> | <span data-ttu-id="2340a-171">Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="2340a-171">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) collection</span></span> |    <span data-ttu-id="2340a-172">Флаг, указывающий, где клиент пометил элемент управления (Ignore, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="2340a-172">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |
|   <span data-ttu-id="2340a-173">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="2340a-173">vendorInformation</span></span> | [<span data-ttu-id="2340a-174">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="2340a-174">securityVendorInformation</span></span>](securityvendorinformation.md) |

## <a name="relationships"></a><span data-ttu-id="2340a-175">Связи</span><span class="sxs-lookup"><span data-stu-id="2340a-175">Relationships</span></span>

<span data-ttu-id="2340a-176">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2340a-176">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2340a-177">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2340a-177">JSON representation</span></span>

<span data-ttu-id="2340a-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2340a-178">The following is a JSON representation of the resource.</span></span>

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
