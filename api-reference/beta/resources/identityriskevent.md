---
title: Тип ресурса Идентитирискевент
description: 'Событие риска, обнаруженное защитой удостоверений Azure Active Directory. Это базовый тип для каждого конкретного типа событий риска:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 47b8b7590be2d4b235bb04fe079b58cf65cb4ae7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866793"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="980a4-104">Тип ресурса Идентитирискевент</span><span class="sxs-lookup"><span data-stu-id="980a4-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="980a4-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="980a4-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="980a4-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="980a4-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="980a4-107">Событие риска, обнаруженное [защитой удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="980a4-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="980a4-108">Это базовый тип для каждого конкретного типа событий риска:</span><span class="sxs-lookup"><span data-stu-id="980a4-108">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="980a4-109">Тип события</span><span class="sxs-lookup"><span data-stu-id="980a4-109">Event type</span></span>         | <span data-ttu-id="980a4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="980a4-110">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="980a4-111">анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="980a4-111">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="980a4-112">Входы из анонимных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="980a4-112">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="980a4-113">малварерискевент</span><span class="sxs-lookup"><span data-stu-id="980a4-113">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="980a4-114">Входы с зараженных вредоносными программами устройств.</span><span class="sxs-lookup"><span data-stu-id="980a4-114">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="980a4-115">импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="980a4-115">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="980a4-116">Невозможность перемещаться к необычным расположениям.</span><span class="sxs-lookup"><span data-stu-id="980a4-116">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="980a4-117">леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="980a4-117">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="980a4-118">Пользователи с потерянными учетными данными.</span><span class="sxs-lookup"><span data-stu-id="980a4-118">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="980a4-119">суспиЦиаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="980a4-119">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="980a4-120">Входы из подозрительных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="980a4-120">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="980a4-121">унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="980a4-121">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="980a4-122">Входы из незнакомых расположений.</span><span class="sxs-lookup"><span data-stu-id="980a4-122">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="980a4-123">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="980a4-123">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="980a4-124">Методы</span><span class="sxs-lookup"><span data-stu-id="980a4-124">Methods</span></span>

| <span data-ttu-id="980a4-125">Метод</span><span class="sxs-lookup"><span data-stu-id="980a4-125">Method</span></span>           | <span data-ttu-id="980a4-126">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="980a4-126">Return Type</span></span>    |<span data-ttu-id="980a4-127">Описание</span><span class="sxs-lookup"><span data-stu-id="980a4-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="980a4-128">Получение объекта identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="980a4-128">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="980a4-129">идентитирискевент</span><span class="sxs-lookup"><span data-stu-id="980a4-129">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="980a4-130">Чтение свойств и связей объекта Идентитирискевент.</span><span class="sxs-lookup"><span data-stu-id="980a4-130">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="980a4-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="980a4-131">Properties</span></span>
| <span data-ttu-id="980a4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="980a4-132">Property</span></span>     | <span data-ttu-id="980a4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="980a4-133">Type</span></span>   |<span data-ttu-id="980a4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="980a4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="980a4-135">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="980a4-135">closedDateTime</span></span>|<span data-ttu-id="980a4-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="980a4-136">dateTimeOffset</span></span>| <span data-ttu-id="980a4-137">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="980a4-137">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="980a4-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="980a4-138">createdDateTime</span></span>|<span data-ttu-id="980a4-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="980a4-139">dateTimeOffset</span></span>| <span data-ttu-id="980a4-140">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="980a4-140">The date and time that the risk event was created.</span></span> <span data-ttu-id="980a4-141">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="980a4-141">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="980a4-142">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="980a4-142">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="980a4-143">id</span><span class="sxs-lookup"><span data-stu-id="980a4-143">id</span></span>|<span data-ttu-id="980a4-144">string</span><span class="sxs-lookup"><span data-stu-id="980a4-144">string</span></span>| <span data-ttu-id="980a4-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="980a4-145">Read-only</span></span>|
|<span data-ttu-id="980a4-146">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="980a4-146">riskEventDateTime</span></span>|<span data-ttu-id="980a4-147">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="980a4-147">dateTimeOffset</span></span>| <span data-ttu-id="980a4-148">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="980a4-148">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="980a4-149">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="980a4-149">riskEventStatus</span></span>|<span data-ttu-id="980a4-150">string</span><span class="sxs-lookup"><span data-stu-id="980a4-150">string</span></span>| <span data-ttu-id="980a4-151">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="980a4-151">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="980a4-152">riskLevel</span><span class="sxs-lookup"><span data-stu-id="980a4-152">riskLevel</span></span>|<span data-ttu-id="980a4-153">string</span><span class="sxs-lookup"><span data-stu-id="980a4-153">string</span></span>| <span data-ttu-id="980a4-154">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="980a4-154">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="980a4-155">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="980a4-155">riskEventType</span></span>|<span data-ttu-id="980a4-156">string</span><span class="sxs-lookup"><span data-stu-id="980a4-156">string</span></span>| <span data-ttu-id="980a4-157">Тип риска</span><span class="sxs-lookup"><span data-stu-id="980a4-157">The type of risk</span></span>|
|<span data-ttu-id="980a4-158">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="980a4-158">userDisplayName</span></span>|<span data-ttu-id="980a4-159">string</span><span class="sxs-lookup"><span data-stu-id="980a4-159">string</span></span>| <span data-ttu-id="980a4-160">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="980a4-160">The name of the user at risk</span></span>|
|<span data-ttu-id="980a4-161">userId</span><span class="sxs-lookup"><span data-stu-id="980a4-161">userId</span></span>|<span data-ttu-id="980a4-162">строка</span><span class="sxs-lookup"><span data-stu-id="980a4-162">string</span></span>| <span data-ttu-id="980a4-163">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="980a4-163">The id of the user at risk</span></span>|
|<span data-ttu-id="980a4-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="980a4-164">userPrincipalName</span></span>|<span data-ttu-id="980a4-165">string</span><span class="sxs-lookup"><span data-stu-id="980a4-165">string</span></span>| <span data-ttu-id="980a4-166">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="980a4-166">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="980a4-167">Отношения</span><span class="sxs-lookup"><span data-stu-id="980a4-167">Relationships</span></span>
| <span data-ttu-id="980a4-168">Связь</span><span class="sxs-lookup"><span data-stu-id="980a4-168">Relationship</span></span> | <span data-ttu-id="980a4-169">Тип</span><span class="sxs-lookup"><span data-stu-id="980a4-169">Type</span></span>   |<span data-ttu-id="980a4-170">Описание</span><span class="sxs-lookup"><span data-stu-id="980a4-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="980a4-171">импактедусер</span><span class="sxs-lookup"><span data-stu-id="980a4-171">impactedUser</span></span>|[<span data-ttu-id="980a4-172">user</span><span class="sxs-lookup"><span data-stu-id="980a4-172">user</span></span>](user.md)| <span data-ttu-id="980a4-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="980a4-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="980a4-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="980a4-175">JSON representation</span></span>

<span data-ttu-id="980a4-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="980a4-176">Here is a JSON representation of the resource.</span></span>

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
