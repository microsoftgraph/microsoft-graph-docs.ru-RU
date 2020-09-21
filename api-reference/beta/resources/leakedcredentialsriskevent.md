---
title: Тип ресурса Леакедкредентиалсрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором были обнаружены учетные данные учетной записи в подстановке. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: c9c1efda0cb4c11899d5884da05a91f07e5a000d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029232"
---
# <a name="leakedcredentialsriskevent-resource-type-deprecated"></a><span data-ttu-id="afbc1-104">Тип ресурса Леакедкредентиалсрискевент (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="afbc1-104">leakedCredentialsRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="afbc1-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afbc1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="afbc1-106">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="afbc1-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="afbc1-107">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="afbc1-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="afbc1-108">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) , в котором были обнаружены учетные данные учетной записи в подстановке.</span><span class="sxs-lookup"><span data-stu-id="afbc1-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="afbc1-109">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="afbc1-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="afbc1-110">Методы</span><span class="sxs-lookup"><span data-stu-id="afbc1-110">Methods</span></span>

| <span data-ttu-id="afbc1-111">Метод</span><span class="sxs-lookup"><span data-stu-id="afbc1-111">Method</span></span>           | <span data-ttu-id="afbc1-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="afbc1-112">Return Type</span></span>    |<span data-ttu-id="afbc1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="afbc1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="afbc1-114">Получение объекта leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="afbc1-114">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="afbc1-115">леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="afbc1-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="afbc1-116">Чтение свойств и связей объекта Леакедкредентиалсрискевент.</span><span class="sxs-lookup"><span data-stu-id="afbc1-116">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="afbc1-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="afbc1-117">Properties</span></span>
| <span data-ttu-id="afbc1-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="afbc1-118">Property</span></span>     | <span data-ttu-id="afbc1-119">Тип</span><span class="sxs-lookup"><span data-stu-id="afbc1-119">Type</span></span>   |<span data-ttu-id="afbc1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="afbc1-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afbc1-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="afbc1-121">closedDateTime</span></span>|<span data-ttu-id="afbc1-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afbc1-122">dateTimeOffset</span></span>| <span data-ttu-id="afbc1-123">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="afbc1-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="afbc1-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afbc1-124">createdDateTime</span></span>|<span data-ttu-id="afbc1-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afbc1-125">dateTimeOffset</span></span>| <span data-ttu-id="afbc1-126">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="afbc1-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="afbc1-127">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="afbc1-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="afbc1-128">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="afbc1-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="afbc1-129">id</span><span class="sxs-lookup"><span data-stu-id="afbc1-129">id</span></span>|<span data-ttu-id="afbc1-130">string</span><span class="sxs-lookup"><span data-stu-id="afbc1-130">string</span></span>| <span data-ttu-id="afbc1-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="afbc1-131">Read-only</span></span>|
|<span data-ttu-id="afbc1-132">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="afbc1-132">riskEventDateTime</span></span>|<span data-ttu-id="afbc1-133">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afbc1-133">dateTimeOffset</span></span>| <span data-ttu-id="afbc1-134">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="afbc1-134">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="afbc1-135">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="afbc1-135">riskEventStatus</span></span>|<span data-ttu-id="afbc1-136">string</span><span class="sxs-lookup"><span data-stu-id="afbc1-136">string</span></span>| <span data-ttu-id="afbc1-137">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="afbc1-137">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="afbc1-138">riskLevel</span><span class="sxs-lookup"><span data-stu-id="afbc1-138">riskLevel</span></span>|<span data-ttu-id="afbc1-139">string</span><span class="sxs-lookup"><span data-stu-id="afbc1-139">string</span></span>| <span data-ttu-id="afbc1-140">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="afbc1-140">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="afbc1-141">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="afbc1-141">riskEventType</span></span>|<span data-ttu-id="afbc1-142">string</span><span class="sxs-lookup"><span data-stu-id="afbc1-142">string</span></span>| <span data-ttu-id="afbc1-143">Тип риска</span><span class="sxs-lookup"><span data-stu-id="afbc1-143">The type of risk</span></span>|
|<span data-ttu-id="afbc1-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="afbc1-144">userDisplayName</span></span>|<span data-ttu-id="afbc1-145">string</span><span class="sxs-lookup"><span data-stu-id="afbc1-145">string</span></span>| <span data-ttu-id="afbc1-146">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="afbc1-146">The name of the user at risk</span></span>|
|<span data-ttu-id="afbc1-147">userId</span><span class="sxs-lookup"><span data-stu-id="afbc1-147">userId</span></span>|<span data-ttu-id="afbc1-148">строка</span><span class="sxs-lookup"><span data-stu-id="afbc1-148">string</span></span>| <span data-ttu-id="afbc1-149">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="afbc1-149">The id of the user at risk</span></span>|
|<span data-ttu-id="afbc1-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="afbc1-150">userPrincipalName</span></span>|<span data-ttu-id="afbc1-151">string</span><span class="sxs-lookup"><span data-stu-id="afbc1-151">string</span></span>| <span data-ttu-id="afbc1-152">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="afbc1-152">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="afbc1-153">Отношения</span><span class="sxs-lookup"><span data-stu-id="afbc1-153">Relationships</span></span>
| <span data-ttu-id="afbc1-154">Связь</span><span class="sxs-lookup"><span data-stu-id="afbc1-154">Relationship</span></span> | <span data-ttu-id="afbc1-155">Тип</span><span class="sxs-lookup"><span data-stu-id="afbc1-155">Type</span></span>   |<span data-ttu-id="afbc1-156">Описание</span><span class="sxs-lookup"><span data-stu-id="afbc1-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afbc1-157">импактедусер</span><span class="sxs-lookup"><span data-stu-id="afbc1-157">impactedUser</span></span>|[<span data-ttu-id="afbc1-158">user</span><span class="sxs-lookup"><span data-stu-id="afbc1-158">user</span></span>](user.md)| <span data-ttu-id="afbc1-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="afbc1-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="afbc1-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="afbc1-161">JSON representation</span></span>

<span data-ttu-id="afbc1-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="afbc1-162">Here is a JSON representation of the resource.</span></span>

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


