---
title: Тип ресурса СуспиЦиаусиприскевент
description: Событие риска, обнаруженное при попытке входа учетной записи с подозрительным IP-адресом с помощью средства защиты удостоверений Azure Active Directory. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 68952fb80906a90c62798422d3fc302336311cab
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406067"
---
# <a name="suspiciousipriskevent-resource-type-deprecated"></a><span data-ttu-id="65042-104">Тип ресурса СуспиЦиаусиприскевент (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="65042-104">suspiciousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="65042-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65042-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="65042-106">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="65042-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="65042-107">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="65042-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="65042-108">Событие риска, обнаруженное при попытке входа учетной записи с подозрительным IP-адресом с помощью средства [защиты удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) .</span><span class="sxs-lookup"><span data-stu-id="65042-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from a suspicious IP address.</span></span> <span data-ttu-id="65042-109">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="65042-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="65042-110">Методы</span><span class="sxs-lookup"><span data-stu-id="65042-110">Methods</span></span>

| <span data-ttu-id="65042-111">Метод</span><span class="sxs-lookup"><span data-stu-id="65042-111">Method</span></span>           | <span data-ttu-id="65042-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65042-112">Return Type</span></span>    |<span data-ttu-id="65042-113">Описание</span><span class="sxs-lookup"><span data-stu-id="65042-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65042-114">Получение объекта suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="65042-114">Get suspiciousIpRiskEvent</span></span>](../api/suspiciousipriskevent-get.md) | [<span data-ttu-id="65042-115">суспиЦиаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="65042-115">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) |<span data-ttu-id="65042-116">Чтение свойств и связей объекта СуспиЦиаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="65042-116">Read properties and relationships of suspiciousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="65042-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="65042-117">Properties</span></span>
| <span data-ttu-id="65042-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="65042-118">Property</span></span>     | <span data-ttu-id="65042-119">Тип</span><span class="sxs-lookup"><span data-stu-id="65042-119">Type</span></span>   |<span data-ttu-id="65042-120">Описание</span><span class="sxs-lookup"><span data-stu-id="65042-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65042-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="65042-121">closedDateTime</span></span>|<span data-ttu-id="65042-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65042-122">dateTimeOffset</span></span>| <span data-ttu-id="65042-123">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="65042-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="65042-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65042-124">createdDateTime</span></span>|<span data-ttu-id="65042-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65042-125">dateTimeOffset</span></span>| <span data-ttu-id="65042-126">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="65042-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="65042-127">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="65042-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="65042-128">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="65042-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="65042-129">id</span><span class="sxs-lookup"><span data-stu-id="65042-129">id</span></span>|<span data-ttu-id="65042-130">string</span><span class="sxs-lookup"><span data-stu-id="65042-130">string</span></span>| <span data-ttu-id="65042-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="65042-131">Read-only</span></span>|
|<span data-ttu-id="65042-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="65042-132">ipAddress</span></span>|<span data-ttu-id="65042-133">string</span><span class="sxs-lookup"><span data-stu-id="65042-133">string</span></span>| <span data-ttu-id="65042-134">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="65042-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="65042-135">location</span><span class="sxs-lookup"><span data-stu-id="65042-135">location</span></span>|<span data-ttu-id="65042-136">string</span><span class="sxs-lookup"><span data-stu-id="65042-136">string</span></span>| <span data-ttu-id="65042-137">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="65042-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="65042-138">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="65042-138">riskEventDateTime</span></span>|<span data-ttu-id="65042-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65042-139">dateTimeOffset</span></span>| <span data-ttu-id="65042-140">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="65042-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="65042-141">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="65042-141">riskEventStatus</span></span>|<span data-ttu-id="65042-142">string</span><span class="sxs-lookup"><span data-stu-id="65042-142">string</span></span>| <span data-ttu-id="65042-143">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="65042-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="65042-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="65042-144">riskLevel</span></span>|<span data-ttu-id="65042-145">string</span><span class="sxs-lookup"><span data-stu-id="65042-145">string</span></span>| <span data-ttu-id="65042-146">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="65042-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="65042-147">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="65042-147">riskEventType</span></span>|<span data-ttu-id="65042-148">string</span><span class="sxs-lookup"><span data-stu-id="65042-148">string</span></span>| <span data-ttu-id="65042-149">Тип риска</span><span class="sxs-lookup"><span data-stu-id="65042-149">The type of risk</span></span>|
|<span data-ttu-id="65042-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="65042-150">userDisplayName</span></span>|<span data-ttu-id="65042-151">string</span><span class="sxs-lookup"><span data-stu-id="65042-151">string</span></span>| <span data-ttu-id="65042-152">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="65042-152">The name of the user at risk</span></span>|
|<span data-ttu-id="65042-153">userId</span><span class="sxs-lookup"><span data-stu-id="65042-153">userId</span></span>|<span data-ttu-id="65042-154">строка</span><span class="sxs-lookup"><span data-stu-id="65042-154">string</span></span>| <span data-ttu-id="65042-155">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="65042-155">The id of the user at risk</span></span>|
|<span data-ttu-id="65042-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65042-156">userPrincipalName</span></span>|<span data-ttu-id="65042-157">string</span><span class="sxs-lookup"><span data-stu-id="65042-157">string</span></span>| <span data-ttu-id="65042-158">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="65042-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="65042-159">Связи</span><span class="sxs-lookup"><span data-stu-id="65042-159">Relationships</span></span>
| <span data-ttu-id="65042-160">Связь</span><span class="sxs-lookup"><span data-stu-id="65042-160">Relationship</span></span> | <span data-ttu-id="65042-161">Тип</span><span class="sxs-lookup"><span data-stu-id="65042-161">Type</span></span>   |<span data-ttu-id="65042-162">Описание</span><span class="sxs-lookup"><span data-stu-id="65042-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65042-163">импактедусер</span><span class="sxs-lookup"><span data-stu-id="65042-163">impactedUser</span></span>|[<span data-ttu-id="65042-164">user</span><span class="sxs-lookup"><span data-stu-id="65042-164">user</span></span>](user.md)| <span data-ttu-id="65042-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="65042-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65042-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65042-167">JSON representation</span></span>

<span data-ttu-id="65042-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65042-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
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
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->