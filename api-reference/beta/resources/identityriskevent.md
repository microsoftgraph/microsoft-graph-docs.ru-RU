---
title: Тип ресурса identityRiskEvent
description: 'Событие риск, обнаруживается Azure Active Directory защиту. Это базовый тип для каждого типа события, определенные риски:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514182"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="f4fbd-104">Тип ресурса identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f4fbd-104">identityRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4fbd-105">Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="f4fbd-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="f4fbd-106">Это базовый тип для каждого типа события, определенные риски:</span><span class="sxs-lookup"><span data-stu-id="f4fbd-106">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="f4fbd-107">Тип события</span><span class="sxs-lookup"><span data-stu-id="f4fbd-107">Event type</span></span>         | <span data-ttu-id="f4fbd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fbd-108">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="f4fbd-109">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f4fbd-109">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="f4fbd-110">Войти в систему с анонимным IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-110">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="f4fbd-111">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f4fbd-111">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="f4fbd-112">Войти в систему с помощью устройств зараженный вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-112">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="f4fbd-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f4fbd-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="f4fbd-114">Невозможно поездок в необычных расположений.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-114">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="f4fbd-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f4fbd-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="f4fbd-116">Пользователи с учетными данными утечки.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-116">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="f4fbd-117">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f4fbd-117">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="f4fbd-118">Войти в систему с подозрительные IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-118">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="f4fbd-119">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f4fbd-119">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="f4fbd-120">Войти в систему из незнакомы расположений.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-120">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="f4fbd-121">Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="f4fbd-121">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="f4fbd-122">Методы</span><span class="sxs-lookup"><span data-stu-id="f4fbd-122">Methods</span></span>

| <span data-ttu-id="f4fbd-123">Метод</span><span class="sxs-lookup"><span data-stu-id="f4fbd-123">Method</span></span>           | <span data-ttu-id="f4fbd-124">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f4fbd-124">Return Type</span></span>    |<span data-ttu-id="f4fbd-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fbd-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4fbd-126">Получение identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f4fbd-126">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="f4fbd-127">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f4fbd-127">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="f4fbd-128">Чтение свойства и связи объекта identityRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-128">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4fbd-129">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4fbd-129">Properties</span></span>
| <span data-ttu-id="f4fbd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4fbd-130">Property</span></span>     | <span data-ttu-id="f4fbd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f4fbd-131">Type</span></span>   |<span data-ttu-id="f4fbd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fbd-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4fbd-133">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4fbd-133">closedDateTime</span></span>|<span data-ttu-id="f4fbd-134">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4fbd-134">dateTimeOffset</span></span>| <span data-ttu-id="f4fbd-135">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="f4fbd-135">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="f4fbd-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4fbd-136">createdDateTime</span></span>|<span data-ttu-id="f4fbd-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4fbd-137">dateTimeOffset</span></span>| <span data-ttu-id="f4fbd-138">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-138">The date and time that the risk event was created.</span></span> <span data-ttu-id="f4fbd-139">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-139">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="f4fbd-140">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-140">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="f4fbd-141">id</span><span class="sxs-lookup"><span data-stu-id="f4fbd-141">id</span></span>|<span data-ttu-id="f4fbd-142">string</span><span class="sxs-lookup"><span data-stu-id="f4fbd-142">string</span></span>| <span data-ttu-id="f4fbd-143">Только чтение</span><span class="sxs-lookup"><span data-stu-id="f4fbd-143">Read-only</span></span>|
|<span data-ttu-id="f4fbd-144">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="f4fbd-144">riskEventDateTime</span></span>|<span data-ttu-id="f4fbd-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4fbd-145">dateTimeOffset</span></span>| <span data-ttu-id="f4fbd-146">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="f4fbd-146">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="f4fbd-147">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="f4fbd-147">riskEventStatus</span></span>|<span data-ttu-id="f4fbd-148">string</span><span class="sxs-lookup"><span data-stu-id="f4fbd-148">string</span></span>| <span data-ttu-id="f4fbd-149">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-149">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="f4fbd-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f4fbd-150">riskLevel</span></span>|<span data-ttu-id="f4fbd-151">string</span><span class="sxs-lookup"><span data-stu-id="f4fbd-151">string</span></span>| <span data-ttu-id="f4fbd-152">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-152">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="f4fbd-153">riskEventType</span><span class="sxs-lookup"><span data-stu-id="f4fbd-153">riskEventType</span></span>|<span data-ttu-id="f4fbd-154">string</span><span class="sxs-lookup"><span data-stu-id="f4fbd-154">string</span></span>| <span data-ttu-id="f4fbd-155">Тип риска</span><span class="sxs-lookup"><span data-stu-id="f4fbd-155">The type of risk</span></span>|
|<span data-ttu-id="f4fbd-156">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4fbd-156">userDisplayName</span></span>|<span data-ttu-id="f4fbd-157">string</span><span class="sxs-lookup"><span data-stu-id="f4fbd-157">string</span></span>| <span data-ttu-id="f4fbd-158">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="f4fbd-158">The name of the user at risk</span></span>|
|<span data-ttu-id="f4fbd-159">userId</span><span class="sxs-lookup"><span data-stu-id="f4fbd-159">userId</span></span>|<span data-ttu-id="f4fbd-160">string</span><span class="sxs-lookup"><span data-stu-id="f4fbd-160">string</span></span>| <span data-ttu-id="f4fbd-161">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="f4fbd-161">The id of the user at risk</span></span>|
|<span data-ttu-id="f4fbd-162">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4fbd-162">userPrincipalName</span></span>|<span data-ttu-id="f4fbd-163">string</span><span class="sxs-lookup"><span data-stu-id="f4fbd-163">string</span></span>| <span data-ttu-id="f4fbd-164">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="f4fbd-164">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4fbd-165">Отношения</span><span class="sxs-lookup"><span data-stu-id="f4fbd-165">Relationships</span></span>
| <span data-ttu-id="f4fbd-166">Связь</span><span class="sxs-lookup"><span data-stu-id="f4fbd-166">Relationship</span></span> | <span data-ttu-id="f4fbd-167">Тип</span><span class="sxs-lookup"><span data-stu-id="f4fbd-167">Type</span></span>   |<span data-ttu-id="f4fbd-168">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fbd-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4fbd-169">impactedUser</span><span class="sxs-lookup"><span data-stu-id="f4fbd-169">impactedUser</span></span>|[<span data-ttu-id="f4fbd-170">user</span><span class="sxs-lookup"><span data-stu-id="f4fbd-170">user</span></span>](user.md)| <span data-ttu-id="f4fbd-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4fbd-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4fbd-173">JSON representation</span></span>

<span data-ttu-id="f4fbd-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4fbd-174">Here is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/identityriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
