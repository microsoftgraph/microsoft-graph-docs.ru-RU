---
title: Тип ресурса identityRiskEvent
description: 'Событие риск, обнаруживается Azure Active Directory защиту. Это базовый тип для каждого типа события, определенные риски:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: be5e4afaa5bf85581c904ed94f07433243651ee9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953653"
---
# <a name="identityriskevent-resource-type"></a><span data-ttu-id="34e00-104">Тип ресурса identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34e00-104">identityRiskEvent resource type</span></span>

> <span data-ttu-id="34e00-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34e00-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34e00-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34e00-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34e00-107">Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="34e00-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span> <span data-ttu-id="34e00-108">Это базовый тип для каждого типа события, определенные риски:</span><span class="sxs-lookup"><span data-stu-id="34e00-108">It is the base type for each specific risk event type:</span></span>

| <span data-ttu-id="34e00-109">Тип события</span><span class="sxs-lookup"><span data-stu-id="34e00-109">Event type</span></span>         | <span data-ttu-id="34e00-110">Описание</span><span class="sxs-lookup"><span data-stu-id="34e00-110">Description</span></span>|
|:---------------|:-----------|
|[<span data-ttu-id="34e00-111">anonymousipRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34e00-111">anonymousipRiskEvent</span></span>](anonymousipriskevent.md) | <span data-ttu-id="34e00-112">Войти в систему с анонимным IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="34e00-112">Sign-ins from anonymous IP addresses.</span></span> |
|[<span data-ttu-id="34e00-113">malwareRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34e00-113">malwareRiskEvent</span></span>](malwareriskevent.md) | <span data-ttu-id="34e00-114">Войти в систему с помощью устройств зараженный вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="34e00-114">Sign-ins from malware-infected devices.</span></span> |
|[<span data-ttu-id="34e00-115">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34e00-115">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) | <span data-ttu-id="34e00-116">Невозможно поездок в необычных расположений.</span><span class="sxs-lookup"><span data-stu-id="34e00-116">Impossible travel to atypical locations.</span></span> |
|[<span data-ttu-id="34e00-117">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34e00-117">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) | <span data-ttu-id="34e00-118">Пользователи с учетными данными утечки.</span><span class="sxs-lookup"><span data-stu-id="34e00-118">Users with leaked credentials.</span></span> |
|[<span data-ttu-id="34e00-119">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34e00-119">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) | <span data-ttu-id="34e00-120">Войти в систему с подозрительные IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="34e00-120">Sign-ins from suspicious IP addresses.</span></span> |
|[<span data-ttu-id="34e00-121">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34e00-121">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) | <span data-ttu-id="34e00-122">Войти в систему из незнакомы расположений.</span><span class="sxs-lookup"><span data-stu-id="34e00-122">Sign-ins from unfamiliar locations.</span></span> |

<span data-ttu-id="34e00-123">Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span><span class="sxs-lookup"><span data-stu-id="34e00-123">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).</span></span>

## <a name="methods"></a><span data-ttu-id="34e00-124">Методы</span><span class="sxs-lookup"><span data-stu-id="34e00-124">Methods</span></span>

| <span data-ttu-id="34e00-125">Метод</span><span class="sxs-lookup"><span data-stu-id="34e00-125">Method</span></span>           | <span data-ttu-id="34e00-126">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="34e00-126">Return Type</span></span>    |<span data-ttu-id="34e00-127">Описание</span><span class="sxs-lookup"><span data-stu-id="34e00-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="34e00-128">Получение identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34e00-128">Get identityRiskEvent</span></span>](../api/identityriskevent-get.md) | [<span data-ttu-id="34e00-129">identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34e00-129">identityRiskEvent</span></span>](identityriskevent.md) |<span data-ttu-id="34e00-130">Чтение свойства и связи объекта identityRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="34e00-130">Read properties and relationships of identityRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="34e00-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="34e00-131">Properties</span></span>
| <span data-ttu-id="34e00-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="34e00-132">Property</span></span>     | <span data-ttu-id="34e00-133">Тип</span><span class="sxs-lookup"><span data-stu-id="34e00-133">Type</span></span>   |<span data-ttu-id="34e00-134">Описание</span><span class="sxs-lookup"><span data-stu-id="34e00-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34e00-135">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="34e00-135">closedDateTime</span></span>|<span data-ttu-id="34e00-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34e00-136">dateTimeOffset</span></span>| <span data-ttu-id="34e00-137">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="34e00-137">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="34e00-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34e00-138">createdDateTime</span></span>|<span data-ttu-id="34e00-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34e00-139">dateTimeOffset</span></span>| <span data-ttu-id="34e00-140">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="34e00-140">The date and time that the risk event was created.</span></span> <span data-ttu-id="34e00-141">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="34e00-141">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="34e00-142">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="34e00-142">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="34e00-143">id</span><span class="sxs-lookup"><span data-stu-id="34e00-143">id</span></span>|<span data-ttu-id="34e00-144">строка</span><span class="sxs-lookup"><span data-stu-id="34e00-144">string</span></span>| <span data-ttu-id="34e00-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="34e00-145">Read-only</span></span>|
|<span data-ttu-id="34e00-146">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="34e00-146">riskEventDateTime</span></span>|<span data-ttu-id="34e00-147">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34e00-147">dateTimeOffset</span></span>| <span data-ttu-id="34e00-148">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="34e00-148">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="34e00-149">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="34e00-149">riskEventStatus</span></span>|<span data-ttu-id="34e00-150">string</span><span class="sxs-lookup"><span data-stu-id="34e00-150">string</span></span>| <span data-ttu-id="34e00-151">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="34e00-151">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="34e00-152">riskLevel</span><span class="sxs-lookup"><span data-stu-id="34e00-152">riskLevel</span></span>|<span data-ttu-id="34e00-153">string</span><span class="sxs-lookup"><span data-stu-id="34e00-153">string</span></span>| <span data-ttu-id="34e00-154">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="34e00-154">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="34e00-155">riskEventType</span><span class="sxs-lookup"><span data-stu-id="34e00-155">riskEventType</span></span>|<span data-ttu-id="34e00-156">string</span><span class="sxs-lookup"><span data-stu-id="34e00-156">string</span></span>| <span data-ttu-id="34e00-157">Тип риска</span><span class="sxs-lookup"><span data-stu-id="34e00-157">The type of risk</span></span>|
|<span data-ttu-id="34e00-158">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="34e00-158">userDisplayName</span></span>|<span data-ttu-id="34e00-159">string</span><span class="sxs-lookup"><span data-stu-id="34e00-159">string</span></span>| <span data-ttu-id="34e00-160">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="34e00-160">The name of the user at risk</span></span>|
|<span data-ttu-id="34e00-161">userId</span><span class="sxs-lookup"><span data-stu-id="34e00-161">userId</span></span>|<span data-ttu-id="34e00-162">string</span><span class="sxs-lookup"><span data-stu-id="34e00-162">string</span></span>| <span data-ttu-id="34e00-163">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="34e00-163">The id of the user at risk</span></span>|
|<span data-ttu-id="34e00-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34e00-164">userPrincipalName</span></span>|<span data-ttu-id="34e00-165">string</span><span class="sxs-lookup"><span data-stu-id="34e00-165">string</span></span>| <span data-ttu-id="34e00-166">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="34e00-166">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="34e00-167">Связи</span><span class="sxs-lookup"><span data-stu-id="34e00-167">Relationships</span></span>
| <span data-ttu-id="34e00-168">Связь</span><span class="sxs-lookup"><span data-stu-id="34e00-168">Relationship</span></span> | <span data-ttu-id="34e00-169">Тип</span><span class="sxs-lookup"><span data-stu-id="34e00-169">Type</span></span>   |<span data-ttu-id="34e00-170">Описание</span><span class="sxs-lookup"><span data-stu-id="34e00-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34e00-171">impactedUser</span><span class="sxs-lookup"><span data-stu-id="34e00-171">impactedUser</span></span>|[<span data-ttu-id="34e00-172">user</span><span class="sxs-lookup"><span data-stu-id="34e00-172">user</span></span>](user.md)| <span data-ttu-id="34e00-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="34e00-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34e00-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34e00-175">JSON representation</span></span>

<span data-ttu-id="34e00-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34e00-176">Here is a JSON representation of the resource.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
