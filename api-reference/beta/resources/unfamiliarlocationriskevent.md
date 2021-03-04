---
title: тип ресурса unfamiliarLocationRiskEvent
description: Событие риска, обнаруженное службой Azure Active Directory Identity Protection, в котором попытка войти в учетную запись будет предпринята из нового расположения для этого пользователя. Полные сведения о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: e2d34106de3e0b72303f103edcc6a798b5790b47
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442735"
---
# <a name="unfamiliarlocationriskevent-resource-type-deprecated"></a><span data-ttu-id="2b1a5-104">тип ресурса unfamiliarLocationRiskEvent (неподготовленный)</span><span class="sxs-lookup"><span data-stu-id="2b1a5-104">unfamiliarLocationRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="2b1a5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b1a5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="2b1a5-106">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="2b1a5-107">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="2b1a5-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="2b1a5-108">Событие риска, обнаруженное [службой Azure Active Directory Identity Protection,](/azure/active-directory/identity-protection/overview-identity-protection) в котором попытка войти в учетную запись будет предпринята из нового расположения для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="2b1a5-109">Полные сведения о событиях риска можно найти в документации [azure AD Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="2b1a5-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="2b1a5-110">Методы</span><span class="sxs-lookup"><span data-stu-id="2b1a5-110">Methods</span></span>

| <span data-ttu-id="2b1a5-111">Метод</span><span class="sxs-lookup"><span data-stu-id="2b1a5-111">Method</span></span>           | <span data-ttu-id="2b1a5-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2b1a5-112">Return Type</span></span>    |<span data-ttu-id="2b1a5-113">Описание</span><span class="sxs-lookup"><span data-stu-id="2b1a5-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b1a5-114">Получение объекта unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2b1a5-114">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="2b1a5-115">unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="2b1a5-115">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="2b1a5-116">Чтение свойств и связей незнакомого объектаLocationRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-116">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b1a5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="2b1a5-117">Properties</span></span>
| <span data-ttu-id="2b1a5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b1a5-118">Property</span></span>     | <span data-ttu-id="2b1a5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2b1a5-119">Type</span></span>   |<span data-ttu-id="2b1a5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2b1a5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b1a5-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b1a5-121">closedDateTime</span></span>|<span data-ttu-id="2b1a5-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b1a5-122">dateTimeOffset</span></span>| <span data-ttu-id="2b1a5-123">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="2b1a5-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="2b1a5-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b1a5-124">createdDateTime</span></span>|<span data-ttu-id="2b1a5-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b1a5-125">dateTimeOffset</span></span>| <span data-ttu-id="2b1a5-126">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="2b1a5-127">Это всегда больше или равно дате самого события риска.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="2b1a5-128">Это правильное свойство, используемее в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="2b1a5-129">id</span><span class="sxs-lookup"><span data-stu-id="2b1a5-129">id</span></span>|<span data-ttu-id="2b1a5-130">string</span><span class="sxs-lookup"><span data-stu-id="2b1a5-130">string</span></span>| <span data-ttu-id="2b1a5-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="2b1a5-131">Read-only</span></span>|
|<span data-ttu-id="2b1a5-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="2b1a5-132">ipAddress</span></span>|<span data-ttu-id="2b1a5-133">string</span><span class="sxs-lookup"><span data-stu-id="2b1a5-133">string</span></span>| <span data-ttu-id="2b1a5-134">IP-адрес входного</span><span class="sxs-lookup"><span data-stu-id="2b1a5-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="2b1a5-135">location</span><span class="sxs-lookup"><span data-stu-id="2b1a5-135">location</span></span>|<span data-ttu-id="2b1a5-136">string</span><span class="sxs-lookup"><span data-stu-id="2b1a5-136">string</span></span>| <span data-ttu-id="2b1a5-137">Расположение, прикрепленное к IP-адресу входного</span><span class="sxs-lookup"><span data-stu-id="2b1a5-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="2b1a5-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="2b1a5-138">riskEventDateTime</span></span>|<span data-ttu-id="2b1a5-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b1a5-139">dateTimeOffset</span></span>| <span data-ttu-id="2b1a5-140">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="2b1a5-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="2b1a5-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="2b1a5-141">riskEventStatus</span></span>|<span data-ttu-id="2b1a5-142">string</span><span class="sxs-lookup"><span data-stu-id="2b1a5-142">string</span></span>| <span data-ttu-id="2b1a5-143">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="2b1a5-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="2b1a5-144">riskLevel</span></span>|<span data-ttu-id="2b1a5-145">string</span><span class="sxs-lookup"><span data-stu-id="2b1a5-145">string</span></span>| <span data-ttu-id="2b1a5-146">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="2b1a5-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="2b1a5-147">riskEventType</span></span>|<span data-ttu-id="2b1a5-148">string</span><span class="sxs-lookup"><span data-stu-id="2b1a5-148">string</span></span>| <span data-ttu-id="2b1a5-149">Тип риска</span><span class="sxs-lookup"><span data-stu-id="2b1a5-149">The type of risk</span></span>|
|<span data-ttu-id="2b1a5-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2b1a5-150">userDisplayName</span></span>|<span data-ttu-id="2b1a5-151">string</span><span class="sxs-lookup"><span data-stu-id="2b1a5-151">string</span></span>| <span data-ttu-id="2b1a5-152">Имя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="2b1a5-152">The name of the user at risk</span></span>|
|<span data-ttu-id="2b1a5-153">userId</span><span class="sxs-lookup"><span data-stu-id="2b1a5-153">userId</span></span>|<span data-ttu-id="2b1a5-154">строка</span><span class="sxs-lookup"><span data-stu-id="2b1a5-154">string</span></span>| <span data-ttu-id="2b1a5-155">ID пользователя, на который существует риск</span><span class="sxs-lookup"><span data-stu-id="2b1a5-155">The id of the user at risk</span></span>|
|<span data-ttu-id="2b1a5-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2b1a5-156">userPrincipalName</span></span>|<span data-ttu-id="2b1a5-157">string</span><span class="sxs-lookup"><span data-stu-id="2b1a5-157">string</span></span>| <span data-ttu-id="2b1a5-158">Основное имя пользователя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="2b1a5-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b1a5-159">Связи</span><span class="sxs-lookup"><span data-stu-id="2b1a5-159">Relationships</span></span>
| <span data-ttu-id="2b1a5-160">Связь</span><span class="sxs-lookup"><span data-stu-id="2b1a5-160">Relationship</span></span> | <span data-ttu-id="2b1a5-161">Тип</span><span class="sxs-lookup"><span data-stu-id="2b1a5-161">Type</span></span>   |<span data-ttu-id="2b1a5-162">Описание</span><span class="sxs-lookup"><span data-stu-id="2b1a5-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b1a5-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="2b1a5-163">impactedUser</span></span>|[<span data-ttu-id="2b1a5-164">user</span><span class="sxs-lookup"><span data-stu-id="2b1a5-164">user</span></span>](user.md)| <span data-ttu-id="2b1a5-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b1a5-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2b1a5-167">JSON representation</span></span>

<span data-ttu-id="2b1a5-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b1a5-168">Here is a JSON representation of the resource.</span></span>

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
