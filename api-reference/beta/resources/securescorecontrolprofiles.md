---
title: Тип ресурса Секурескореконтролпрофилес
description: Представляет уровень безопасности клиента для данных элемента управления. По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549176"
---
# <a name="securescorecontrolprofiles-resource-type"></a><span data-ttu-id="efd09-104">Тип ресурса Секурескореконтролпрофилес</span><span class="sxs-lookup"><span data-stu-id="efd09-104">secureScoreControlProfiles resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd09-105">Представляет уровень безопасности клиента для данных элемента управления.</span><span class="sxs-lookup"><span data-stu-id="efd09-105">Represents a tenant's secure score per control data.</span></span> <span data-ttu-id="efd09-106">По умолчанию он возвращает все элементы управления для клиента и может явно извлекать отдельные элементы управления.</span><span class="sxs-lookup"><span data-stu-id="efd09-106">By default, it returns all controls for a tenant and can explicitly pull individual controls.</span></span>


## <a name="methods"></a><span data-ttu-id="efd09-107">Методы</span><span class="sxs-lookup"><span data-stu-id="efd09-107">Methods</span></span>

| <span data-ttu-id="efd09-108">Метод</span><span class="sxs-lookup"><span data-stu-id="efd09-108">Method</span></span>   | <span data-ttu-id="efd09-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="efd09-109">Return Type</span></span>|<span data-ttu-id="efd09-110">Описание</span><span class="sxs-lookup"><span data-stu-id="efd09-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efd09-111">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="efd09-111">List secureScoreControlProfiles</span></span>](../api/securescorecontrolprofiles-list.md) | [<span data-ttu-id="efd09-112">secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="efd09-112">secureScoreControlProfiles</span></span>](securescorecontrolprofiles.md) |<span data-ttu-id="efd09-113">Чтение свойств и метаданных объекта Секурескореконтролпрофилес.</span><span class="sxs-lookup"><span data-stu-id="efd09-113">Read properties and metadata of a secureScoreControlProfiles object.</span></span>|


## <a name="properties"></a><span data-ttu-id="efd09-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="efd09-114">Properties</span></span>

|<span data-ttu-id="efd09-115">Имя</span><span class="sxs-lookup"><span data-stu-id="efd09-115">Name</span></span> |<span data-ttu-id="efd09-116">Тип</span><span class="sxs-lookup"><span data-stu-id="efd09-116">Type</span></span> |<span data-ttu-id="efd09-117">Описание</span><span class="sxs-lookup"><span data-stu-id="efd09-117">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="efd09-118">Азуретенантид</span><span class="sxs-lookup"><span data-stu-id="efd09-118">azureTenantId</span></span>   |   <span data-ttu-id="efd09-119">String</span><span class="sxs-lookup"><span data-stu-id="efd09-119">String</span></span>  |   <span data-ttu-id="efd09-120">Строка GUID для идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="efd09-120">GUID string for tenant ID.</span></span>  |
|   <span data-ttu-id="efd09-121">Контролнаме</span><span class="sxs-lookup"><span data-stu-id="efd09-121">controlName</span></span> |   <span data-ttu-id="efd09-122">String</span><span class="sxs-lookup"><span data-stu-id="efd09-122">String</span></span>  |   <span data-ttu-id="efd09-123">Имя элемента управления.</span><span class="sxs-lookup"><span data-stu-id="efd09-123">Name of the control.</span></span> |
|   <span data-ttu-id="efd09-124">title</span><span class="sxs-lookup"><span data-stu-id="efd09-124">title</span></span>   |   <span data-ttu-id="efd09-125">Строка</span><span class="sxs-lookup"><span data-stu-id="efd09-125">String</span></span>  |   <span data-ttu-id="efd09-126">Название элемента управления.</span><span class="sxs-lookup"><span data-stu-id="efd09-126">Title of the control.</span></span>   |
| <span data-ttu-id="efd09-127">Комплианцеинформатион</span><span class="sxs-lookup"><span data-stu-id="efd09-127">complianceInformation</span></span> | <span data-ttu-id="efd09-128">Коллекция [комплианцеинформатион](complianceinformation.md)</span><span class="sxs-lookup"><span data-stu-id="efd09-128">[complianceInformation](complianceinformation.md) collection</span></span> | <span data-ttu-id="efd09-129">Коллекция сведений о соответствии, связанных с контролем безопасности по показателю</span><span class="sxs-lookup"><span data-stu-id="efd09-129">The collection of compliance information associated with secure score control</span></span> |
|   <span data-ttu-id="efd09-130">Контролкатегори</span><span class="sxs-lookup"><span data-stu-id="efd09-130">controlCategory</span></span> |   <span data-ttu-id="efd09-131">String</span><span class="sxs-lookup"><span data-stu-id="efd09-131">String</span></span>  |   <span data-ttu-id="efd09-132">Категория действий управления (учетная запись, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="efd09-132">Control action category (Account, Data, Device, Apps, Infrastructure).</span></span>  |
|   <span data-ttu-id="efd09-133">actionType</span><span class="sxs-lookup"><span data-stu-id="efd09-133">actionType</span></span>  |   <span data-ttu-id="efd09-134">String</span><span class="sxs-lookup"><span data-stu-id="efd09-134">String</span></span>  |   <span data-ttu-id="efd09-135">Тип действия управления (config, проверка, поведение).</span><span class="sxs-lookup"><span data-stu-id="efd09-135">Control action type (Config, Review, Behavior).</span></span> |
|   <span data-ttu-id="efd09-136">service</span><span class="sxs-lookup"><span data-stu-id="efd09-136">service</span></span> |   <span data-ttu-id="efd09-137">String</span><span class="sxs-lookup"><span data-stu-id="efd09-137">String</span></span>  |   <span data-ttu-id="efd09-138">Служба, которая владеет элементом управления (Exchange, SharePoint, Azure AD).</span><span class="sxs-lookup"><span data-stu-id="efd09-138">Service that owns the control (Exchange, Sharepoint, Azure AD).</span></span> |
|   <span data-ttu-id="efd09-139">Максскоре</span><span class="sxs-lookup"><span data-stu-id="efd09-139">maxScore</span></span> |  <span data-ttu-id="efd09-140">String</span><span class="sxs-lookup"><span data-stu-id="efd09-140">String</span></span>  |   <span data-ttu-id="efd09-141">Текущий полученный максимальный показатель на указанную дату.</span><span class="sxs-lookup"><span data-stu-id="efd09-141">Current obtained max score on specified date.</span></span>   |
|   <span data-ttu-id="efd09-142">медленно</span><span class="sxs-lookup"><span data-stu-id="efd09-142">tier</span></span> |  <span data-ttu-id="efd09-143">String</span><span class="sxs-lookup"><span data-stu-id="efd09-143">String</span></span>  |   <span data-ttu-id="efd09-144">Уровень управления (ядро, Глубокая защита, расширенная)</span><span class="sxs-lookup"><span data-stu-id="efd09-144">Control tier (Core, Defense in Depth, Advanced.)</span></span>    |
|   <span data-ttu-id="efd09-145">Усеримпакт</span><span class="sxs-lookup"><span data-stu-id="efd09-145">userImpact</span></span> |    <span data-ttu-id="efd09-146">String</span><span class="sxs-lookup"><span data-stu-id="efd09-146">String</span></span>  | <span data-ttu-id="efd09-147">Пользовательское воздействие на реализацию элемента управления (минимальный, средний, высокий).</span><span class="sxs-lookup"><span data-stu-id="efd09-147">User impact of implementing control (low, moderate, high).</span></span>    |
|   <span data-ttu-id="efd09-148">Имплементатионкост</span><span class="sxs-lookup"><span data-stu-id="efd09-148">implementationCost</span></span> |    <span data-ttu-id="efd09-149">String</span><span class="sxs-lookup"><span data-stu-id="efd09-149">String</span></span>  |   <span data-ttu-id="efd09-150">Стоимость ресурсов элемента управления имплемментатинг (минимальная, средняя, высокая).</span><span class="sxs-lookup"><span data-stu-id="efd09-150">Resource cost of implemmentating control (low, moderate, high).</span></span> |
|   <span data-ttu-id="efd09-151">rank</span><span class="sxs-lookup"><span data-stu-id="efd09-151">rank</span></span> |  <span data-ttu-id="efd09-152">Int32</span><span class="sxs-lookup"><span data-stu-id="efd09-152">Int32</span></span>   |   <span data-ttu-id="efd09-153">Ранжирование стека для элемента управления корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="efd09-153">Microsoft's stack ranking of control.</span></span>   |
|   <span data-ttu-id="efd09-154">угроз</span><span class="sxs-lookup"><span data-stu-id="efd09-154">threats</span></span> |   <span data-ttu-id="efd09-155">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="efd09-155">String Collection</span></span>   |   <span data-ttu-id="efd09-156">Список угроз, по которым элемент управления уменьшается (Аккаунтбреач, Датаексфилтратион,,, elevationOfPrivilege, МалиЦиаусинсидер, Пассвордкраккинг, Фишингорвхалинг, подмена).</span><span class="sxs-lookup"><span data-stu-id="efd09-156">List of threats the control mitigates (accountBreach,dataDeletion,dataExfiltration,dataSpillage,elevationOfPrivilege,maliciousInsider,passwordCracking,phishingOrWhaling,spoofing).</span></span> |
|   <span data-ttu-id="efd09-157">устаревшие</span><span class="sxs-lookup"><span data-stu-id="efd09-157">deprecated</span></span> |    <span data-ttu-id="efd09-158">Логический</span><span class="sxs-lookup"><span data-stu-id="efd09-158">Boolean</span></span> |   <span data-ttu-id="efd09-159">Флаг, указывающий, является ли элемент управления амортизировано.</span><span class="sxs-lookup"><span data-stu-id="efd09-159">Flag to indicate if a control is depreciated.</span></span>   |
|   <span data-ttu-id="efd09-160">исправления</span><span class="sxs-lookup"><span data-stu-id="efd09-160">remediation</span></span> |   <span data-ttu-id="efd09-161">String</span><span class="sxs-lookup"><span data-stu-id="efd09-161">String</span></span>  |   <span data-ttu-id="efd09-162">Описание того, что будет исправлено элементом управления.</span><span class="sxs-lookup"><span data-stu-id="efd09-162">Description of what the control will help remediate.</span></span> |
|   <span data-ttu-id="efd09-163">Ремедиатионимпакт</span><span class="sxs-lookup"><span data-stu-id="efd09-163">remediationImpact</span></span> | <span data-ttu-id="efd09-164">String</span><span class="sxs-lookup"><span data-stu-id="efd09-164">String</span></span>  |   <span data-ttu-id="efd09-165">Описание влияния на пользователей об исправлении.</span><span class="sxs-lookup"><span data-stu-id="efd09-165">Description of the impact on users of the remediation.</span></span> |
|   <span data-ttu-id="efd09-166">Актионурл</span><span class="sxs-lookup"><span data-stu-id="efd09-166">actionUrl</span></span> | <span data-ttu-id="efd09-167">String</span><span class="sxs-lookup"><span data-stu-id="efd09-167">String</span></span>  |   <span data-ttu-id="efd09-168">URL-адрес, по которому можно выполнить действия с элементом управления.</span><span class="sxs-lookup"><span data-stu-id="efd09-168">URL to where the control can be actioned.</span></span> |
|   <span data-ttu-id="efd09-169">Контролстатеупдатес</span><span class="sxs-lookup"><span data-stu-id="efd09-169">controlStateUpdates</span></span> |   <span data-ttu-id="efd09-170">Коллекция [секурескореконтролстатеупдате](securescorecontrolstateupdate.md)</span><span class="sxs-lookup"><span data-stu-id="efd09-170">[secureScoreControlStateUpdate](securescorecontrolstateupdate.md)   collection</span></span> |    <span data-ttu-id="efd09-171">Флаг, указывающий, где клиент пометил элемент управления (Ignore, thirdParty, проверен) (поддерживает [Обновление](../api/securescorecontrolprofiles-update.md)).</span><span class="sxs-lookup"><span data-stu-id="efd09-171">Flag to indicate where the tenant has marked a control (ignore, thirdParty, reviewed) (supports [update](../api/securescorecontrolprofiles-update.md)).</span></span> |

## <a name="relationships"></a><span data-ttu-id="efd09-172">Связи</span><span class="sxs-lookup"><span data-stu-id="efd09-172">Relationships</span></span>

<span data-ttu-id="efd09-173">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="efd09-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="efd09-174">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="efd09-174">JSON representation</span></span>

<span data-ttu-id="efd09-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efd09-175">The following is a JSON representation of the resource.</span></span>

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
