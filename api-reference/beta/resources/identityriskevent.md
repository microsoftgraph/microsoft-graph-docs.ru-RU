---
title: Тип ресурса Идентитирискевент
description: 'Событие риска, обнаруженное защитой удостоверений Azure Active Directory. Это базовый тип для каждого конкретного типа событий риска:'
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 77ca53e3da465438bef1054b281842faa866a38c
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401416"
---
# <a name="identityriskevent-resource-type-deprecated"></a><span data-ttu-id="164ca-104">Тип ресурса Идентитирискевент (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="164ca-104">identityRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="164ca-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="164ca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="164ca-106">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="164ca-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="164ca-107">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="164ca-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="164ca-108">Событие риска, обнаруженное [защитой удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="164ca-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span> <span data-ttu-id="164ca-109">Это базовый тип для каждого конкретного типа событий риска:</span><span class="sxs-lookup"><span data-stu-id="164ca-109">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="164ca-110">Тип события</span><span class="sxs-lookup"><span data-stu-id="164ca-110">Event type</span></span>         | <span data-ttu-id="164ca-111">Описание</span><span class="sxs-lookup"><span data-stu-id="164ca-111">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="164ca-112">анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="164ca-112">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="164ca-113">Входы из анонимных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="164ca-113">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="164ca-114">малварерискевент</span><span class="sxs-lookup"><span data-stu-id="164ca-114">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="164ca-115">Входы с зараженных вредоносными программами устройств.</span><span class="sxs-lookup"><span data-stu-id="164ca-115">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="164ca-116">импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="164ca-116">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="164ca-117">Невозможность перемещаться к необычным расположениям.</span><span class="sxs-lookup"><span data-stu-id="164ca-117">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="164ca-118">леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="164ca-118">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="164ca-119">Пользователи с потерянными учетными данными.</span><span class="sxs-lookup"><span data-stu-id="164ca-119">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="164ca-120">суспиЦиаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="164ca-120">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="164ca-121">Входы из подозрительных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="164ca-121">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="164ca-122">унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="164ca-122">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="164ca-123">Входы из незнакомых расположений.</span><span class="sxs-lookup"><span data-stu-id="164ca-123">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="164ca-124">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="164ca-124">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="164ca-125">Методы</span><span class="sxs-lookup"><span data-stu-id="164ca-125">Methods</span></span>

| <span data-ttu-id="164ca-126">Метод</span><span class="sxs-lookup"><span data-stu-id="164ca-126">Method</span></span>           | <span data-ttu-id="164ca-127">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="164ca-127">Return Type</span></span>    |<span data-ttu-id="164ca-128">Описание</span><span class="sxs-lookup"><span data-stu-id="164ca-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="164ca-129">Получение объекта identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="164ca-129">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="164ca-130">идентитирискевент</span><span class="sxs-lookup"><span data-stu-id="164ca-130">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="164ca-131">Чтение свойств и связей объекта Идентитирискевент.</span><span class="sxs-lookup"><span data-stu-id="164ca-131">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="164ca-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="164ca-132">Properties</span></span>
| <span data-ttu-id="164ca-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="164ca-133">Property</span></span>     | <span data-ttu-id="164ca-134">Тип</span><span class="sxs-lookup"><span data-stu-id="164ca-134">Type</span></span>   |<span data-ttu-id="164ca-135">Описание</span><span class="sxs-lookup"><span data-stu-id="164ca-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="164ca-136">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="164ca-136">closedDateTime</span></span>|<span data-ttu-id="164ca-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="164ca-137">dateTimeOffset</span></span>| <span data-ttu-id="164ca-138">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="164ca-138">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="164ca-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="164ca-139">createdDateTime</span></span>|<span data-ttu-id="164ca-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="164ca-140">dateTimeOffset</span></span>| <span data-ttu-id="164ca-141">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="164ca-141">The date and time that the risk event was created.</span></span> <span data-ttu-id="164ca-142">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="164ca-142">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="164ca-143">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="164ca-143">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="164ca-144">id</span><span class="sxs-lookup"><span data-stu-id="164ca-144">id</span></span>|<span data-ttu-id="164ca-145">string</span><span class="sxs-lookup"><span data-stu-id="164ca-145">string</span></span>| <span data-ttu-id="164ca-146">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="164ca-146">Read-only</span></span>|
|<span data-ttu-id="164ca-147">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="164ca-147">riskEventDateTime</span></span>|<span data-ttu-id="164ca-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="164ca-148">dateTimeOffset</span></span>| <span data-ttu-id="164ca-149">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="164ca-149">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="164ca-150">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="164ca-150">riskEventStatus</span></span>|<span data-ttu-id="164ca-151">string</span><span class="sxs-lookup"><span data-stu-id="164ca-151">string</span></span>| <span data-ttu-id="164ca-152">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="164ca-152">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="164ca-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="164ca-153">riskLevel</span></span>|<span data-ttu-id="164ca-154">string</span><span class="sxs-lookup"><span data-stu-id="164ca-154">string</span></span>| <span data-ttu-id="164ca-155">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="164ca-155">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="164ca-156">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="164ca-156">riskEventType</span></span>|<span data-ttu-id="164ca-157">string</span><span class="sxs-lookup"><span data-stu-id="164ca-157">string</span></span>| <span data-ttu-id="164ca-158">Тип риска</span><span class="sxs-lookup"><span data-stu-id="164ca-158">The type of risk</span></span>|
|<span data-ttu-id="164ca-159">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="164ca-159">userDisplayName</span></span>|<span data-ttu-id="164ca-160">string</span><span class="sxs-lookup"><span data-stu-id="164ca-160">string</span></span>| <span data-ttu-id="164ca-161">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="164ca-161">The name of the user at risk</span></span>|
|<span data-ttu-id="164ca-162">userId</span><span class="sxs-lookup"><span data-stu-id="164ca-162">userId</span></span>|<span data-ttu-id="164ca-163">строка</span><span class="sxs-lookup"><span data-stu-id="164ca-163">string</span></span>| <span data-ttu-id="164ca-164">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="164ca-164">The id of the user at risk</span></span>|
|<span data-ttu-id="164ca-165">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="164ca-165">userPrincipalName</span></span>|<span data-ttu-id="164ca-166">string</span><span class="sxs-lookup"><span data-stu-id="164ca-166">string</span></span>| <span data-ttu-id="164ca-167">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="164ca-167">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="164ca-168">Связи</span><span class="sxs-lookup"><span data-stu-id="164ca-168">Relationships</span></span>
| <span data-ttu-id="164ca-169">Связь</span><span class="sxs-lookup"><span data-stu-id="164ca-169">Relationship</span></span> | <span data-ttu-id="164ca-170">Тип</span><span class="sxs-lookup"><span data-stu-id="164ca-170">Type</span></span>   |<span data-ttu-id="164ca-171">Описание</span><span class="sxs-lookup"><span data-stu-id="164ca-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="164ca-172">импактедусер</span><span class="sxs-lookup"><span data-stu-id="164ca-172">impactedUser</span></span>|[<span data-ttu-id="164ca-173">user</span><span class="sxs-lookup"><span data-stu-id="164ca-173">user</span></span>](user.md)| <span data-ttu-id="164ca-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="164ca-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="164ca-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="164ca-176">JSON representation</span></span>

<span data-ttu-id="164ca-177">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="164ca-177">Here is a JSON representation of the resource.</span></span>

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