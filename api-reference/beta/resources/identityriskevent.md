---
title: тип ресурса identityRiskEvent
description: 'Событие риска, обнаруженное службой Azure Active Directory Identity Protection. Это базовый тип для каждого конкретного типа событий риска:'
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: acb48ce5ef63abf5ec2a09d8a3365a744bb8a668
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440292"
---
# <a name="identityriskevent-resource-type-deprecated"></a><span data-ttu-id="f0771-104">тип ресурса identityRiskEvent (обесценен)</span><span class="sxs-lookup"><span data-stu-id="f0771-104">identityRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="f0771-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0771-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="f0771-106">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="f0771-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="f0771-107">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="f0771-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="f0771-108">Событие риска, обнаруженное [Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="f0771-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span> <span data-ttu-id="f0771-109">Это базовый тип для каждого конкретного типа событий риска:</span><span class="sxs-lookup"><span data-stu-id="f0771-109">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="f0771-110">Тип события</span><span class="sxs-lookup"><span data-stu-id="f0771-110">Event type</span></span>         | <span data-ttu-id="f0771-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f0771-111">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="f0771-112">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f0771-112">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="f0771-113">Входы с анонимных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="f0771-113">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="f0771-114">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f0771-114">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="f0771-115">Входы с зараженных вредоносными программами устройств.</span><span class="sxs-lookup"><span data-stu-id="f0771-115">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="f0771-116">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f0771-116">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="f0771-117">Невозможное путешествие в нетипичные расположения.</span><span class="sxs-lookup"><span data-stu-id="f0771-117">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="f0771-118">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f0771-118">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="f0771-119">Пользователи с утечкой учетных данных.</span><span class="sxs-lookup"><span data-stu-id="f0771-119">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="f0771-120">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f0771-120">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="f0771-121">Входы с подозрительных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="f0771-121">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="f0771-122">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f0771-122">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="f0771-123">Входы из незнакомых мест.</span><span class="sxs-lookup"><span data-stu-id="f0771-123">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="f0771-124">Полные сведения о событиях риска можно найти в документации [azure AD Identity Protection.](/azure/active-directory/active-directory-reporting-risk-events)</span><span class="sxs-lookup"><span data-stu-id="f0771-124">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="f0771-125">Методы</span><span class="sxs-lookup"><span data-stu-id="f0771-125">Methods</span></span>

| <span data-ttu-id="f0771-126">Метод</span><span class="sxs-lookup"><span data-stu-id="f0771-126">Method</span></span>           | <span data-ttu-id="f0771-127">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f0771-127">Return Type</span></span>    |<span data-ttu-id="f0771-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f0771-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0771-129">Получение объекта identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f0771-129">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="f0771-130">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f0771-130">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="f0771-131">Чтение свойств и связей объекта identityRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="f0771-131">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0771-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0771-132">Properties</span></span>
| <span data-ttu-id="f0771-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0771-133">Property</span></span>     | <span data-ttu-id="f0771-134">Тип</span><span class="sxs-lookup"><span data-stu-id="f0771-134">Type</span></span>   |<span data-ttu-id="f0771-135">Описание</span><span class="sxs-lookup"><span data-stu-id="f0771-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0771-136">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0771-136">closedDateTime</span></span>|<span data-ttu-id="f0771-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0771-137">dateTimeOffset</span></span>| <span data-ttu-id="f0771-138">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="f0771-138">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="f0771-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0771-139">createdDateTime</span></span>|<span data-ttu-id="f0771-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0771-140">dateTimeOffset</span></span>| <span data-ttu-id="f0771-141">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="f0771-141">The date and time that the risk event was created.</span></span> <span data-ttu-id="f0771-142">Это всегда больше или равно дате самого события риска.</span><span class="sxs-lookup"><span data-stu-id="f0771-142">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="f0771-143">Это правильное свойство, используемее в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="f0771-143">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="f0771-144">id</span><span class="sxs-lookup"><span data-stu-id="f0771-144">id</span></span>|<span data-ttu-id="f0771-145">string</span><span class="sxs-lookup"><span data-stu-id="f0771-145">string</span></span>| <span data-ttu-id="f0771-146">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="f0771-146">Read-only</span></span>|
|<span data-ttu-id="f0771-147">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="f0771-147">riskEventDateTime</span></span>|<span data-ttu-id="f0771-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0771-148">dateTimeOffset</span></span>| <span data-ttu-id="f0771-149">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="f0771-149">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="f0771-150">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="f0771-150">riskEventStatus</span></span>|<span data-ttu-id="f0771-151">string</span><span class="sxs-lookup"><span data-stu-id="f0771-151">string</span></span>| <span data-ttu-id="f0771-152">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="f0771-152">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="f0771-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f0771-153">riskLevel</span></span>|<span data-ttu-id="f0771-154">string</span><span class="sxs-lookup"><span data-stu-id="f0771-154">string</span></span>| <span data-ttu-id="f0771-155">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f0771-155">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="f0771-156">riskEventType</span><span class="sxs-lookup"><span data-stu-id="f0771-156">riskEventType</span></span>|<span data-ttu-id="f0771-157">string</span><span class="sxs-lookup"><span data-stu-id="f0771-157">string</span></span>| <span data-ttu-id="f0771-158">Тип риска</span><span class="sxs-lookup"><span data-stu-id="f0771-158">The type of risk</span></span>|
|<span data-ttu-id="f0771-159">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f0771-159">userDisplayName</span></span>|<span data-ttu-id="f0771-160">string</span><span class="sxs-lookup"><span data-stu-id="f0771-160">string</span></span>| <span data-ttu-id="f0771-161">Имя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="f0771-161">The name of the user at risk</span></span>|
|<span data-ttu-id="f0771-162">userId</span><span class="sxs-lookup"><span data-stu-id="f0771-162">userId</span></span>|<span data-ttu-id="f0771-163">строка</span><span class="sxs-lookup"><span data-stu-id="f0771-163">string</span></span>| <span data-ttu-id="f0771-164">ID пользователя, на который существует риск</span><span class="sxs-lookup"><span data-stu-id="f0771-164">The id of the user at risk</span></span>|
|<span data-ttu-id="f0771-165">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f0771-165">userPrincipalName</span></span>|<span data-ttu-id="f0771-166">string</span><span class="sxs-lookup"><span data-stu-id="f0771-166">string</span></span>| <span data-ttu-id="f0771-167">Основное имя пользователя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="f0771-167">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0771-168">Связи</span><span class="sxs-lookup"><span data-stu-id="f0771-168">Relationships</span></span>
| <span data-ttu-id="f0771-169">Связь</span><span class="sxs-lookup"><span data-stu-id="f0771-169">Relationship</span></span> | <span data-ttu-id="f0771-170">Тип</span><span class="sxs-lookup"><span data-stu-id="f0771-170">Type</span></span>   |<span data-ttu-id="f0771-171">Описание</span><span class="sxs-lookup"><span data-stu-id="f0771-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0771-172">impactedUser</span><span class="sxs-lookup"><span data-stu-id="f0771-172">impactedUser</span></span>|[<span data-ttu-id="f0771-173">user</span><span class="sxs-lookup"><span data-stu-id="f0771-173">user</span></span>](user.md)| <span data-ttu-id="f0771-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f0771-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0771-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0771-176">JSON representation</span></span>

<span data-ttu-id="f0771-177">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0771-177">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
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
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
