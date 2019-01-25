---
title: Тип ресурса impossibleTravelRiskEvent
description: События риска обнаруживается Azure Active Directory защиту которых возникают два учетной записи войти в систему из мест необычных для пользователя и невозможно в поездке между различными расположениями в интервал между которые запускаются входа полные сведения о события рисков можно найти в документации по Azure AD защиту.
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529385"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="594af-103">Тип ресурса impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="594af-103">impossibleTravelRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="594af-104">События риска обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) которых возникают два учетной записи войти в систему из мест необычных для пользователя и невозможно в поездке между различными расположениями в интервал между полная которые запускаются входа сведения о мероприятиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="594af-104">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="594af-105">Методы</span><span class="sxs-lookup"><span data-stu-id="594af-105">Methods</span></span>

| <span data-ttu-id="594af-106">Метод</span><span class="sxs-lookup"><span data-stu-id="594af-106">Method</span></span>           | <span data-ttu-id="594af-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="594af-107">Return Type</span></span>    |<span data-ttu-id="594af-108">Описание</span><span class="sxs-lookup"><span data-stu-id="594af-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="594af-109">Получение impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="594af-109">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="594af-110">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="594af-110">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="594af-111">Чтение свойства и связи объекта impossibleTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="594af-111">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="594af-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="594af-112">Properties</span></span>
| <span data-ttu-id="594af-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="594af-113">Property</span></span>     | <span data-ttu-id="594af-114">Тип</span><span class="sxs-lookup"><span data-stu-id="594af-114">Type</span></span>   |<span data-ttu-id="594af-115">Описание</span><span class="sxs-lookup"><span data-stu-id="594af-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="594af-116">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="594af-116">closedDateTime</span></span>|<span data-ttu-id="594af-117">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="594af-117">dateTimeOffset</span></span>| <span data-ttu-id="594af-118">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="594af-118">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="594af-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="594af-119">createdDateTime</span></span>|<span data-ttu-id="594af-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="594af-120">dateTimeOffset</span></span>| <span data-ttu-id="594af-121">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="594af-121">The date and time that the risk event was created.</span></span> <span data-ttu-id="594af-122">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="594af-122">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="594af-123">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="594af-123">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="594af-124">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="594af-124">deviceInformation</span></span>|<span data-ttu-id="594af-125">string</span><span class="sxs-lookup"><span data-stu-id="594af-125">string</span></span>| <span data-ttu-id="594af-126">Сведения об устройстве</span><span class="sxs-lookup"><span data-stu-id="594af-126">Information about the device</span></span>|
|<span data-ttu-id="594af-127">id</span><span class="sxs-lookup"><span data-stu-id="594af-127">id</span></span>|<span data-ttu-id="594af-128">string</span><span class="sxs-lookup"><span data-stu-id="594af-128">string</span></span>| <span data-ttu-id="594af-129">Только чтение</span><span class="sxs-lookup"><span data-stu-id="594af-129">Read-only</span></span>|
|<span data-ttu-id="594af-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="594af-130">ipAddress</span></span>|<span data-ttu-id="594af-131">string</span><span class="sxs-lookup"><span data-stu-id="594af-131">string</span></span>| <span data-ttu-id="594af-132">IP-адрес второго входа в</span><span class="sxs-lookup"><span data-stu-id="594af-132">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="594af-133">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="594af-133">isAtypicalLocation</span></span>|<span data-ttu-id="594af-134">boolean</span><span class="sxs-lookup"><span data-stu-id="594af-134">boolean</span></span>| <span data-ttu-id="594af-135">Если выполняется одно из расположений необычных для пользователя</span><span class="sxs-lookup"><span data-stu-id="594af-135">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="594af-136">location</span><span class="sxs-lookup"><span data-stu-id="594af-136">location</span></span>|<span data-ttu-id="594af-137">string</span><span class="sxs-lookup"><span data-stu-id="594af-137">string</span></span>| <span data-ttu-id="594af-138">Расположение, подключенного к IP-адрес второго входа в</span><span class="sxs-lookup"><span data-stu-id="594af-138">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="594af-139">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="594af-139">previousIPAddress</span></span>|<span data-ttu-id="594af-140">string</span><span class="sxs-lookup"><span data-stu-id="594af-140">string</span></span>| <span data-ttu-id="594af-141">IP-адрес первого входа в</span><span class="sxs-lookup"><span data-stu-id="594af-141">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="594af-142">previousLocation</span><span class="sxs-lookup"><span data-stu-id="594af-142">previousLocation</span></span>|<span data-ttu-id="594af-143">string</span><span class="sxs-lookup"><span data-stu-id="594af-143">string</span></span>| <span data-ttu-id="594af-144">Расположение, подключенного к IP-адрес первого входа в</span><span class="sxs-lookup"><span data-stu-id="594af-144">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="594af-145">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="594af-145">previousSigninDateTime</span></span>|<span data-ttu-id="594af-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="594af-146">dateTimeOffset</span></span>| <span data-ttu-id="594af-147">Дата и время первого входа в</span><span class="sxs-lookup"><span data-stu-id="594af-147">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="594af-148">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="594af-148">riskEventDateTime</span></span>|<span data-ttu-id="594af-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="594af-149">dateTimeOffset</span></span>| <span data-ttu-id="594af-150">Дата и время второго входа в</span><span class="sxs-lookup"><span data-stu-id="594af-150">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="594af-151">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="594af-151">riskEventStatus</span></span>|<span data-ttu-id="594af-152">string</span><span class="sxs-lookup"><span data-stu-id="594af-152">string</span></span>| <span data-ttu-id="594af-153">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="594af-153">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="594af-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="594af-154">riskLevel</span></span>|<span data-ttu-id="594af-155">string</span><span class="sxs-lookup"><span data-stu-id="594af-155">string</span></span>| <span data-ttu-id="594af-156">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="594af-156">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="594af-157">riskEventType</span><span class="sxs-lookup"><span data-stu-id="594af-157">riskEventType</span></span>|<span data-ttu-id="594af-158">string</span><span class="sxs-lookup"><span data-stu-id="594af-158">string</span></span>| <span data-ttu-id="594af-159">Тип риска</span><span class="sxs-lookup"><span data-stu-id="594af-159">The type of risk</span></span>|
|<span data-ttu-id="594af-160">UserAgent</span><span class="sxs-lookup"><span data-stu-id="594af-160">userAgent</span></span>|<span data-ttu-id="594af-161">string</span><span class="sxs-lookup"><span data-stu-id="594af-161">string</span></span>| <span data-ttu-id="594af-162">Строка агента пользователя в браузере</span><span class="sxs-lookup"><span data-stu-id="594af-162">The browser's user agent string</span></span>|
|<span data-ttu-id="594af-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="594af-163">userDisplayName</span></span>|<span data-ttu-id="594af-164">string</span><span class="sxs-lookup"><span data-stu-id="594af-164">string</span></span>| <span data-ttu-id="594af-165">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="594af-165">The name of the user at risk</span></span>|
|<span data-ttu-id="594af-166">userId</span><span class="sxs-lookup"><span data-stu-id="594af-166">userId</span></span>|<span data-ttu-id="594af-167">string</span><span class="sxs-lookup"><span data-stu-id="594af-167">string</span></span>| <span data-ttu-id="594af-168">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="594af-168">The id of the user at risk</span></span>|
|<span data-ttu-id="594af-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="594af-169">userPrincipalName</span></span>|<span data-ttu-id="594af-170">string</span><span class="sxs-lookup"><span data-stu-id="594af-170">string</span></span>| <span data-ttu-id="594af-171">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="594af-171">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="594af-172">Отношения</span><span class="sxs-lookup"><span data-stu-id="594af-172">Relationships</span></span>
| <span data-ttu-id="594af-173">Связь</span><span class="sxs-lookup"><span data-stu-id="594af-173">Relationship</span></span> | <span data-ttu-id="594af-174">Тип</span><span class="sxs-lookup"><span data-stu-id="594af-174">Type</span></span>   |<span data-ttu-id="594af-175">Описание</span><span class="sxs-lookup"><span data-stu-id="594af-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="594af-176">impactedUser</span><span class="sxs-lookup"><span data-stu-id="594af-176">impactedUser</span></span>|[<span data-ttu-id="594af-177">user</span><span class="sxs-lookup"><span data-stu-id="594af-177">user</span></span>](user.md)| <span data-ttu-id="594af-p102">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="594af-p102">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="594af-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="594af-180">JSON representation</span></span>

<span data-ttu-id="594af-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="594af-181">Here is a JSON representation of the resource.</span></span>

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
