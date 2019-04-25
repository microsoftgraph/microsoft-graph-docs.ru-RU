---
title: Тип ресурса Импоссиблетравелрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором два входа с учетной записью происходят из расположений нетипично для пользователя, и вы не сможете перемещаться между расположениями в период между входами. полная информация события риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548329"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="619af-103">Тип ресурса Импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="619af-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="619af-104">Событие риска, обнаруженное службой [удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , в котором два входа учетной записи происходят из расположений, нетипичных для пользователя, и вы не сможете перемещаться между расположениями в промежутке между входами. Complete сведения о событиях риска можно найти в [документации по защите удостоверенИй Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="619af-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="619af-105">Методы</span><span class="sxs-lookup"><span data-stu-id="619af-105">Methods</span></span>

| <span data-ttu-id="619af-106">Метод</span><span class="sxs-lookup"><span data-stu-id="619af-106">Method</span></span>           | <span data-ttu-id="619af-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="619af-107">Return Type</span></span>    |<span data-ttu-id="619af-108">Описание</span><span class="sxs-lookup"><span data-stu-id="619af-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="619af-109">Получение объекта impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="619af-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="619af-110">Импоссиблетравелрискевент</span><span class="sxs-lookup"><span data-stu-id="619af-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="619af-111">Чтение свойств и связей объекта Импоссиблетравелрискевент.</span><span class="sxs-lookup"><span data-stu-id="619af-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="619af-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="619af-112">Properties</span></span>
| <span data-ttu-id="619af-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="619af-113">Property</span></span>     | <span data-ttu-id="619af-114">Тип</span><span class="sxs-lookup"><span data-stu-id="619af-114">Type</span></span>   |<span data-ttu-id="619af-115">Описание</span><span class="sxs-lookup"><span data-stu-id="619af-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="619af-116">Клоседдатетиме</span><span class="sxs-lookup"><span data-stu-id="619af-116">closedDateTime</span></span>|<span data-ttu-id="619af-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="619af-117">dateTimeOffset</span></span>| <span data-ttu-id="619af-118">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="619af-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="619af-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="619af-119">createdDateTime</span></span>|<span data-ttu-id="619af-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="619af-120">dateTimeOffset</span></span>| <span data-ttu-id="619af-121">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="619af-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="619af-122">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="619af-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="619af-123">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="619af-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="619af-124">Девицеинформатион</span><span class="sxs-lookup"><span data-stu-id="619af-124">deviceInformation</span></span>|<span data-ttu-id="619af-125">string</span><span class="sxs-lookup"><span data-stu-id="619af-125">string</span></span>| <span data-ttu-id="619af-126">Сведения об устройстве</span><span class="sxs-lookup"><span data-stu-id="619af-126">Information about the device</span></span>|
|<span data-ttu-id="619af-127">id</span><span class="sxs-lookup"><span data-stu-id="619af-127">id</span></span>|<span data-ttu-id="619af-128">string</span><span class="sxs-lookup"><span data-stu-id="619af-128">string</span></span>| <span data-ttu-id="619af-129">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="619af-129">Read-only</span></span>|
|<span data-ttu-id="619af-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="619af-130">ipAddress</span></span>|<span data-ttu-id="619af-131">string</span><span class="sxs-lookup"><span data-stu-id="619af-131">string</span></span>| <span data-ttu-id="619af-132">IP-адрес второго входа</span><span class="sxs-lookup"><span data-stu-id="619af-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="619af-133">Исатипикаллокатион</span><span class="sxs-lookup"><span data-stu-id="619af-133">isAtypicalLocation</span></span>|<span data-ttu-id="619af-134">логический</span><span class="sxs-lookup"><span data-stu-id="619af-134">boolean</span></span>| <span data-ttu-id="619af-135">Если одно из расположений для пользователя является нетипичным</span><span class="sxs-lookup"><span data-stu-id="619af-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="619af-136">location</span><span class="sxs-lookup"><span data-stu-id="619af-136">location</span></span>|<span data-ttu-id="619af-137">string</span><span class="sxs-lookup"><span data-stu-id="619af-137">string</span></span>| <span data-ttu-id="619af-138">Расположение, подключенное к IP-адресу второго входа</span><span class="sxs-lookup"><span data-stu-id="619af-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="619af-139">Превиаусипаддресс</span><span class="sxs-lookup"><span data-stu-id="619af-139">previousIPAddress</span></span>|<span data-ttu-id="619af-140">string</span><span class="sxs-lookup"><span data-stu-id="619af-140">string</span></span>| <span data-ttu-id="619af-141">IP-адрес первого входа</span><span class="sxs-lookup"><span data-stu-id="619af-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="619af-142">Превиауслокатион</span><span class="sxs-lookup"><span data-stu-id="619af-142">previousLocation</span></span>|<span data-ttu-id="619af-143">string</span><span class="sxs-lookup"><span data-stu-id="619af-143">string</span></span>| <span data-ttu-id="619af-144">Расположение, подключенное к IP-адресу первого входа</span><span class="sxs-lookup"><span data-stu-id="619af-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="619af-145">Превиауссигниндатетиме</span><span class="sxs-lookup"><span data-stu-id="619af-145">previousSigninDateTime</span></span>|<span data-ttu-id="619af-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="619af-146">dateTimeOffset</span></span>| <span data-ttu-id="619af-147">Дата и время первого входа</span><span class="sxs-lookup"><span data-stu-id="619af-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="619af-148">Рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="619af-148">riskEventDateTime</span></span>|<span data-ttu-id="619af-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="619af-149">dateTimeOffset</span></span>| <span data-ttu-id="619af-150">Дата и время второго входа</span><span class="sxs-lookup"><span data-stu-id="619af-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="619af-151">Рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="619af-151">riskEventStatus</span></span>|<span data-ttu-id="619af-152">string</span><span class="sxs-lookup"><span data-stu-id="619af-152">string</span></span>| <span data-ttu-id="619af-153">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="619af-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="619af-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="619af-154">riskLevel</span></span>|<span data-ttu-id="619af-155">string</span><span class="sxs-lookup"><span data-stu-id="619af-155">string</span></span>| <span data-ttu-id="619af-156">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="619af-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="619af-157">Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="619af-157">riskEventType</span></span>|<span data-ttu-id="619af-158">string</span><span class="sxs-lookup"><span data-stu-id="619af-158">string</span></span>| <span data-ttu-id="619af-159">Тип риска</span><span class="sxs-lookup"><span data-stu-id="619af-159">The type of risk</span></span>|
|<span data-ttu-id="619af-160">userAgent</span><span class="sxs-lookup"><span data-stu-id="619af-160">userAgent</span></span>|<span data-ttu-id="619af-161">string</span><span class="sxs-lookup"><span data-stu-id="619af-161">string</span></span>| <span data-ttu-id="619af-162">Строка агента пользователя браузера</span><span class="sxs-lookup"><span data-stu-id="619af-162">The browser's user agent string</span></span>|
|<span data-ttu-id="619af-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="619af-163">userDisplayName</span></span>|<span data-ttu-id="619af-164">string</span><span class="sxs-lookup"><span data-stu-id="619af-164">string</span></span>| <span data-ttu-id="619af-165">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="619af-165">The name of the user at risk</span></span>|
|<span data-ttu-id="619af-166">userId</span><span class="sxs-lookup"><span data-stu-id="619af-166">userId</span></span>|<span data-ttu-id="619af-167">string</span><span class="sxs-lookup"><span data-stu-id="619af-167">string</span></span>| <span data-ttu-id="619af-168">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="619af-168">The id of the user at risk</span></span>|
|<span data-ttu-id="619af-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="619af-169">userPrincipalName</span></span>|<span data-ttu-id="619af-170">string</span><span class="sxs-lookup"><span data-stu-id="619af-170">string</span></span>| <span data-ttu-id="619af-171">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="619af-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="619af-172">Связи</span><span class="sxs-lookup"><span data-stu-id="619af-172">Relationships</span></span>
| <span data-ttu-id="619af-173">Отношение</span><span class="sxs-lookup"><span data-stu-id="619af-173">Relationship</span></span> | <span data-ttu-id="619af-174">Тип</span><span class="sxs-lookup"><span data-stu-id="619af-174">Type</span></span>   |<span data-ttu-id="619af-175">Описание</span><span class="sxs-lookup"><span data-stu-id="619af-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="619af-176">Импактедусер</span><span class="sxs-lookup"><span data-stu-id="619af-176">impactedUser</span></span>|[<span data-ttu-id="619af-177">user</span><span class="sxs-lookup"><span data-stu-id="619af-177">user</span></span>](user.md)| <span data-ttu-id="619af-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="619af-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="619af-180">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="619af-180">JSON representation</span></span>

<span data-ttu-id="619af-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="619af-181">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/impossibletravelriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
