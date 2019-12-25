---
title: Тип ресурса Импоссиблетравелрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором два входа с учетной записью происходят из расположений нетипично для пользователя, и вы не сможете перемещаться между расположениями в период между входами. полная информация события риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: be2b5db09a20264525e783e05771f6d1da2783e2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866786"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="0b055-103">Тип ресурса Импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="0b055-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="0b055-104">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="0b055-104">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="0b055-105">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="0b055-105">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="0b055-106">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) , в котором два входа учетной записи происходят из расположений нетипично для пользователя, и вы не сможете перемещаться между расположениями в период между входами. полные сведения о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="0b055-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="0b055-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0b055-107">Methods</span></span>

| <span data-ttu-id="0b055-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0b055-108">Method</span></span>           | <span data-ttu-id="0b055-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0b055-109">Return Type</span></span>    |<span data-ttu-id="0b055-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0b055-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b055-111">Получение объекта impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="0b055-111">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="0b055-112">импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="0b055-112">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="0b055-113">Чтение свойств и связей объекта Импоссиблетравелрискевент.</span><span class="sxs-lookup"><span data-stu-id="0b055-113">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b055-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b055-114">Properties</span></span>
| <span data-ttu-id="0b055-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b055-115">Property</span></span>     | <span data-ttu-id="0b055-116">Тип</span><span class="sxs-lookup"><span data-stu-id="0b055-116">Type</span></span>   |<span data-ttu-id="0b055-117">Описание</span><span class="sxs-lookup"><span data-stu-id="0b055-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b055-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b055-118">closedDateTime</span></span>|<span data-ttu-id="0b055-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b055-119">dateTimeOffset</span></span>| <span data-ttu-id="0b055-120">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="0b055-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="0b055-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b055-121">createdDateTime</span></span>|<span data-ttu-id="0b055-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b055-122">dateTimeOffset</span></span>| <span data-ttu-id="0b055-123">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="0b055-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="0b055-124">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="0b055-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="0b055-125">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="0b055-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="0b055-126">девицеинформатион</span><span class="sxs-lookup"><span data-stu-id="0b055-126">deviceInformation</span></span>|<span data-ttu-id="0b055-127">string</span><span class="sxs-lookup"><span data-stu-id="0b055-127">string</span></span>| <span data-ttu-id="0b055-128">Сведения об устройстве</span><span class="sxs-lookup"><span data-stu-id="0b055-128">Information about the device</span></span>|
|<span data-ttu-id="0b055-129">id</span><span class="sxs-lookup"><span data-stu-id="0b055-129">id</span></span>|<span data-ttu-id="0b055-130">string</span><span class="sxs-lookup"><span data-stu-id="0b055-130">string</span></span>| <span data-ttu-id="0b055-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="0b055-131">Read-only</span></span>|
|<span data-ttu-id="0b055-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0b055-132">ipAddress</span></span>|<span data-ttu-id="0b055-133">string</span><span class="sxs-lookup"><span data-stu-id="0b055-133">string</span></span>| <span data-ttu-id="0b055-134">IP-адрес второго входа</span><span class="sxs-lookup"><span data-stu-id="0b055-134">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="0b055-135">исатипикаллокатион</span><span class="sxs-lookup"><span data-stu-id="0b055-135">isAtypicalLocation</span></span>|<span data-ttu-id="0b055-136">boolean</span><span class="sxs-lookup"><span data-stu-id="0b055-136">boolean</span></span>| <span data-ttu-id="0b055-137">Если одно из расположений для пользователя является нетипичным</span><span class="sxs-lookup"><span data-stu-id="0b055-137">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="0b055-138">location</span><span class="sxs-lookup"><span data-stu-id="0b055-138">location</span></span>|<span data-ttu-id="0b055-139">string</span><span class="sxs-lookup"><span data-stu-id="0b055-139">string</span></span>| <span data-ttu-id="0b055-140">Расположение, подключенное к IP-адресу второго входа</span><span class="sxs-lookup"><span data-stu-id="0b055-140">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="0b055-141">превиаусипаддресс</span><span class="sxs-lookup"><span data-stu-id="0b055-141">previousIPAddress</span></span>|<span data-ttu-id="0b055-142">string</span><span class="sxs-lookup"><span data-stu-id="0b055-142">string</span></span>| <span data-ttu-id="0b055-143">IP-адрес первого входа</span><span class="sxs-lookup"><span data-stu-id="0b055-143">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="0b055-144">превиауслокатион</span><span class="sxs-lookup"><span data-stu-id="0b055-144">previousLocation</span></span>|<span data-ttu-id="0b055-145">string</span><span class="sxs-lookup"><span data-stu-id="0b055-145">string</span></span>| <span data-ttu-id="0b055-146">Расположение, подключенное к IP-адресу первого входа</span><span class="sxs-lookup"><span data-stu-id="0b055-146">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="0b055-147">превиауссигниндатетиме</span><span class="sxs-lookup"><span data-stu-id="0b055-147">previousSigninDateTime</span></span>|<span data-ttu-id="0b055-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b055-148">dateTimeOffset</span></span>| <span data-ttu-id="0b055-149">Дата и время первого входа</span><span class="sxs-lookup"><span data-stu-id="0b055-149">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="0b055-150">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="0b055-150">riskEventDateTime</span></span>|<span data-ttu-id="0b055-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b055-151">dateTimeOffset</span></span>| <span data-ttu-id="0b055-152">Дата и время второго входа</span><span class="sxs-lookup"><span data-stu-id="0b055-152">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="0b055-153">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="0b055-153">riskEventStatus</span></span>|<span data-ttu-id="0b055-154">string</span><span class="sxs-lookup"><span data-stu-id="0b055-154">string</span></span>| <span data-ttu-id="0b055-155">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="0b055-155">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="0b055-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0b055-156">riskLevel</span></span>|<span data-ttu-id="0b055-157">string</span><span class="sxs-lookup"><span data-stu-id="0b055-157">string</span></span>| <span data-ttu-id="0b055-158">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="0b055-158">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="0b055-159">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="0b055-159">riskEventType</span></span>|<span data-ttu-id="0b055-160">string</span><span class="sxs-lookup"><span data-stu-id="0b055-160">string</span></span>| <span data-ttu-id="0b055-161">Тип риска</span><span class="sxs-lookup"><span data-stu-id="0b055-161">The type of risk</span></span>|
|<span data-ttu-id="0b055-162">userAgent</span><span class="sxs-lookup"><span data-stu-id="0b055-162">userAgent</span></span>|<span data-ttu-id="0b055-163">string</span><span class="sxs-lookup"><span data-stu-id="0b055-163">string</span></span>| <span data-ttu-id="0b055-164">Строка агента пользователя браузера</span><span class="sxs-lookup"><span data-stu-id="0b055-164">The browser's user agent string</span></span>|
|<span data-ttu-id="0b055-165">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0b055-165">userDisplayName</span></span>|<span data-ttu-id="0b055-166">string</span><span class="sxs-lookup"><span data-stu-id="0b055-166">string</span></span>| <span data-ttu-id="0b055-167">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="0b055-167">The name of the user at risk</span></span>|
|<span data-ttu-id="0b055-168">userId</span><span class="sxs-lookup"><span data-stu-id="0b055-168">userId</span></span>|<span data-ttu-id="0b055-169">строка</span><span class="sxs-lookup"><span data-stu-id="0b055-169">string</span></span>| <span data-ttu-id="0b055-170">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="0b055-170">The id of the user at risk</span></span>|
|<span data-ttu-id="0b055-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0b055-171">userPrincipalName</span></span>|<span data-ttu-id="0b055-172">string</span><span class="sxs-lookup"><span data-stu-id="0b055-172">string</span></span>| <span data-ttu-id="0b055-173">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="0b055-173">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b055-174">Отношения</span><span class="sxs-lookup"><span data-stu-id="0b055-174">Relationships</span></span>
| <span data-ttu-id="0b055-175">Связь</span><span class="sxs-lookup"><span data-stu-id="0b055-175">Relationship</span></span> | <span data-ttu-id="0b055-176">Тип</span><span class="sxs-lookup"><span data-stu-id="0b055-176">Type</span></span>   |<span data-ttu-id="0b055-177">Описание</span><span class="sxs-lookup"><span data-stu-id="0b055-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b055-178">импактедусер</span><span class="sxs-lookup"><span data-stu-id="0b055-178">impactedUser</span></span>|[<span data-ttu-id="0b055-179">user</span><span class="sxs-lookup"><span data-stu-id="0b055-179">user</span></span>](user.md)| <span data-ttu-id="0b055-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="0b055-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b055-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b055-182">JSON representation</span></span>

<span data-ttu-id="0b055-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b055-183">Here is a JSON representation of the resource.</span></span>

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
