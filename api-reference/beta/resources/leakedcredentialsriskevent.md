---
title: Тип ресурса Леакедкредентиалсрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором были обнаружены учетные данные учетной записи в подстановке. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4f12131d1dafcd8bc33d026ef4c56d220eae2799
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870217"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="db3c0-104">Тип ресурса Леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="db3c0-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="db3c0-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="db3c0-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="db3c0-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="db3c0-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="db3c0-107">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) , в котором были обнаружены учетные данные учетной записи в подстановке.</span><span class="sxs-lookup"><span data-stu-id="db3c0-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="db3c0-108">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="db3c0-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="db3c0-109">Методы</span><span class="sxs-lookup"><span data-stu-id="db3c0-109">Methods</span></span>

| <span data-ttu-id="db3c0-110">Метод</span><span class="sxs-lookup"><span data-stu-id="db3c0-110">Method</span></span>           | <span data-ttu-id="db3c0-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="db3c0-111">Return Type</span></span>    |<span data-ttu-id="db3c0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="db3c0-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db3c0-113">Получение объекта leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="db3c0-113">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="db3c0-114">леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="db3c0-114">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="db3c0-115">Чтение свойств и связей объекта Леакедкредентиалсрискевент.</span><span class="sxs-lookup"><span data-stu-id="db3c0-115">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="db3c0-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="db3c0-116">Properties</span></span>
| <span data-ttu-id="db3c0-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="db3c0-117">Property</span></span>     | <span data-ttu-id="db3c0-118">Тип</span><span class="sxs-lookup"><span data-stu-id="db3c0-118">Type</span></span>   |<span data-ttu-id="db3c0-119">Описание</span><span class="sxs-lookup"><span data-stu-id="db3c0-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db3c0-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="db3c0-120">closedDateTime</span></span>|<span data-ttu-id="db3c0-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db3c0-121">dateTimeOffset</span></span>| <span data-ttu-id="db3c0-122">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="db3c0-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="db3c0-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db3c0-123">createdDateTime</span></span>|<span data-ttu-id="db3c0-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db3c0-124">dateTimeOffset</span></span>| <span data-ttu-id="db3c0-125">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="db3c0-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="db3c0-126">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="db3c0-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="db3c0-127">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="db3c0-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="db3c0-128">id</span><span class="sxs-lookup"><span data-stu-id="db3c0-128">id</span></span>|<span data-ttu-id="db3c0-129">string</span><span class="sxs-lookup"><span data-stu-id="db3c0-129">string</span></span>| <span data-ttu-id="db3c0-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="db3c0-130">Read-only</span></span>|
|<span data-ttu-id="db3c0-131">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="db3c0-131">riskEventDateTime</span></span>|<span data-ttu-id="db3c0-132">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db3c0-132">dateTimeOffset</span></span>| <span data-ttu-id="db3c0-133">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="db3c0-133">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="db3c0-134">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="db3c0-134">riskEventStatus</span></span>|<span data-ttu-id="db3c0-135">string</span><span class="sxs-lookup"><span data-stu-id="db3c0-135">string</span></span>| <span data-ttu-id="db3c0-136">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="db3c0-136">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="db3c0-137">riskLevel</span><span class="sxs-lookup"><span data-stu-id="db3c0-137">riskLevel</span></span>|<span data-ttu-id="db3c0-138">string</span><span class="sxs-lookup"><span data-stu-id="db3c0-138">string</span></span>| <span data-ttu-id="db3c0-139">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="db3c0-139">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="db3c0-140">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="db3c0-140">riskEventType</span></span>|<span data-ttu-id="db3c0-141">string</span><span class="sxs-lookup"><span data-stu-id="db3c0-141">string</span></span>| <span data-ttu-id="db3c0-142">Тип риска</span><span class="sxs-lookup"><span data-stu-id="db3c0-142">The type of risk</span></span>|
|<span data-ttu-id="db3c0-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="db3c0-143">userDisplayName</span></span>|<span data-ttu-id="db3c0-144">string</span><span class="sxs-lookup"><span data-stu-id="db3c0-144">string</span></span>| <span data-ttu-id="db3c0-145">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="db3c0-145">The name of the user at risk</span></span>|
|<span data-ttu-id="db3c0-146">userId</span><span class="sxs-lookup"><span data-stu-id="db3c0-146">userId</span></span>|<span data-ttu-id="db3c0-147">строка</span><span class="sxs-lookup"><span data-stu-id="db3c0-147">string</span></span>| <span data-ttu-id="db3c0-148">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="db3c0-148">The id of the user at risk</span></span>|
|<span data-ttu-id="db3c0-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="db3c0-149">userPrincipalName</span></span>|<span data-ttu-id="db3c0-150">string</span><span class="sxs-lookup"><span data-stu-id="db3c0-150">string</span></span>| <span data-ttu-id="db3c0-151">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="db3c0-151">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="db3c0-152">Отношения</span><span class="sxs-lookup"><span data-stu-id="db3c0-152">Relationships</span></span>
| <span data-ttu-id="db3c0-153">Связь</span><span class="sxs-lookup"><span data-stu-id="db3c0-153">Relationship</span></span> | <span data-ttu-id="db3c0-154">Тип</span><span class="sxs-lookup"><span data-stu-id="db3c0-154">Type</span></span>   |<span data-ttu-id="db3c0-155">Описание</span><span class="sxs-lookup"><span data-stu-id="db3c0-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db3c0-156">импактедусер</span><span class="sxs-lookup"><span data-stu-id="db3c0-156">impactedUser</span></span>|[<span data-ttu-id="db3c0-157">user</span><span class="sxs-lookup"><span data-stu-id="db3c0-157">user</span></span>](user.md)| <span data-ttu-id="db3c0-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="db3c0-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db3c0-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db3c0-160">JSON representation</span></span>

<span data-ttu-id="db3c0-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db3c0-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
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
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
