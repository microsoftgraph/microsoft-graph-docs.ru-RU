---
title: Тип ресурса Импоссиблетравелрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором два входа с учетной записью происходят из расположений нетипично для пользователя, и вы не сможете перемещаться между расположениями в период между входами. полная информация события риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
ms.openlocfilehash: d086a6fc127649da10184ae0396a2c58ee82964e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333605"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="ec665-103">Тип ресурса Импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="ec665-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec665-104">Событие риска, обнаруженное службой [удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , в котором два входа учетной записи происходят из расположений, нетипичных для пользователя, и вы не сможете перемещаться между расположениями в промежутке между входами. Complete сведения о событиях риска можно найти в [документации по защите удостоверенИй Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="ec665-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="ec665-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ec665-105">Methods</span></span>

| <span data-ttu-id="ec665-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ec665-106">Method</span></span>           | <span data-ttu-id="ec665-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ec665-107">Return Type</span></span>    |<span data-ttu-id="ec665-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ec665-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ec665-109">Получение объекта impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ec665-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="ec665-110">Импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="ec665-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="ec665-111">Чтение свойств и связей объекта Импоссиблетравелрискевент.</span><span class="sxs-lookup"><span data-stu-id="ec665-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ec665-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec665-112">Properties</span></span>
| <span data-ttu-id="ec665-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec665-113">Property</span></span>     | <span data-ttu-id="ec665-114">Тип</span><span class="sxs-lookup"><span data-stu-id="ec665-114">Type</span></span>   |<span data-ttu-id="ec665-115">Описание</span><span class="sxs-lookup"><span data-stu-id="ec665-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec665-116">Клоседдатетиме</span><span class="sxs-lookup"><span data-stu-id="ec665-116">closedDateTime</span></span>|<span data-ttu-id="ec665-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec665-117">dateTimeOffset</span></span>| <span data-ttu-id="ec665-118">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="ec665-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="ec665-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec665-119">createdDateTime</span></span>|<span data-ttu-id="ec665-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec665-120">dateTimeOffset</span></span>| <span data-ttu-id="ec665-121">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="ec665-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="ec665-122">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="ec665-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="ec665-123">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="ec665-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="ec665-124">Девицеинформатион</span><span class="sxs-lookup"><span data-stu-id="ec665-124">deviceInformation</span></span>|<span data-ttu-id="ec665-125">string</span><span class="sxs-lookup"><span data-stu-id="ec665-125">string</span></span>| <span data-ttu-id="ec665-126">Сведения об устройстве</span><span class="sxs-lookup"><span data-stu-id="ec665-126">Information about the device</span></span>|
|<span data-ttu-id="ec665-127">id</span><span class="sxs-lookup"><span data-stu-id="ec665-127">id</span></span>|<span data-ttu-id="ec665-128">строка</span><span class="sxs-lookup"><span data-stu-id="ec665-128">string</span></span>| <span data-ttu-id="ec665-129">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="ec665-129">Read-only</span></span>|
|<span data-ttu-id="ec665-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="ec665-130">ipAddress</span></span>|<span data-ttu-id="ec665-131">string</span><span class="sxs-lookup"><span data-stu-id="ec665-131">string</span></span>| <span data-ttu-id="ec665-132">IP-адрес второго входа</span><span class="sxs-lookup"><span data-stu-id="ec665-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="ec665-133">Исатипикаллокатион</span><span class="sxs-lookup"><span data-stu-id="ec665-133">isAtypicalLocation</span></span>|<span data-ttu-id="ec665-134">boolean</span><span class="sxs-lookup"><span data-stu-id="ec665-134">boolean</span></span>| <span data-ttu-id="ec665-135">Если одно из расположений для пользователя является нетипичным</span><span class="sxs-lookup"><span data-stu-id="ec665-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="ec665-136">location</span><span class="sxs-lookup"><span data-stu-id="ec665-136">location</span></span>|<span data-ttu-id="ec665-137">string</span><span class="sxs-lookup"><span data-stu-id="ec665-137">string</span></span>| <span data-ttu-id="ec665-138">Расположение, подключенное к IP-адресу второго входа</span><span class="sxs-lookup"><span data-stu-id="ec665-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="ec665-139">Превиаусипаддресс</span><span class="sxs-lookup"><span data-stu-id="ec665-139">previousIPAddress</span></span>|<span data-ttu-id="ec665-140">string</span><span class="sxs-lookup"><span data-stu-id="ec665-140">string</span></span>| <span data-ttu-id="ec665-141">IP-адрес первого входа</span><span class="sxs-lookup"><span data-stu-id="ec665-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="ec665-142">Превиауслокатион</span><span class="sxs-lookup"><span data-stu-id="ec665-142">previousLocation</span></span>|<span data-ttu-id="ec665-143">string</span><span class="sxs-lookup"><span data-stu-id="ec665-143">string</span></span>| <span data-ttu-id="ec665-144">Расположение, подключенное к IP-адресу первого входа</span><span class="sxs-lookup"><span data-stu-id="ec665-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="ec665-145">Превиауссигниндатетиме</span><span class="sxs-lookup"><span data-stu-id="ec665-145">previousSigninDateTime</span></span>|<span data-ttu-id="ec665-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec665-146">dateTimeOffset</span></span>| <span data-ttu-id="ec665-147">Дата и время первого входа</span><span class="sxs-lookup"><span data-stu-id="ec665-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="ec665-148">Рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="ec665-148">riskEventDateTime</span></span>|<span data-ttu-id="ec665-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec665-149">dateTimeOffset</span></span>| <span data-ttu-id="ec665-150">Дата и время второго входа</span><span class="sxs-lookup"><span data-stu-id="ec665-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="ec665-151">Рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="ec665-151">riskEventStatus</span></span>|<span data-ttu-id="ec665-152">string</span><span class="sxs-lookup"><span data-stu-id="ec665-152">string</span></span>| <span data-ttu-id="ec665-153">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="ec665-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="ec665-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ec665-154">riskLevel</span></span>|<span data-ttu-id="ec665-155">string</span><span class="sxs-lookup"><span data-stu-id="ec665-155">string</span></span>| <span data-ttu-id="ec665-156">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ec665-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="ec665-157">Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="ec665-157">riskEventType</span></span>|<span data-ttu-id="ec665-158">string</span><span class="sxs-lookup"><span data-stu-id="ec665-158">string</span></span>| <span data-ttu-id="ec665-159">Тип риска</span><span class="sxs-lookup"><span data-stu-id="ec665-159">The type of risk</span></span>|
|<span data-ttu-id="ec665-160">userAgent</span><span class="sxs-lookup"><span data-stu-id="ec665-160">userAgent</span></span>|<span data-ttu-id="ec665-161">string</span><span class="sxs-lookup"><span data-stu-id="ec665-161">string</span></span>| <span data-ttu-id="ec665-162">Строка агента пользователя браузера</span><span class="sxs-lookup"><span data-stu-id="ec665-162">The browser's user agent string</span></span>|
|<span data-ttu-id="ec665-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ec665-163">userDisplayName</span></span>|<span data-ttu-id="ec665-164">string</span><span class="sxs-lookup"><span data-stu-id="ec665-164">string</span></span>| <span data-ttu-id="ec665-165">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="ec665-165">The name of the user at risk</span></span>|
|<span data-ttu-id="ec665-166">userId</span><span class="sxs-lookup"><span data-stu-id="ec665-166">userId</span></span>|<span data-ttu-id="ec665-167">string</span><span class="sxs-lookup"><span data-stu-id="ec665-167">string</span></span>| <span data-ttu-id="ec665-168">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="ec665-168">The id of the user at risk</span></span>|
|<span data-ttu-id="ec665-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec665-169">userPrincipalName</span></span>|<span data-ttu-id="ec665-170">string</span><span class="sxs-lookup"><span data-stu-id="ec665-170">string</span></span>| <span data-ttu-id="ec665-171">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="ec665-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec665-172">Отношения</span><span class="sxs-lookup"><span data-stu-id="ec665-172">Relationships</span></span>
| <span data-ttu-id="ec665-173">Отношение</span><span class="sxs-lookup"><span data-stu-id="ec665-173">Relationship</span></span> | <span data-ttu-id="ec665-174">Тип</span><span class="sxs-lookup"><span data-stu-id="ec665-174">Type</span></span>   |<span data-ttu-id="ec665-175">Описание</span><span class="sxs-lookup"><span data-stu-id="ec665-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec665-176">Импактедусер</span><span class="sxs-lookup"><span data-stu-id="ec665-176">impactedUser</span></span>|[<span data-ttu-id="ec665-177">user</span><span class="sxs-lookup"><span data-stu-id="ec665-177">user</span></span>](user.md)| <span data-ttu-id="ec665-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ec665-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec665-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec665-180">JSON representation</span></span>

<span data-ttu-id="ec665-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec665-181">Here is a JSON representation of the resource.</span></span>

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
