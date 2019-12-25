---
title: Тип ресурса Анонимаусиприскевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором выполняется попытка входа учетной записи с IP-адреса, который является анонимным. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 205659f4ebc301824798cd39506cd73853c167ca
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870402"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="1cf07-104">Тип ресурса Анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="1cf07-104">anonymousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="1cf07-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="1cf07-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="1cf07-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="1cf07-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="1cf07-107">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) , в котором выполняется попытка входа учетной записи с IP-адреса, который является анонимным.</span><span class="sxs-lookup"><span data-stu-id="1cf07-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="1cf07-108">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="1cf07-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="1cf07-109">Методы</span><span class="sxs-lookup"><span data-stu-id="1cf07-109">Methods</span></span>

| <span data-ttu-id="1cf07-110">Метод</span><span class="sxs-lookup"><span data-stu-id="1cf07-110">Method</span></span>           | <span data-ttu-id="1cf07-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1cf07-111">Return Type</span></span>    |<span data-ttu-id="1cf07-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf07-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1cf07-113">Получение объекта anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1cf07-113">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="1cf07-114">анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="1cf07-114">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="1cf07-115">Чтение свойств и связей объекта Анонимаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="1cf07-115">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1cf07-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="1cf07-116">Properties</span></span>
| <span data-ttu-id="1cf07-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cf07-117">Property</span></span>     | <span data-ttu-id="1cf07-118">Тип</span><span class="sxs-lookup"><span data-stu-id="1cf07-118">Type</span></span>   |<span data-ttu-id="1cf07-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf07-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cf07-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cf07-120">closedDateTime</span></span>|<span data-ttu-id="1cf07-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cf07-121">dateTimeOffset</span></span>| <span data-ttu-id="1cf07-122">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="1cf07-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="1cf07-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cf07-123">createdDateTime</span></span>|<span data-ttu-id="1cf07-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cf07-124">dateTimeOffset</span></span>| <span data-ttu-id="1cf07-125">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="1cf07-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="1cf07-126">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="1cf07-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="1cf07-127">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="1cf07-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="1cf07-128">id</span><span class="sxs-lookup"><span data-stu-id="1cf07-128">id</span></span>|<span data-ttu-id="1cf07-129">string</span><span class="sxs-lookup"><span data-stu-id="1cf07-129">string</span></span>| <span data-ttu-id="1cf07-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="1cf07-130">Read-only</span></span>|
|<span data-ttu-id="1cf07-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1cf07-131">ipAddress</span></span>|<span data-ttu-id="1cf07-132">string</span><span class="sxs-lookup"><span data-stu-id="1cf07-132">string</span></span>| <span data-ttu-id="1cf07-133">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="1cf07-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="1cf07-134">location</span><span class="sxs-lookup"><span data-stu-id="1cf07-134">location</span></span>|<span data-ttu-id="1cf07-135">string</span><span class="sxs-lookup"><span data-stu-id="1cf07-135">string</span></span>| <span data-ttu-id="1cf07-136">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="1cf07-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="1cf07-137">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="1cf07-137">riskEventDateTime</span></span>|<span data-ttu-id="1cf07-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cf07-138">dateTimeOffset</span></span>| <span data-ttu-id="1cf07-139">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="1cf07-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="1cf07-140">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="1cf07-140">riskEventStatus</span></span>|<span data-ttu-id="1cf07-141">string</span><span class="sxs-lookup"><span data-stu-id="1cf07-141">string</span></span>| <span data-ttu-id="1cf07-142">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="1cf07-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="1cf07-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="1cf07-143">riskLevel</span></span>|<span data-ttu-id="1cf07-144">string</span><span class="sxs-lookup"><span data-stu-id="1cf07-144">string</span></span>| <span data-ttu-id="1cf07-145">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="1cf07-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="1cf07-146">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="1cf07-146">riskEventType</span></span>|<span data-ttu-id="1cf07-147">string</span><span class="sxs-lookup"><span data-stu-id="1cf07-147">string</span></span>| <span data-ttu-id="1cf07-148">Тип риска</span><span class="sxs-lookup"><span data-stu-id="1cf07-148">The type of risk</span></span>|
|<span data-ttu-id="1cf07-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1cf07-149">userDisplayName</span></span>|<span data-ttu-id="1cf07-150">string</span><span class="sxs-lookup"><span data-stu-id="1cf07-150">string</span></span>| <span data-ttu-id="1cf07-151">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="1cf07-151">The name of the user at risk</span></span>|
|<span data-ttu-id="1cf07-152">userId</span><span class="sxs-lookup"><span data-stu-id="1cf07-152">userId</span></span>|<span data-ttu-id="1cf07-153">строка</span><span class="sxs-lookup"><span data-stu-id="1cf07-153">string</span></span>| <span data-ttu-id="1cf07-154">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="1cf07-154">The id of the user at risk</span></span>|
|<span data-ttu-id="1cf07-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1cf07-155">userPrincipalName</span></span>|<span data-ttu-id="1cf07-156">string</span><span class="sxs-lookup"><span data-stu-id="1cf07-156">string</span></span>| <span data-ttu-id="1cf07-157">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="1cf07-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cf07-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="1cf07-158">Relationships</span></span>
| <span data-ttu-id="1cf07-159">Связь</span><span class="sxs-lookup"><span data-stu-id="1cf07-159">Relationship</span></span> | <span data-ttu-id="1cf07-160">Тип</span><span class="sxs-lookup"><span data-stu-id="1cf07-160">Type</span></span>   |<span data-ttu-id="1cf07-161">Описание</span><span class="sxs-lookup"><span data-stu-id="1cf07-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cf07-162">импактедусер</span><span class="sxs-lookup"><span data-stu-id="1cf07-162">impactedUser</span></span>|[<span data-ttu-id="1cf07-163">user</span><span class="sxs-lookup"><span data-stu-id="1cf07-163">user</span></span>](user.md)| <span data-ttu-id="1cf07-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1cf07-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cf07-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1cf07-166">JSON representation</span></span>

<span data-ttu-id="1cf07-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cf07-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
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
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
