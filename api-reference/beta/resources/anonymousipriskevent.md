---
title: Тип ресурса Анонимаусиприскевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором выполняется попытка входа учетной записи с IP-адреса, который является анонимным. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 41d4109cb14053621baebd8383c522ad7e0ae3c0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807572"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="f43d5-104">Тип ресурса Анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="f43d5-104">anonymousIpRiskEvent resource type</span></span>

<span data-ttu-id="f43d5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f43d5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="f43d5-106">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="f43d5-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="f43d5-107">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="f43d5-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="f43d5-108">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) , в котором выполняется попытка входа учетной записи с IP-адреса, который является анонимным.</span><span class="sxs-lookup"><span data-stu-id="f43d5-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="f43d5-109">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="f43d5-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="f43d5-110">Методы</span><span class="sxs-lookup"><span data-stu-id="f43d5-110">Methods</span></span>

| <span data-ttu-id="f43d5-111">Метод</span><span class="sxs-lookup"><span data-stu-id="f43d5-111">Method</span></span>           | <span data-ttu-id="f43d5-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f43d5-112">Return Type</span></span>    |<span data-ttu-id="f43d5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f43d5-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f43d5-114">Получение объекта anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f43d5-114">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="f43d5-115">анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="f43d5-115">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="f43d5-116">Чтение свойств и связей объекта Анонимаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="f43d5-116">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f43d5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="f43d5-117">Properties</span></span>
| <span data-ttu-id="f43d5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="f43d5-118">Property</span></span>     | <span data-ttu-id="f43d5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f43d5-119">Type</span></span>   |<span data-ttu-id="f43d5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f43d5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f43d5-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f43d5-121">closedDateTime</span></span>|<span data-ttu-id="f43d5-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f43d5-122">dateTimeOffset</span></span>| <span data-ttu-id="f43d5-123">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="f43d5-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="f43d5-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f43d5-124">createdDateTime</span></span>|<span data-ttu-id="f43d5-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f43d5-125">dateTimeOffset</span></span>| <span data-ttu-id="f43d5-126">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="f43d5-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="f43d5-127">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="f43d5-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="f43d5-128">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="f43d5-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="f43d5-129">id</span><span class="sxs-lookup"><span data-stu-id="f43d5-129">id</span></span>|<span data-ttu-id="f43d5-130">string</span><span class="sxs-lookup"><span data-stu-id="f43d5-130">string</span></span>| <span data-ttu-id="f43d5-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="f43d5-131">Read-only</span></span>|
|<span data-ttu-id="f43d5-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f43d5-132">ipAddress</span></span>|<span data-ttu-id="f43d5-133">string</span><span class="sxs-lookup"><span data-stu-id="f43d5-133">string</span></span>| <span data-ttu-id="f43d5-134">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="f43d5-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="f43d5-135">location</span><span class="sxs-lookup"><span data-stu-id="f43d5-135">location</span></span>|<span data-ttu-id="f43d5-136">string</span><span class="sxs-lookup"><span data-stu-id="f43d5-136">string</span></span>| <span data-ttu-id="f43d5-137">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="f43d5-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="f43d5-138">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="f43d5-138">riskEventDateTime</span></span>|<span data-ttu-id="f43d5-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f43d5-139">dateTimeOffset</span></span>| <span data-ttu-id="f43d5-140">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="f43d5-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="f43d5-141">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="f43d5-141">riskEventStatus</span></span>|<span data-ttu-id="f43d5-142">string</span><span class="sxs-lookup"><span data-stu-id="f43d5-142">string</span></span>| <span data-ttu-id="f43d5-143">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="f43d5-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="f43d5-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f43d5-144">riskLevel</span></span>|<span data-ttu-id="f43d5-145">string</span><span class="sxs-lookup"><span data-stu-id="f43d5-145">string</span></span>| <span data-ttu-id="f43d5-146">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f43d5-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="f43d5-147">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="f43d5-147">riskEventType</span></span>|<span data-ttu-id="f43d5-148">string</span><span class="sxs-lookup"><span data-stu-id="f43d5-148">string</span></span>| <span data-ttu-id="f43d5-149">Тип риска</span><span class="sxs-lookup"><span data-stu-id="f43d5-149">The type of risk</span></span>|
|<span data-ttu-id="f43d5-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f43d5-150">userDisplayName</span></span>|<span data-ttu-id="f43d5-151">string</span><span class="sxs-lookup"><span data-stu-id="f43d5-151">string</span></span>| <span data-ttu-id="f43d5-152">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="f43d5-152">The name of the user at risk</span></span>|
|<span data-ttu-id="f43d5-153">userId</span><span class="sxs-lookup"><span data-stu-id="f43d5-153">userId</span></span>|<span data-ttu-id="f43d5-154">строка</span><span class="sxs-lookup"><span data-stu-id="f43d5-154">string</span></span>| <span data-ttu-id="f43d5-155">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="f43d5-155">The id of the user at risk</span></span>|
|<span data-ttu-id="f43d5-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f43d5-156">userPrincipalName</span></span>|<span data-ttu-id="f43d5-157">string</span><span class="sxs-lookup"><span data-stu-id="f43d5-157">string</span></span>| <span data-ttu-id="f43d5-158">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="f43d5-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="f43d5-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="f43d5-159">Relationships</span></span>
| <span data-ttu-id="f43d5-160">Связь</span><span class="sxs-lookup"><span data-stu-id="f43d5-160">Relationship</span></span> | <span data-ttu-id="f43d5-161">Тип</span><span class="sxs-lookup"><span data-stu-id="f43d5-161">Type</span></span>   |<span data-ttu-id="f43d5-162">Описание</span><span class="sxs-lookup"><span data-stu-id="f43d5-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f43d5-163">импактедусер</span><span class="sxs-lookup"><span data-stu-id="f43d5-163">impactedUser</span></span>|[<span data-ttu-id="f43d5-164">user</span><span class="sxs-lookup"><span data-stu-id="f43d5-164">user</span></span>](user.md)| <span data-ttu-id="f43d5-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f43d5-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f43d5-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f43d5-167">JSON representation</span></span>

<span data-ttu-id="f43d5-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f43d5-168">Here is a JSON representation of the resource.</span></span>

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
