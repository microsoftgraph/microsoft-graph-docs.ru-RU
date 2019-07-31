---
title: Тип ресурса Идентитирискевент
description: 'Событие риска, обнаруженное защитой удостоверений Azure Active Directory. Это базовый тип для каждого конкретного типа событий риска:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 7ea0a11931021e828660cc7b03991b8ea96ef1f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005802"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="e82a3-104">Тип ресурса Идентитирискевент</span><span class="sxs-lookup"><span data-stu-id="e82a3-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e82a3-105">Событие риска, обнаруженное [защитой удостоверений Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="e82a3-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="e82a3-106">Это базовый тип для каждого конкретного типа событий риска:</span><span class="sxs-lookup"><span data-stu-id="e82a3-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="e82a3-107">Тип события</span><span class="sxs-lookup"><span data-stu-id="e82a3-107">Event type</span></span>         | <span data-ttu-id="e82a3-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e82a3-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="e82a3-109">Анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="e82a3-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="e82a3-110">Входы из анонимных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="e82a3-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="e82a3-111">Малварерискевент</span><span class="sxs-lookup"><span data-stu-id="e82a3-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="e82a3-112">Входы с зараженных вредоносными программами устройств.</span><span class="sxs-lookup"><span data-stu-id="e82a3-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="e82a3-113">Импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="e82a3-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="e82a3-114">Невозможность перемещаться к необычным расположениям.</span><span class="sxs-lookup"><span data-stu-id="e82a3-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="e82a3-115">Леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="e82a3-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="e82a3-116">Пользователи с потерянными учетными данными.</span><span class="sxs-lookup"><span data-stu-id="e82a3-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="e82a3-117">СуспиЦиаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="e82a3-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="e82a3-118">Входы из подозрительных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="e82a3-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="e82a3-119">Унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="e82a3-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="e82a3-120">Входы из незнакомых расположений.</span><span class="sxs-lookup"><span data-stu-id="e82a3-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="e82a3-121">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="e82a3-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="e82a3-122">Методы</span><span class="sxs-lookup"><span data-stu-id="e82a3-122">Methods</span></span>

| <span data-ttu-id="e82a3-123">Метод</span><span class="sxs-lookup"><span data-stu-id="e82a3-123">Method</span></span>           | <span data-ttu-id="e82a3-124">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e82a3-124">Return Type</span></span>    |<span data-ttu-id="e82a3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="e82a3-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e82a3-126">Получение объекта identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e82a3-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="e82a3-127">Идентитирискевент</span><span class="sxs-lookup"><span data-stu-id="e82a3-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="e82a3-128">Чтение свойств и связей объекта Идентитирискевент.</span><span class="sxs-lookup"><span data-stu-id="e82a3-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e82a3-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="e82a3-129">Properties</span></span>
| <span data-ttu-id="e82a3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e82a3-130">Property</span></span>     | <span data-ttu-id="e82a3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e82a3-131">Type</span></span>   |<span data-ttu-id="e82a3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e82a3-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e82a3-133">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="e82a3-133">closedDateTime</span></span>|<span data-ttu-id="e82a3-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e82a3-134">dateTimeOffset</span></span>| <span data-ttu-id="e82a3-135">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="e82a3-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="e82a3-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e82a3-136">createdDateTime</span></span>|<span data-ttu-id="e82a3-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e82a3-137">dateTimeOffset</span></span>| <span data-ttu-id="e82a3-138">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="e82a3-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="e82a3-139">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="e82a3-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="e82a3-140">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="e82a3-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="e82a3-141">id</span><span class="sxs-lookup"><span data-stu-id="e82a3-141">id</span></span>|<span data-ttu-id="e82a3-142">string</span><span class="sxs-lookup"><span data-stu-id="e82a3-142">string</span></span>| <span data-ttu-id="e82a3-143">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="e82a3-143">Read-only</span></span>|
|<span data-ttu-id="e82a3-144">Рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="e82a3-144">riskEventDateTime</span></span>|<span data-ttu-id="e82a3-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e82a3-145">dateTimeOffset</span></span>| <span data-ttu-id="e82a3-146">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="e82a3-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="e82a3-147">Рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="e82a3-147">riskEventStatus</span></span>|<span data-ttu-id="e82a3-148">string</span><span class="sxs-lookup"><span data-stu-id="e82a3-148">string</span></span>| <span data-ttu-id="e82a3-149">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="e82a3-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="e82a3-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e82a3-150">riskLevel</span></span>|<span data-ttu-id="e82a3-151">string</span><span class="sxs-lookup"><span data-stu-id="e82a3-151">string</span></span>| <span data-ttu-id="e82a3-152">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e82a3-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e82a3-153">Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="e82a3-153">riskEventType</span></span>|<span data-ttu-id="e82a3-154">string</span><span class="sxs-lookup"><span data-stu-id="e82a3-154">string</span></span>| <span data-ttu-id="e82a3-155">Тип риска</span><span class="sxs-lookup"><span data-stu-id="e82a3-155">The type of risk</span></span>|
|<span data-ttu-id="e82a3-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e82a3-156">userDisplayName</span></span>|<span data-ttu-id="e82a3-157">string</span><span class="sxs-lookup"><span data-stu-id="e82a3-157">string</span></span>| <span data-ttu-id="e82a3-158">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="e82a3-158">The name of the user at risk</span></span>|
|<span data-ttu-id="e82a3-159">userId</span><span class="sxs-lookup"><span data-stu-id="e82a3-159">userId</span></span>|<span data-ttu-id="e82a3-160">string</span><span class="sxs-lookup"><span data-stu-id="e82a3-160">string</span></span>| <span data-ttu-id="e82a3-161">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="e82a3-161">The id of the user at risk</span></span>|
|<span data-ttu-id="e82a3-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e82a3-162">userPrincipalName</span></span>|<span data-ttu-id="e82a3-163">string</span><span class="sxs-lookup"><span data-stu-id="e82a3-163">string</span></span>| <span data-ttu-id="e82a3-164">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="e82a3-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="e82a3-165">Отношения</span><span class="sxs-lookup"><span data-stu-id="e82a3-165">Relationships</span></span>
| <span data-ttu-id="e82a3-166">Отношение</span><span class="sxs-lookup"><span data-stu-id="e82a3-166">Relationship</span></span> | <span data-ttu-id="e82a3-167">Тип</span><span class="sxs-lookup"><span data-stu-id="e82a3-167">Type</span></span>   |<span data-ttu-id="e82a3-168">Описание</span><span class="sxs-lookup"><span data-stu-id="e82a3-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e82a3-169">Импактедусер</span><span class="sxs-lookup"><span data-stu-id="e82a3-169">impactedUser</span></span>|[<span data-ttu-id="e82a3-170">user</span><span class="sxs-lookup"><span data-stu-id="e82a3-170">user</span></span>](user.md)| <span data-ttu-id="e82a3-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e82a3-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e82a3-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e82a3-173">JSON representation</span></span>

<span data-ttu-id="e82a3-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e82a3-174">Here is a JSON representation of the resource.</span></span> 

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
