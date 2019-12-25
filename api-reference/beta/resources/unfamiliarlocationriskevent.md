---
title: Тип ресурса Унфамилиарлокатионрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором выполняется попытка входа учетной записи из нового расположения для этого пользователя. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 72a114fb42d24bd61aef3bff5cd3fba8d2de93a0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866513"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="36490-104">Тип ресурса Унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="36490-104">unfamiliarLocationRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="36490-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="36490-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="36490-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="36490-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="36490-107">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) , в котором выполняется попытка входа учетной записи из нового расположения для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="36490-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="36490-108">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="36490-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="36490-109">Методы</span><span class="sxs-lookup"><span data-stu-id="36490-109">Methods</span></span>

| <span data-ttu-id="36490-110">Метод</span><span class="sxs-lookup"><span data-stu-id="36490-110">Method</span></span>           | <span data-ttu-id="36490-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="36490-111">Return Type</span></span>    |<span data-ttu-id="36490-112">Описание</span><span class="sxs-lookup"><span data-stu-id="36490-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36490-113">Получение объекта unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="36490-113">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="36490-114">унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="36490-114">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="36490-115">Чтение свойств и связей объекта Унфамилиарлокатионрискевент.</span><span class="sxs-lookup"><span data-stu-id="36490-115">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="36490-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="36490-116">Properties</span></span>
| <span data-ttu-id="36490-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="36490-117">Property</span></span>     | <span data-ttu-id="36490-118">Тип</span><span class="sxs-lookup"><span data-stu-id="36490-118">Type</span></span>   |<span data-ttu-id="36490-119">Описание</span><span class="sxs-lookup"><span data-stu-id="36490-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36490-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="36490-120">closedDateTime</span></span>|<span data-ttu-id="36490-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36490-121">dateTimeOffset</span></span>| <span data-ttu-id="36490-122">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="36490-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="36490-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36490-123">createdDateTime</span></span>|<span data-ttu-id="36490-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36490-124">dateTimeOffset</span></span>| <span data-ttu-id="36490-125">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="36490-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="36490-126">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="36490-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="36490-127">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="36490-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="36490-128">id</span><span class="sxs-lookup"><span data-stu-id="36490-128">id</span></span>|<span data-ttu-id="36490-129">string</span><span class="sxs-lookup"><span data-stu-id="36490-129">string</span></span>| <span data-ttu-id="36490-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="36490-130">Read-only</span></span>|
|<span data-ttu-id="36490-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="36490-131">ipAddress</span></span>|<span data-ttu-id="36490-132">string</span><span class="sxs-lookup"><span data-stu-id="36490-132">string</span></span>| <span data-ttu-id="36490-133">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="36490-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="36490-134">location</span><span class="sxs-lookup"><span data-stu-id="36490-134">location</span></span>|<span data-ttu-id="36490-135">string</span><span class="sxs-lookup"><span data-stu-id="36490-135">string</span></span>| <span data-ttu-id="36490-136">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="36490-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="36490-137">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="36490-137">riskEventDateTime</span></span>|<span data-ttu-id="36490-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36490-138">dateTimeOffset</span></span>| <span data-ttu-id="36490-139">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="36490-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="36490-140">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="36490-140">riskEventStatus</span></span>|<span data-ttu-id="36490-141">string</span><span class="sxs-lookup"><span data-stu-id="36490-141">string</span></span>| <span data-ttu-id="36490-142">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="36490-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="36490-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="36490-143">riskLevel</span></span>|<span data-ttu-id="36490-144">string</span><span class="sxs-lookup"><span data-stu-id="36490-144">string</span></span>| <span data-ttu-id="36490-145">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="36490-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="36490-146">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="36490-146">riskEventType</span></span>|<span data-ttu-id="36490-147">string</span><span class="sxs-lookup"><span data-stu-id="36490-147">string</span></span>| <span data-ttu-id="36490-148">Тип риска</span><span class="sxs-lookup"><span data-stu-id="36490-148">The type of risk</span></span>|
|<span data-ttu-id="36490-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="36490-149">userDisplayName</span></span>|<span data-ttu-id="36490-150">string</span><span class="sxs-lookup"><span data-stu-id="36490-150">string</span></span>| <span data-ttu-id="36490-151">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="36490-151">The name of the user at risk</span></span>|
|<span data-ttu-id="36490-152">userId</span><span class="sxs-lookup"><span data-stu-id="36490-152">userId</span></span>|<span data-ttu-id="36490-153">строка</span><span class="sxs-lookup"><span data-stu-id="36490-153">string</span></span>| <span data-ttu-id="36490-154">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="36490-154">The id of the user at risk</span></span>|
|<span data-ttu-id="36490-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="36490-155">userPrincipalName</span></span>|<span data-ttu-id="36490-156">string</span><span class="sxs-lookup"><span data-stu-id="36490-156">string</span></span>| <span data-ttu-id="36490-157">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="36490-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="36490-158">Отношения</span><span class="sxs-lookup"><span data-stu-id="36490-158">Relationships</span></span>
| <span data-ttu-id="36490-159">Связь</span><span class="sxs-lookup"><span data-stu-id="36490-159">Relationship</span></span> | <span data-ttu-id="36490-160">Тип</span><span class="sxs-lookup"><span data-stu-id="36490-160">Type</span></span>   |<span data-ttu-id="36490-161">Описание</span><span class="sxs-lookup"><span data-stu-id="36490-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36490-162">импактедусер</span><span class="sxs-lookup"><span data-stu-id="36490-162">impactedUser</span></span>|[<span data-ttu-id="36490-163">user</span><span class="sxs-lookup"><span data-stu-id="36490-163">user</span></span>](user.md)| <span data-ttu-id="36490-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="36490-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36490-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36490-166">JSON representation</span></span>

<span data-ttu-id="36490-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36490-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
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
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
