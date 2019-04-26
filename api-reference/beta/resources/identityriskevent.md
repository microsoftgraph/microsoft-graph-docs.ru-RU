---
title: Тип ресурса Идентитирискевент
description: 'Событие риска, обнаруженное защитой удостоверений Azure Active Directory. Это базовый тип для каждого конкретного типа событий риска:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 654b6380120c0584045d3267bddffb9db88a39aa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340010"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="36e2d-104">Тип ресурса Идентитирискевент</span><span class="sxs-lookup"><span data-stu-id="36e2d-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36e2d-105">Событие риска, обнаруженное [защитОй удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="36e2d-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="36e2d-106">Это базовый тип для каждого конкретного типа событий риска:</span><span class="sxs-lookup"><span data-stu-id="36e2d-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="36e2d-107">Тип события</span><span class="sxs-lookup"><span data-stu-id="36e2d-107">Event type</span></span>         | <span data-ttu-id="36e2d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="36e2d-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="36e2d-109">Анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="36e2d-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="36e2d-110">Входы из анонимных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="36e2d-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="36e2d-111">Малварерискевент</span><span class="sxs-lookup"><span data-stu-id="36e2d-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="36e2d-112">Входы с зараженных вредоносными программами устройств.</span><span class="sxs-lookup"><span data-stu-id="36e2d-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="36e2d-113">Импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="36e2d-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="36e2d-114">НеВозможность перемещаться к необычным расположениям.</span><span class="sxs-lookup"><span data-stu-id="36e2d-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="36e2d-115">Леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="36e2d-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="36e2d-116">Пользователи с потерянными учетными данными.</span><span class="sxs-lookup"><span data-stu-id="36e2d-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="36e2d-117">СуспиЦиаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="36e2d-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="36e2d-118">Входы из подозрительных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="36e2d-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="36e2d-119">Унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="36e2d-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="36e2d-120">Входы из незнакомых расположений.</span><span class="sxs-lookup"><span data-stu-id="36e2d-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="36e2d-121">Полную информацию о событиях риска можно найти в [документации по защите удостоверенИй Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="36e2d-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="36e2d-122">Методы</span><span class="sxs-lookup"><span data-stu-id="36e2d-122">Methods</span></span>

| <span data-ttu-id="36e2d-123">Метод</span><span class="sxs-lookup"><span data-stu-id="36e2d-123">Method</span></span>           | <span data-ttu-id="36e2d-124">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="36e2d-124">Return Type</span></span>    |<span data-ttu-id="36e2d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="36e2d-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36e2d-126">Получение объекта identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="36e2d-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="36e2d-127">Идентитирискевент</span><span class="sxs-lookup"><span data-stu-id="36e2d-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="36e2d-128">Чтение свойств и связей объекта Идентитирискевент.</span><span class="sxs-lookup"><span data-stu-id="36e2d-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="36e2d-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="36e2d-129">Properties</span></span>
| <span data-ttu-id="36e2d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="36e2d-130">Property</span></span>     | <span data-ttu-id="36e2d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="36e2d-131">Type</span></span>   |<span data-ttu-id="36e2d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="36e2d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36e2d-133">Клоседдатетиме</span><span class="sxs-lookup"><span data-stu-id="36e2d-133">closedDateTime</span></span>|<span data-ttu-id="36e2d-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36e2d-134">dateTimeOffset</span></span>| <span data-ttu-id="36e2d-135">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="36e2d-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="36e2d-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36e2d-136">createdDateTime</span></span>|<span data-ttu-id="36e2d-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36e2d-137">dateTimeOffset</span></span>| <span data-ttu-id="36e2d-138">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="36e2d-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="36e2d-139">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="36e2d-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="36e2d-140">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="36e2d-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="36e2d-141">id</span><span class="sxs-lookup"><span data-stu-id="36e2d-141">id</span></span>|<span data-ttu-id="36e2d-142">строка</span><span class="sxs-lookup"><span data-stu-id="36e2d-142">string</span></span>| <span data-ttu-id="36e2d-143">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="36e2d-143">Read-only</span></span>|
|<span data-ttu-id="36e2d-144">Рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="36e2d-144">riskEventDateTime</span></span>|<span data-ttu-id="36e2d-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36e2d-145">dateTimeOffset</span></span>| <span data-ttu-id="36e2d-146">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="36e2d-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="36e2d-147">Рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="36e2d-147">riskEventStatus</span></span>|<span data-ttu-id="36e2d-148">string</span><span class="sxs-lookup"><span data-stu-id="36e2d-148">string</span></span>| <span data-ttu-id="36e2d-149">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="36e2d-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="36e2d-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="36e2d-150">riskLevel</span></span>|<span data-ttu-id="36e2d-151">string</span><span class="sxs-lookup"><span data-stu-id="36e2d-151">string</span></span>| <span data-ttu-id="36e2d-152">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="36e2d-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="36e2d-153">Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="36e2d-153">riskEventType</span></span>|<span data-ttu-id="36e2d-154">string</span><span class="sxs-lookup"><span data-stu-id="36e2d-154">string</span></span>| <span data-ttu-id="36e2d-155">Тип риска</span><span class="sxs-lookup"><span data-stu-id="36e2d-155">The type of risk</span></span>|
|<span data-ttu-id="36e2d-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="36e2d-156">userDisplayName</span></span>|<span data-ttu-id="36e2d-157">string</span><span class="sxs-lookup"><span data-stu-id="36e2d-157">string</span></span>| <span data-ttu-id="36e2d-158">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="36e2d-158">The name of the user at risk</span></span>|
|<span data-ttu-id="36e2d-159">userId</span><span class="sxs-lookup"><span data-stu-id="36e2d-159">userId</span></span>|<span data-ttu-id="36e2d-160">string</span><span class="sxs-lookup"><span data-stu-id="36e2d-160">string</span></span>| <span data-ttu-id="36e2d-161">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="36e2d-161">The id of the user at risk</span></span>|
|<span data-ttu-id="36e2d-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="36e2d-162">userPrincipalName</span></span>|<span data-ttu-id="36e2d-163">string</span><span class="sxs-lookup"><span data-stu-id="36e2d-163">string</span></span>| <span data-ttu-id="36e2d-164">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="36e2d-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="36e2d-165">Отношения</span><span class="sxs-lookup"><span data-stu-id="36e2d-165">Relationships</span></span>
| <span data-ttu-id="36e2d-166">Отношение</span><span class="sxs-lookup"><span data-stu-id="36e2d-166">Relationship</span></span> | <span data-ttu-id="36e2d-167">Тип</span><span class="sxs-lookup"><span data-stu-id="36e2d-167">Type</span></span>   |<span data-ttu-id="36e2d-168">Описание</span><span class="sxs-lookup"><span data-stu-id="36e2d-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36e2d-169">Импактедусер</span><span class="sxs-lookup"><span data-stu-id="36e2d-169">impactedUser</span></span>|[<span data-ttu-id="36e2d-170">user</span><span class="sxs-lookup"><span data-stu-id="36e2d-170">user</span></span>](user.md)| <span data-ttu-id="36e2d-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="36e2d-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36e2d-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36e2d-173">JSON representation</span></span>

<span data-ttu-id="36e2d-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36e2d-174">Here is a JSON representation of the resource.</span></span> 

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
