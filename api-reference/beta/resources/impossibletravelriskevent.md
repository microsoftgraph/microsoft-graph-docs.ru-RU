---
title: тип ресурса impossibleTravelRiskEvent
description: Событие риска, обнаруженное службой Azure Active Directory Identity Protection, в котором две входные записи происходят из нетипичных для пользователя местоположений и невозможно будет ездить между расположениями в период между входами. Полные сведения о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: c62dfda856bf2761290fff93b505669348eded0e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440236"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a><span data-ttu-id="e78f8-103">невозможный тип ресурсовTravelRiskEvent (обесценен)</span><span class="sxs-lookup"><span data-stu-id="e78f8-103">impossibleTravelRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="e78f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e78f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="e78f8-105">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="e78f8-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="e78f8-106">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="e78f8-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="e78f8-107">Событие риска, обнаруженное [службой Azure Active Directory Identity Protection,](/azure/active-directory/identity-protection/overview-identity-protection) в котором две входные записи происходят из нетипичных для пользователя местоположений и невозможно будет ездить между расположениями в период между входами. Полные сведения о событиях риска можно найти в документации [azure AD Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="e78f8-107">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="e78f8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e78f8-108">Methods</span></span>

| <span data-ttu-id="e78f8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e78f8-109">Method</span></span>           | <span data-ttu-id="e78f8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e78f8-110">Return Type</span></span>    |<span data-ttu-id="e78f8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e78f8-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e78f8-112">Получение объекта impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e78f8-112">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="e78f8-113">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e78f8-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="e78f8-114">Чтение свойств и связей невозможного объектаTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="e78f8-114">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e78f8-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="e78f8-115">Properties</span></span>
| <span data-ttu-id="e78f8-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="e78f8-116">Property</span></span>     | <span data-ttu-id="e78f8-117">Тип</span><span class="sxs-lookup"><span data-stu-id="e78f8-117">Type</span></span>   |<span data-ttu-id="e78f8-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e78f8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e78f8-119">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="e78f8-119">closedDateTime</span></span>|<span data-ttu-id="e78f8-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78f8-120">dateTimeOffset</span></span>| <span data-ttu-id="e78f8-121">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="e78f8-121">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="e78f8-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e78f8-122">createdDateTime</span></span>|<span data-ttu-id="e78f8-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78f8-123">dateTimeOffset</span></span>| <span data-ttu-id="e78f8-124">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="e78f8-124">The date and time that the risk event was created.</span></span> <span data-ttu-id="e78f8-125">Это всегда больше или равно дате самого события риска.</span><span class="sxs-lookup"><span data-stu-id="e78f8-125">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="e78f8-126">Это правильное свойство, используемее в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="e78f8-126">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="e78f8-127">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="e78f8-127">deviceInformation</span></span>|<span data-ttu-id="e78f8-128">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-128">string</span></span>| <span data-ttu-id="e78f8-129">Сведения об устройстве</span><span class="sxs-lookup"><span data-stu-id="e78f8-129">Information about the device</span></span>|
|<span data-ttu-id="e78f8-130">id</span><span class="sxs-lookup"><span data-stu-id="e78f8-130">id</span></span>|<span data-ttu-id="e78f8-131">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-131">string</span></span>| <span data-ttu-id="e78f8-132">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="e78f8-132">Read-only</span></span>|
|<span data-ttu-id="e78f8-133">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e78f8-133">ipAddress</span></span>|<span data-ttu-id="e78f8-134">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-134">string</span></span>| <span data-ttu-id="e78f8-135">IP-адрес второго входного</span><span class="sxs-lookup"><span data-stu-id="e78f8-135">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="e78f8-136">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="e78f8-136">isAtypicalLocation</span></span>|<span data-ttu-id="e78f8-137">boolean</span><span class="sxs-lookup"><span data-stu-id="e78f8-137">boolean</span></span>| <span data-ttu-id="e78f8-138">Если одно из местоположений нетипично для пользователя</span><span class="sxs-lookup"><span data-stu-id="e78f8-138">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="e78f8-139">location</span><span class="sxs-lookup"><span data-stu-id="e78f8-139">location</span></span>|<span data-ttu-id="e78f8-140">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-140">string</span></span>| <span data-ttu-id="e78f8-141">Расположение, присоединенное к IP-адресу второго входного</span><span class="sxs-lookup"><span data-stu-id="e78f8-141">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="e78f8-142">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="e78f8-142">previousIPAddress</span></span>|<span data-ttu-id="e78f8-143">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-143">string</span></span>| <span data-ttu-id="e78f8-144">IP-адрес первого входного</span><span class="sxs-lookup"><span data-stu-id="e78f8-144">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="e78f8-145">previousLocation</span><span class="sxs-lookup"><span data-stu-id="e78f8-145">previousLocation</span></span>|<span data-ttu-id="e78f8-146">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-146">string</span></span>| <span data-ttu-id="e78f8-147">Расположение, присоединенное к IP-адресу первого входного</span><span class="sxs-lookup"><span data-stu-id="e78f8-147">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="e78f8-148">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="e78f8-148">previousSigninDateTime</span></span>|<span data-ttu-id="e78f8-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78f8-149">dateTimeOffset</span></span>| <span data-ttu-id="e78f8-150">Дата и время первого входного</span><span class="sxs-lookup"><span data-stu-id="e78f8-150">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="e78f8-151">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="e78f8-151">riskEventDateTime</span></span>|<span data-ttu-id="e78f8-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78f8-152">dateTimeOffset</span></span>| <span data-ttu-id="e78f8-153">Дата и время второго входного</span><span class="sxs-lookup"><span data-stu-id="e78f8-153">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="e78f8-154">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="e78f8-154">riskEventStatus</span></span>|<span data-ttu-id="e78f8-155">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-155">string</span></span>| <span data-ttu-id="e78f8-156">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="e78f8-156">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="e78f8-157">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e78f8-157">riskLevel</span></span>|<span data-ttu-id="e78f8-158">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-158">string</span></span>| <span data-ttu-id="e78f8-159">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e78f8-159">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e78f8-160">riskEventType</span><span class="sxs-lookup"><span data-stu-id="e78f8-160">riskEventType</span></span>|<span data-ttu-id="e78f8-161">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-161">string</span></span>| <span data-ttu-id="e78f8-162">Тип риска</span><span class="sxs-lookup"><span data-stu-id="e78f8-162">The type of risk</span></span>|
|<span data-ttu-id="e78f8-163">userAgent</span><span class="sxs-lookup"><span data-stu-id="e78f8-163">userAgent</span></span>|<span data-ttu-id="e78f8-164">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-164">string</span></span>| <span data-ttu-id="e78f8-165">Строка агента пользователя браузера</span><span class="sxs-lookup"><span data-stu-id="e78f8-165">The browser's user agent string</span></span>|
|<span data-ttu-id="e78f8-166">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e78f8-166">userDisplayName</span></span>|<span data-ttu-id="e78f8-167">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-167">string</span></span>| <span data-ttu-id="e78f8-168">Имя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="e78f8-168">The name of the user at risk</span></span>|
|<span data-ttu-id="e78f8-169">userId</span><span class="sxs-lookup"><span data-stu-id="e78f8-169">userId</span></span>|<span data-ttu-id="e78f8-170">строка</span><span class="sxs-lookup"><span data-stu-id="e78f8-170">string</span></span>| <span data-ttu-id="e78f8-171">ID пользователя, на который существует риск</span><span class="sxs-lookup"><span data-stu-id="e78f8-171">The id of the user at risk</span></span>|
|<span data-ttu-id="e78f8-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e78f8-172">userPrincipalName</span></span>|<span data-ttu-id="e78f8-173">string</span><span class="sxs-lookup"><span data-stu-id="e78f8-173">string</span></span>| <span data-ttu-id="e78f8-174">Основное имя пользователя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="e78f8-174">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="e78f8-175">Связи</span><span class="sxs-lookup"><span data-stu-id="e78f8-175">Relationships</span></span>
| <span data-ttu-id="e78f8-176">Связь</span><span class="sxs-lookup"><span data-stu-id="e78f8-176">Relationship</span></span> | <span data-ttu-id="e78f8-177">Тип</span><span class="sxs-lookup"><span data-stu-id="e78f8-177">Type</span></span>   |<span data-ttu-id="e78f8-178">Описание</span><span class="sxs-lookup"><span data-stu-id="e78f8-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e78f8-179">impactedUser</span><span class="sxs-lookup"><span data-stu-id="e78f8-179">impactedUser</span></span>|[<span data-ttu-id="e78f8-180">user</span><span class="sxs-lookup"><span data-stu-id="e78f8-180">user</span></span>](user.md)| <span data-ttu-id="e78f8-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e78f8-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e78f8-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e78f8-183">JSON representation</span></span>

<span data-ttu-id="e78f8-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e78f8-184">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
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
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
