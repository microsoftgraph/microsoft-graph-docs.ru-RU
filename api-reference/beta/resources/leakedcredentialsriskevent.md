---
title: тип ресурса leakedCredentialsRiskEvent
description: Событие риска, обнаруженное службой Azure Active Directory Identity Protection, в котором учетные данные учетной записи были обнаружены в дикой природе. Полные сведения о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: ac8e9dc0c2adb685513c74658464f4a79af5cb45
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442985"
---
# <a name="leakedcredentialsriskevent-resource-type-deprecated"></a><span data-ttu-id="11878-104">leakedCredentialsRiskEvent resource type (deprecated)</span><span class="sxs-lookup"><span data-stu-id="11878-104">leakedCredentialsRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="11878-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11878-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="11878-106">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="11878-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="11878-107">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="11878-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="11878-108">Событие риска, обнаруженное [службой Azure Active Directory Identity Protection,](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) в котором учетные данные учетной записи были обнаружены в дикой природе.</span><span class="sxs-lookup"><span data-stu-id="11878-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="11878-109">Полные сведения о событиях риска можно найти в документации [azure AD Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="11878-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="11878-110">Методы</span><span class="sxs-lookup"><span data-stu-id="11878-110">Methods</span></span>

| <span data-ttu-id="11878-111">Метод</span><span class="sxs-lookup"><span data-stu-id="11878-111">Method</span></span>           | <span data-ttu-id="11878-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11878-112">Return Type</span></span>    |<span data-ttu-id="11878-113">Описание</span><span class="sxs-lookup"><span data-stu-id="11878-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11878-114">Получение объекта leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11878-114">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="11878-115">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="11878-115">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="11878-116">Чтение свойств и связей объекта leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="11878-116">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11878-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="11878-117">Properties</span></span>
| <span data-ttu-id="11878-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="11878-118">Property</span></span>     | <span data-ttu-id="11878-119">Тип</span><span class="sxs-lookup"><span data-stu-id="11878-119">Type</span></span>   |<span data-ttu-id="11878-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11878-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11878-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="11878-121">closedDateTime</span></span>|<span data-ttu-id="11878-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11878-122">dateTimeOffset</span></span>| <span data-ttu-id="11878-123">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="11878-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="11878-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11878-124">createdDateTime</span></span>|<span data-ttu-id="11878-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11878-125">dateTimeOffset</span></span>| <span data-ttu-id="11878-126">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="11878-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="11878-127">Это всегда больше или равно дате самого события риска.</span><span class="sxs-lookup"><span data-stu-id="11878-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="11878-128">Это правильное свойство, используемее в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="11878-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="11878-129">id</span><span class="sxs-lookup"><span data-stu-id="11878-129">id</span></span>|<span data-ttu-id="11878-130">string</span><span class="sxs-lookup"><span data-stu-id="11878-130">string</span></span>| <span data-ttu-id="11878-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="11878-131">Read-only</span></span>|
|<span data-ttu-id="11878-132">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="11878-132">riskEventDateTime</span></span>|<span data-ttu-id="11878-133">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11878-133">dateTimeOffset</span></span>| <span data-ttu-id="11878-134">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="11878-134">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="11878-135">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="11878-135">riskEventStatus</span></span>|<span data-ttu-id="11878-136">string</span><span class="sxs-lookup"><span data-stu-id="11878-136">string</span></span>| <span data-ttu-id="11878-137">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="11878-137">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="11878-138">riskLevel</span><span class="sxs-lookup"><span data-stu-id="11878-138">riskLevel</span></span>|<span data-ttu-id="11878-139">string</span><span class="sxs-lookup"><span data-stu-id="11878-139">string</span></span>| <span data-ttu-id="11878-140">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="11878-140">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="11878-141">riskEventType</span><span class="sxs-lookup"><span data-stu-id="11878-141">riskEventType</span></span>|<span data-ttu-id="11878-142">string</span><span class="sxs-lookup"><span data-stu-id="11878-142">string</span></span>| <span data-ttu-id="11878-143">Тип риска</span><span class="sxs-lookup"><span data-stu-id="11878-143">The type of risk</span></span>|
|<span data-ttu-id="11878-144">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="11878-144">userDisplayName</span></span>|<span data-ttu-id="11878-145">string</span><span class="sxs-lookup"><span data-stu-id="11878-145">string</span></span>| <span data-ttu-id="11878-146">Имя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="11878-146">The name of the user at risk</span></span>|
|<span data-ttu-id="11878-147">userId</span><span class="sxs-lookup"><span data-stu-id="11878-147">userId</span></span>|<span data-ttu-id="11878-148">строка</span><span class="sxs-lookup"><span data-stu-id="11878-148">string</span></span>| <span data-ttu-id="11878-149">ID пользователя, на который существует риск</span><span class="sxs-lookup"><span data-stu-id="11878-149">The id of the user at risk</span></span>|
|<span data-ttu-id="11878-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="11878-150">userPrincipalName</span></span>|<span data-ttu-id="11878-151">string</span><span class="sxs-lookup"><span data-stu-id="11878-151">string</span></span>| <span data-ttu-id="11878-152">Основное имя пользователя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="11878-152">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="11878-153">Связи</span><span class="sxs-lookup"><span data-stu-id="11878-153">Relationships</span></span>
| <span data-ttu-id="11878-154">Связь</span><span class="sxs-lookup"><span data-stu-id="11878-154">Relationship</span></span> | <span data-ttu-id="11878-155">Тип</span><span class="sxs-lookup"><span data-stu-id="11878-155">Type</span></span>   |<span data-ttu-id="11878-156">Описание</span><span class="sxs-lookup"><span data-stu-id="11878-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11878-157">impactedUser</span><span class="sxs-lookup"><span data-stu-id="11878-157">impactedUser</span></span>|[<span data-ttu-id="11878-158">user</span><span class="sxs-lookup"><span data-stu-id="11878-158">user</span></span>](user.md)| <span data-ttu-id="11878-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="11878-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11878-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11878-161">JSON representation</span></span>

<span data-ttu-id="11878-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11878-162">Here is a JSON representation of the resource.</span></span>

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
