---
title: Тип ресурса Анонимаусиприскевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором выполняется попытка входа учетной записи с IP-адреса, который является анонимным. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: bcbe25270f4752e7660ab4ce0c8b9d7d636c22e6
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405619"
---
# <a name="anonymousipriskevent-resource-type-deprecated"></a><span data-ttu-id="f2f70-104">Тип ресурса Анонимаусиприскевент (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="f2f70-104">anonymousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="f2f70-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2f70-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="f2f70-106">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="f2f70-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="f2f70-107">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="f2f70-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="f2f70-108">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) , в котором выполняется попытка входа учетной записи с IP-адреса, который является анонимным.</span><span class="sxs-lookup"><span data-stu-id="f2f70-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="f2f70-109">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="f2f70-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="f2f70-110">Методы</span><span class="sxs-lookup"><span data-stu-id="f2f70-110">Methods</span></span>

| <span data-ttu-id="f2f70-111">Метод</span><span class="sxs-lookup"><span data-stu-id="f2f70-111">Method</span></span>           | <span data-ttu-id="f2f70-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f2f70-112">Return Type</span></span>    |<span data-ttu-id="f2f70-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f70-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2f70-114">Получение объекта anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="f2f70-114">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="f2f70-115">анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="f2f70-115">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="f2f70-116">Чтение свойств и связей объекта Анонимаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="f2f70-116">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2f70-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2f70-117">Properties</span></span>
| <span data-ttu-id="f2f70-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2f70-118">Property</span></span>     | <span data-ttu-id="f2f70-119">Тип</span><span class="sxs-lookup"><span data-stu-id="f2f70-119">Type</span></span>   |<span data-ttu-id="f2f70-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f70-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2f70-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2f70-121">closedDateTime</span></span>|<span data-ttu-id="f2f70-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2f70-122">dateTimeOffset</span></span>| <span data-ttu-id="f2f70-123">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="f2f70-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="f2f70-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2f70-124">createdDateTime</span></span>|<span data-ttu-id="f2f70-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2f70-125">dateTimeOffset</span></span>| <span data-ttu-id="f2f70-126">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="f2f70-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="f2f70-127">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="f2f70-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="f2f70-128">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="f2f70-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="f2f70-129">id</span><span class="sxs-lookup"><span data-stu-id="f2f70-129">id</span></span>|<span data-ttu-id="f2f70-130">string</span><span class="sxs-lookup"><span data-stu-id="f2f70-130">string</span></span>| <span data-ttu-id="f2f70-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="f2f70-131">Read-only</span></span>|
|<span data-ttu-id="f2f70-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f2f70-132">ipAddress</span></span>|<span data-ttu-id="f2f70-133">string</span><span class="sxs-lookup"><span data-stu-id="f2f70-133">string</span></span>| <span data-ttu-id="f2f70-134">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="f2f70-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="f2f70-135">location</span><span class="sxs-lookup"><span data-stu-id="f2f70-135">location</span></span>|<span data-ttu-id="f2f70-136">string</span><span class="sxs-lookup"><span data-stu-id="f2f70-136">string</span></span>| <span data-ttu-id="f2f70-137">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="f2f70-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="f2f70-138">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="f2f70-138">riskEventDateTime</span></span>|<span data-ttu-id="f2f70-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2f70-139">dateTimeOffset</span></span>| <span data-ttu-id="f2f70-140">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="f2f70-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="f2f70-141">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="f2f70-141">riskEventStatus</span></span>|<span data-ttu-id="f2f70-142">string</span><span class="sxs-lookup"><span data-stu-id="f2f70-142">string</span></span>| <span data-ttu-id="f2f70-143">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="f2f70-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="f2f70-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f2f70-144">riskLevel</span></span>|<span data-ttu-id="f2f70-145">string</span><span class="sxs-lookup"><span data-stu-id="f2f70-145">string</span></span>| <span data-ttu-id="f2f70-146">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f2f70-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="f2f70-147">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="f2f70-147">riskEventType</span></span>|<span data-ttu-id="f2f70-148">string</span><span class="sxs-lookup"><span data-stu-id="f2f70-148">string</span></span>| <span data-ttu-id="f2f70-149">Тип риска</span><span class="sxs-lookup"><span data-stu-id="f2f70-149">The type of risk</span></span>|
|<span data-ttu-id="f2f70-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f2f70-150">userDisplayName</span></span>|<span data-ttu-id="f2f70-151">string</span><span class="sxs-lookup"><span data-stu-id="f2f70-151">string</span></span>| <span data-ttu-id="f2f70-152">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="f2f70-152">The name of the user at risk</span></span>|
|<span data-ttu-id="f2f70-153">userId</span><span class="sxs-lookup"><span data-stu-id="f2f70-153">userId</span></span>|<span data-ttu-id="f2f70-154">строка</span><span class="sxs-lookup"><span data-stu-id="f2f70-154">string</span></span>| <span data-ttu-id="f2f70-155">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="f2f70-155">The id of the user at risk</span></span>|
|<span data-ttu-id="f2f70-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2f70-156">userPrincipalName</span></span>|<span data-ttu-id="f2f70-157">string</span><span class="sxs-lookup"><span data-stu-id="f2f70-157">string</span></span>| <span data-ttu-id="f2f70-158">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="f2f70-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2f70-159">Связи</span><span class="sxs-lookup"><span data-stu-id="f2f70-159">Relationships</span></span>
| <span data-ttu-id="f2f70-160">Связь</span><span class="sxs-lookup"><span data-stu-id="f2f70-160">Relationship</span></span> | <span data-ttu-id="f2f70-161">Тип</span><span class="sxs-lookup"><span data-stu-id="f2f70-161">Type</span></span>   |<span data-ttu-id="f2f70-162">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f70-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2f70-163">импактедусер</span><span class="sxs-lookup"><span data-stu-id="f2f70-163">impactedUser</span></span>|[<span data-ttu-id="f2f70-164">user</span><span class="sxs-lookup"><span data-stu-id="f2f70-164">user</span></span>](user.md)| <span data-ttu-id="f2f70-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="f2f70-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2f70-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2f70-167">JSON representation</span></span>

<span data-ttu-id="f2f70-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2f70-168">Here is a JSON representation of the resource.</span></span>

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