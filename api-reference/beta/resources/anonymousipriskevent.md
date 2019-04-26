---
title: Тип ресурса Анонимаусиприскевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором выполняется попытка входа учетной записи с IP-адреса, который является анонимным. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
ms.openlocfilehash: 8fa1210a8899af11e295e6503dfcae51dba43776
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339169"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="e770f-104">Тип ресурса Анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="e770f-104">anonymousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e770f-105">Событие риска, обнаруженное службой [удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , в котором выполняется попытка входа учетной записи с IP-адреса, который является анонимным.</span><span class="sxs-lookup"><span data-stu-id="e770f-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="e770f-106">Полную информацию о событиях риска можно найти в [документации по защите удостоверенИй Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="e770f-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="e770f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e770f-107">Methods</span></span>

| <span data-ttu-id="e770f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e770f-108">Method</span></span>           | <span data-ttu-id="e770f-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e770f-109">Return Type</span></span>    |<span data-ttu-id="e770f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e770f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e770f-111">Получение объекта anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e770f-111">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="e770f-112">Анонимаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="e770f-112">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="e770f-113">Чтение свойств и связей объекта Анонимаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="e770f-113">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e770f-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="e770f-114">Properties</span></span>
| <span data-ttu-id="e770f-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="e770f-115">Property</span></span>     | <span data-ttu-id="e770f-116">Тип</span><span class="sxs-lookup"><span data-stu-id="e770f-116">Type</span></span>   |<span data-ttu-id="e770f-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e770f-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e770f-118">Клоседдатетиме</span><span class="sxs-lookup"><span data-stu-id="e770f-118">closedDateTime</span></span>|<span data-ttu-id="e770f-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e770f-119">dateTimeOffset</span></span>| <span data-ttu-id="e770f-120">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="e770f-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="e770f-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e770f-121">createdDateTime</span></span>|<span data-ttu-id="e770f-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e770f-122">dateTimeOffset</span></span>| <span data-ttu-id="e770f-123">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="e770f-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="e770f-124">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="e770f-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="e770f-125">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="e770f-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="e770f-126">id</span><span class="sxs-lookup"><span data-stu-id="e770f-126">id</span></span>|<span data-ttu-id="e770f-127">строка</span><span class="sxs-lookup"><span data-stu-id="e770f-127">string</span></span>| <span data-ttu-id="e770f-128">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="e770f-128">Read-only</span></span>|
|<span data-ttu-id="e770f-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e770f-129">ipAddress</span></span>|<span data-ttu-id="e770f-130">string</span><span class="sxs-lookup"><span data-stu-id="e770f-130">string</span></span>| <span data-ttu-id="e770f-131">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="e770f-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="e770f-132">location</span><span class="sxs-lookup"><span data-stu-id="e770f-132">location</span></span>|<span data-ttu-id="e770f-133">string</span><span class="sxs-lookup"><span data-stu-id="e770f-133">string</span></span>| <span data-ttu-id="e770f-134">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="e770f-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="e770f-135">Рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="e770f-135">riskEventDateTime</span></span>|<span data-ttu-id="e770f-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e770f-136">dateTimeOffset</span></span>| <span data-ttu-id="e770f-137">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="e770f-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="e770f-138">Рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="e770f-138">riskEventStatus</span></span>|<span data-ttu-id="e770f-139">string</span><span class="sxs-lookup"><span data-stu-id="e770f-139">string</span></span>| <span data-ttu-id="e770f-140">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="e770f-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="e770f-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e770f-141">riskLevel</span></span>|<span data-ttu-id="e770f-142">string</span><span class="sxs-lookup"><span data-stu-id="e770f-142">string</span></span>| <span data-ttu-id="e770f-143">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e770f-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e770f-144">Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="e770f-144">riskEventType</span></span>|<span data-ttu-id="e770f-145">string</span><span class="sxs-lookup"><span data-stu-id="e770f-145">string</span></span>| <span data-ttu-id="e770f-146">Тип риска</span><span class="sxs-lookup"><span data-stu-id="e770f-146">The type of risk</span></span>|
|<span data-ttu-id="e770f-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e770f-147">userDisplayName</span></span>|<span data-ttu-id="e770f-148">string</span><span class="sxs-lookup"><span data-stu-id="e770f-148">string</span></span>| <span data-ttu-id="e770f-149">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="e770f-149">The name of the user at risk</span></span>|
|<span data-ttu-id="e770f-150">userId</span><span class="sxs-lookup"><span data-stu-id="e770f-150">userId</span></span>|<span data-ttu-id="e770f-151">string</span><span class="sxs-lookup"><span data-stu-id="e770f-151">string</span></span>| <span data-ttu-id="e770f-152">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="e770f-152">The id of the user at risk</span></span>|
|<span data-ttu-id="e770f-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e770f-153">userPrincipalName</span></span>|<span data-ttu-id="e770f-154">string</span><span class="sxs-lookup"><span data-stu-id="e770f-154">string</span></span>| <span data-ttu-id="e770f-155">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="e770f-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="e770f-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="e770f-156">Relationships</span></span>
| <span data-ttu-id="e770f-157">Отношение</span><span class="sxs-lookup"><span data-stu-id="e770f-157">Relationship</span></span> | <span data-ttu-id="e770f-158">Тип</span><span class="sxs-lookup"><span data-stu-id="e770f-158">Type</span></span>   |<span data-ttu-id="e770f-159">Описание</span><span class="sxs-lookup"><span data-stu-id="e770f-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e770f-160">Импактедусер</span><span class="sxs-lookup"><span data-stu-id="e770f-160">impactedUser</span></span>|[<span data-ttu-id="e770f-161">user</span><span class="sxs-lookup"><span data-stu-id="e770f-161">user</span></span>](user.md)| <span data-ttu-id="e770f-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e770f-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e770f-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e770f-164">JSON representation</span></span>

<span data-ttu-id="e770f-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e770f-165">Here is a JSON representation of the resource.</span></span>

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
