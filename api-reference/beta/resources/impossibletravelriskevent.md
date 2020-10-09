---
title: Тип ресурса Импоссиблетравелрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором два входа учетной записи происходят из расположений нетипично для пользователя, и вы не сможете перемещаться между расположениями в период между входными данными. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 72492c3542733c194ee4d5560b473cb7a67387c7
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404191"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a><span data-ttu-id="d8316-103">Тип ресурса Импоссиблетравелрискевент (не рекомендуется)</span><span class="sxs-lookup"><span data-stu-id="d8316-103">impossibleTravelRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="d8316-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8316-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="d8316-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="d8316-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="d8316-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="d8316-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="d8316-107">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) , в котором два входа учетной записи происходят из расположений нетипично для пользователя, и вы не сможете перемещаться между расположениями в период между входными данными. Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="d8316-107">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="d8316-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d8316-108">Methods</span></span>

| <span data-ttu-id="d8316-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d8316-109">Method</span></span>           | <span data-ttu-id="d8316-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d8316-110">Return Type</span></span>    |<span data-ttu-id="d8316-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8316-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8316-112">Получение объекта impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="d8316-112">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="d8316-113">импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="d8316-113">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="d8316-114">Чтение свойств и связей объекта Импоссиблетравелрискевент.</span><span class="sxs-lookup"><span data-stu-id="d8316-114">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8316-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8316-115">Properties</span></span>
| <span data-ttu-id="d8316-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8316-116">Property</span></span>     | <span data-ttu-id="d8316-117">Тип</span><span class="sxs-lookup"><span data-stu-id="d8316-117">Type</span></span>   |<span data-ttu-id="d8316-118">Описание</span><span class="sxs-lookup"><span data-stu-id="d8316-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8316-119">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8316-119">closedDateTime</span></span>|<span data-ttu-id="d8316-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8316-120">dateTimeOffset</span></span>| <span data-ttu-id="d8316-121">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="d8316-121">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="d8316-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8316-122">createdDateTime</span></span>|<span data-ttu-id="d8316-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8316-123">dateTimeOffset</span></span>| <span data-ttu-id="d8316-124">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="d8316-124">The date and time that the risk event was created.</span></span> <span data-ttu-id="d8316-125">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="d8316-125">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="d8316-126">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="d8316-126">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="d8316-127">девицеинформатион</span><span class="sxs-lookup"><span data-stu-id="d8316-127">deviceInformation</span></span>|<span data-ttu-id="d8316-128">string</span><span class="sxs-lookup"><span data-stu-id="d8316-128">string</span></span>| <span data-ttu-id="d8316-129">Сведения об устройстве</span><span class="sxs-lookup"><span data-stu-id="d8316-129">Information about the device</span></span>|
|<span data-ttu-id="d8316-130">id</span><span class="sxs-lookup"><span data-stu-id="d8316-130">id</span></span>|<span data-ttu-id="d8316-131">string</span><span class="sxs-lookup"><span data-stu-id="d8316-131">string</span></span>| <span data-ttu-id="d8316-132">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="d8316-132">Read-only</span></span>|
|<span data-ttu-id="d8316-133">ipAddress</span><span class="sxs-lookup"><span data-stu-id="d8316-133">ipAddress</span></span>|<span data-ttu-id="d8316-134">string</span><span class="sxs-lookup"><span data-stu-id="d8316-134">string</span></span>| <span data-ttu-id="d8316-135">IP-адрес второго входа</span><span class="sxs-lookup"><span data-stu-id="d8316-135">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="d8316-136">исатипикаллокатион</span><span class="sxs-lookup"><span data-stu-id="d8316-136">isAtypicalLocation</span></span>|<span data-ttu-id="d8316-137">boolean</span><span class="sxs-lookup"><span data-stu-id="d8316-137">boolean</span></span>| <span data-ttu-id="d8316-138">Если одно из расположений для пользователя является нетипичным</span><span class="sxs-lookup"><span data-stu-id="d8316-138">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="d8316-139">location</span><span class="sxs-lookup"><span data-stu-id="d8316-139">location</span></span>|<span data-ttu-id="d8316-140">string</span><span class="sxs-lookup"><span data-stu-id="d8316-140">string</span></span>| <span data-ttu-id="d8316-141">Расположение, подключенное к IP-адресу второго входа</span><span class="sxs-lookup"><span data-stu-id="d8316-141">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="d8316-142">превиаусипаддресс</span><span class="sxs-lookup"><span data-stu-id="d8316-142">previousIPAddress</span></span>|<span data-ttu-id="d8316-143">string</span><span class="sxs-lookup"><span data-stu-id="d8316-143">string</span></span>| <span data-ttu-id="d8316-144">IP-адрес первого входа</span><span class="sxs-lookup"><span data-stu-id="d8316-144">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="d8316-145">превиауслокатион</span><span class="sxs-lookup"><span data-stu-id="d8316-145">previousLocation</span></span>|<span data-ttu-id="d8316-146">string</span><span class="sxs-lookup"><span data-stu-id="d8316-146">string</span></span>| <span data-ttu-id="d8316-147">Расположение, подключенное к IP-адресу первого входа</span><span class="sxs-lookup"><span data-stu-id="d8316-147">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="d8316-148">превиауссигниндатетиме</span><span class="sxs-lookup"><span data-stu-id="d8316-148">previousSigninDateTime</span></span>|<span data-ttu-id="d8316-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8316-149">dateTimeOffset</span></span>| <span data-ttu-id="d8316-150">Дата и время первого входа</span><span class="sxs-lookup"><span data-stu-id="d8316-150">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="d8316-151">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="d8316-151">riskEventDateTime</span></span>|<span data-ttu-id="d8316-152">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8316-152">dateTimeOffset</span></span>| <span data-ttu-id="d8316-153">Дата и время второго входа</span><span class="sxs-lookup"><span data-stu-id="d8316-153">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="d8316-154">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="d8316-154">riskEventStatus</span></span>|<span data-ttu-id="d8316-155">string</span><span class="sxs-lookup"><span data-stu-id="d8316-155">string</span></span>| <span data-ttu-id="d8316-156">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="d8316-156">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="d8316-157">riskLevel</span><span class="sxs-lookup"><span data-stu-id="d8316-157">riskLevel</span></span>|<span data-ttu-id="d8316-158">string</span><span class="sxs-lookup"><span data-stu-id="d8316-158">string</span></span>| <span data-ttu-id="d8316-159">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d8316-159">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="d8316-160">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="d8316-160">riskEventType</span></span>|<span data-ttu-id="d8316-161">string</span><span class="sxs-lookup"><span data-stu-id="d8316-161">string</span></span>| <span data-ttu-id="d8316-162">Тип риска</span><span class="sxs-lookup"><span data-stu-id="d8316-162">The type of risk</span></span>|
|<span data-ttu-id="d8316-163">userAgent</span><span class="sxs-lookup"><span data-stu-id="d8316-163">userAgent</span></span>|<span data-ttu-id="d8316-164">string</span><span class="sxs-lookup"><span data-stu-id="d8316-164">string</span></span>| <span data-ttu-id="d8316-165">Строка агента пользователя браузера</span><span class="sxs-lookup"><span data-stu-id="d8316-165">The browser's user agent string</span></span>|
|<span data-ttu-id="d8316-166">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="d8316-166">userDisplayName</span></span>|<span data-ttu-id="d8316-167">string</span><span class="sxs-lookup"><span data-stu-id="d8316-167">string</span></span>| <span data-ttu-id="d8316-168">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="d8316-168">The name of the user at risk</span></span>|
|<span data-ttu-id="d8316-169">userId</span><span class="sxs-lookup"><span data-stu-id="d8316-169">userId</span></span>|<span data-ttu-id="d8316-170">строка</span><span class="sxs-lookup"><span data-stu-id="d8316-170">string</span></span>| <span data-ttu-id="d8316-171">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="d8316-171">The id of the user at risk</span></span>|
|<span data-ttu-id="d8316-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d8316-172">userPrincipalName</span></span>|<span data-ttu-id="d8316-173">string</span><span class="sxs-lookup"><span data-stu-id="d8316-173">string</span></span>| <span data-ttu-id="d8316-174">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="d8316-174">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8316-175">Связи</span><span class="sxs-lookup"><span data-stu-id="d8316-175">Relationships</span></span>
| <span data-ttu-id="d8316-176">Связь</span><span class="sxs-lookup"><span data-stu-id="d8316-176">Relationship</span></span> | <span data-ttu-id="d8316-177">Тип</span><span class="sxs-lookup"><span data-stu-id="d8316-177">Type</span></span>   |<span data-ttu-id="d8316-178">Описание</span><span class="sxs-lookup"><span data-stu-id="d8316-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8316-179">импактедусер</span><span class="sxs-lookup"><span data-stu-id="d8316-179">impactedUser</span></span>|[<span data-ttu-id="d8316-180">user</span><span class="sxs-lookup"><span data-stu-id="d8316-180">user</span></span>](user.md)| <span data-ttu-id="d8316-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="d8316-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8316-183">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8316-183">JSON representation</span></span>

<span data-ttu-id="d8316-184">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8316-184">Here is a JSON representation of the resource.</span></span>

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