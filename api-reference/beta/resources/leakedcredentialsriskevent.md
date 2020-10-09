---
title: Тип ресурса Леакедкредентиалсрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором были обнаружены учетные данные учетной записи в подстановке. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 05c887fade095da07b12c1b82c9efdf71259234f
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404681"
---
# <a name="leakedcredentialsriskevent-resource-type-deprecated"></a><span data-ttu-id="468b6-104">Тип ресурса Леакедкредентиалсрискевент (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="468b6-104">leakedCredentialsRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="468b6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="468b6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="468b6-106">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="468b6-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="468b6-107">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="468b6-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="468b6-108">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) , в котором были обнаружены учетные данные учетной записи в подстановке.</span><span class="sxs-lookup"><span data-stu-id="468b6-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="468b6-109">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="468b6-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="468b6-110">Методы</span><span class="sxs-lookup"><span data-stu-id="468b6-110">Methods</span></span>

| <span data-ttu-id="468b6-111">Метод</span><span class="sxs-lookup"><span data-stu-id="468b6-111">Method</span></span>           | <span data-ttu-id="468b6-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="468b6-112">Return Type</span></span>    |<span data-ttu-id="468b6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="468b6-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="468b6-114">Получение объекта leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="468b6-114">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="468b6-115">леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="468b6-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="468b6-116">Чтение свойств и связей объекта Леакедкредентиалсрискевент.</span><span class="sxs-lookup"><span data-stu-id="468b6-116">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="468b6-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="468b6-117">Properties</span></span>
| <span data-ttu-id="468b6-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="468b6-118">Property</span></span>     | <span data-ttu-id="468b6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="468b6-119">Type</span></span>   |<span data-ttu-id="468b6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="468b6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="468b6-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="468b6-121">closedDateTime</span></span>|<span data-ttu-id="468b6-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="468b6-122">dateTimeOffset</span></span>| <span data-ttu-id="468b6-123">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="468b6-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="468b6-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="468b6-124">createdDateTime</span></span>|<span data-ttu-id="468b6-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="468b6-125">dateTimeOffset</span></span>| <span data-ttu-id="468b6-126">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="468b6-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="468b6-127">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="468b6-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="468b6-128">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="468b6-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="468b6-129">id</span><span class="sxs-lookup"><span data-stu-id="468b6-129">id</span></span>|<span data-ttu-id="468b6-130">string</span><span class="sxs-lookup"><span data-stu-id="468b6-130">string</span></span>| <span data-ttu-id="468b6-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="468b6-131">Read-only</span></span>|
|<span data-ttu-id="468b6-132">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="468b6-132">riskEventDateTime</span></span>|<span data-ttu-id="468b6-133">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="468b6-133">dateTimeOffset</span></span>| <span data-ttu-id="468b6-134">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="468b6-134">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="468b6-135">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="468b6-135">riskEventStatus</span></span>|<span data-ttu-id="468b6-136">string</span><span class="sxs-lookup"><span data-stu-id="468b6-136">string</span></span>| <span data-ttu-id="468b6-137">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="468b6-137">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="468b6-138">riskLevel</span><span class="sxs-lookup"><span data-stu-id="468b6-138">riskLevel</span></span>|<span data-ttu-id="468b6-139">string</span><span class="sxs-lookup"><span data-stu-id="468b6-139">string</span></span>| <span data-ttu-id="468b6-140">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="468b6-140">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="468b6-141">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="468b6-141">riskEventType</span></span>|<span data-ttu-id="468b6-142">string</span><span class="sxs-lookup"><span data-stu-id="468b6-142">string</span></span>| <span data-ttu-id="468b6-143">Тип риска</span><span class="sxs-lookup"><span data-stu-id="468b6-143">The type of risk</span></span>|
|<span data-ttu-id="468b6-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="468b6-144">userDisplayName</span></span>|<span data-ttu-id="468b6-145">string</span><span class="sxs-lookup"><span data-stu-id="468b6-145">string</span></span>| <span data-ttu-id="468b6-146">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="468b6-146">The name of the user at risk</span></span>|
|<span data-ttu-id="468b6-147">userId</span><span class="sxs-lookup"><span data-stu-id="468b6-147">userId</span></span>|<span data-ttu-id="468b6-148">строка</span><span class="sxs-lookup"><span data-stu-id="468b6-148">string</span></span>| <span data-ttu-id="468b6-149">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="468b6-149">The id of the user at risk</span></span>|
|<span data-ttu-id="468b6-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="468b6-150">userPrincipalName</span></span>|<span data-ttu-id="468b6-151">string</span><span class="sxs-lookup"><span data-stu-id="468b6-151">string</span></span>| <span data-ttu-id="468b6-152">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="468b6-152">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="468b6-153">Связи</span><span class="sxs-lookup"><span data-stu-id="468b6-153">Relationships</span></span>
| <span data-ttu-id="468b6-154">Связь</span><span class="sxs-lookup"><span data-stu-id="468b6-154">Relationship</span></span> | <span data-ttu-id="468b6-155">Тип</span><span class="sxs-lookup"><span data-stu-id="468b6-155">Type</span></span>   |<span data-ttu-id="468b6-156">Описание</span><span class="sxs-lookup"><span data-stu-id="468b6-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="468b6-157">импактедусер</span><span class="sxs-lookup"><span data-stu-id="468b6-157">impactedUser</span></span>|[<span data-ttu-id="468b6-158">user</span><span class="sxs-lookup"><span data-stu-id="468b6-158">user</span></span>](user.md)| <span data-ttu-id="468b6-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="468b6-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="468b6-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="468b6-161">JSON representation</span></span>

<span data-ttu-id="468b6-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="468b6-162">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->