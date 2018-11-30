---
title: Тип ресурса impossibleTravelRiskEvent
description: События риска обнаруживается Azure Active Directory защиту которых возникают два учетной записи войти в систему из мест необычных для пользователя и невозможно в поездке между различными расположениями в интервал между которые запускаются входа полные сведения о события рисков можно найти в документации по Azure AD защиту.
ms.openlocfilehash: 38e61927121f520e79fd1fec8b8e6443fa8b76e7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075119"
---
# <a name="impossibletravelriskevent-resource-type"></a><span data-ttu-id="6553a-103">Тип ресурса impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="6553a-103">impossibleTravelRiskEvent resource type</span></span>

> <span data-ttu-id="6553a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6553a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6553a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6553a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6553a-106">События риска обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) которых возникают два учетной записи войти в систему из мест необычных для пользователя и невозможно в поездке между различными расположениями в интервал между полная которые запускаются входа сведения о мероприятиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="6553a-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where two account sign-ins occur from locations atypical for the user and it would be impossible to travel between the locations in the duration between the sign-ins. Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="6553a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6553a-107">Methods</span></span>

| <span data-ttu-id="6553a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6553a-108">Method</span></span>           | <span data-ttu-id="6553a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6553a-109">Return Type</span></span>    |<span data-ttu-id="6553a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6553a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6553a-111">Получение impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="6553a-111">Get impossibleTravelRiskEvent</span></span>](../api/impossibletravelriskevent-get.md) | [<span data-ttu-id="6553a-112">impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="6553a-112">impossibleTravelRiskEvent</span></span>](impossibletravelriskevent.md) |<span data-ttu-id="6553a-113">Чтение свойства и связи объекта impossibleTravelRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="6553a-113">Read properties and relationships of impossibleTravelRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6553a-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="6553a-114">Properties</span></span>
| <span data-ttu-id="6553a-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="6553a-115">Property</span></span>     | <span data-ttu-id="6553a-116">Тип</span><span class="sxs-lookup"><span data-stu-id="6553a-116">Type</span></span>   |<span data-ttu-id="6553a-117">Description</span><span class="sxs-lookup"><span data-stu-id="6553a-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6553a-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="6553a-118">closedDateTime</span></span>|<span data-ttu-id="6553a-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6553a-119">dateTimeOffset</span></span>| <span data-ttu-id="6553a-120">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="6553a-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="6553a-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6553a-121">createdDateTime</span></span>|<span data-ttu-id="6553a-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6553a-122">dateTimeOffset</span></span>| <span data-ttu-id="6553a-123">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="6553a-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="6553a-124">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="6553a-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="6553a-125">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="6553a-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="6553a-126">deviceInformation</span><span class="sxs-lookup"><span data-stu-id="6553a-126">deviceInformation</span></span>|<span data-ttu-id="6553a-127">string</span><span class="sxs-lookup"><span data-stu-id="6553a-127">string</span></span>| <span data-ttu-id="6553a-128">Сведения об устройстве</span><span class="sxs-lookup"><span data-stu-id="6553a-128">Information about the device</span></span>|
|<span data-ttu-id="6553a-129">id</span><span class="sxs-lookup"><span data-stu-id="6553a-129">id</span></span>|<span data-ttu-id="6553a-130">строка</span><span class="sxs-lookup"><span data-stu-id="6553a-130">string</span></span>| <span data-ttu-id="6553a-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="6553a-131">Read-only</span></span>|
|<span data-ttu-id="6553a-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6553a-132">ipAddress</span></span>|<span data-ttu-id="6553a-133">string</span><span class="sxs-lookup"><span data-stu-id="6553a-133">string</span></span>| <span data-ttu-id="6553a-134">IP-адрес второго входа в</span><span class="sxs-lookup"><span data-stu-id="6553a-134">The IP address of the second sign-in</span></span>|
|<span data-ttu-id="6553a-135">isAtypicalLocation</span><span class="sxs-lookup"><span data-stu-id="6553a-135">isAtypicalLocation</span></span>|<span data-ttu-id="6553a-136">boolean</span><span class="sxs-lookup"><span data-stu-id="6553a-136">boolean</span></span>| <span data-ttu-id="6553a-137">Если выполняется одно из расположений необычных для пользователя</span><span class="sxs-lookup"><span data-stu-id="6553a-137">If one of the locations is atypical for the user</span></span>|
|<span data-ttu-id="6553a-138">location</span><span class="sxs-lookup"><span data-stu-id="6553a-138">location</span></span>|<span data-ttu-id="6553a-139">string</span><span class="sxs-lookup"><span data-stu-id="6553a-139">string</span></span>| <span data-ttu-id="6553a-140">Расположение, подключенного к IP-адрес второго входа в</span><span class="sxs-lookup"><span data-stu-id="6553a-140">The location attached to the IP address of the second sign-in</span></span>|
|<span data-ttu-id="6553a-141">previousIPAddress</span><span class="sxs-lookup"><span data-stu-id="6553a-141">previousIPAddress</span></span>|<span data-ttu-id="6553a-142">string</span><span class="sxs-lookup"><span data-stu-id="6553a-142">string</span></span>| <span data-ttu-id="6553a-143">IP-адрес первого входа в</span><span class="sxs-lookup"><span data-stu-id="6553a-143">The IP address of the first sign-in</span></span>|
|<span data-ttu-id="6553a-144">previousLocation</span><span class="sxs-lookup"><span data-stu-id="6553a-144">previousLocation</span></span>|<span data-ttu-id="6553a-145">string</span><span class="sxs-lookup"><span data-stu-id="6553a-145">string</span></span>| <span data-ttu-id="6553a-146">Расположение, подключенного к IP-адрес первого входа в</span><span class="sxs-lookup"><span data-stu-id="6553a-146">The location attached to the IP address of the first sign-in</span></span>|
|<span data-ttu-id="6553a-147">previousSigninDateTime</span><span class="sxs-lookup"><span data-stu-id="6553a-147">previousSigninDateTime</span></span>|<span data-ttu-id="6553a-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6553a-148">dateTimeOffset</span></span>| <span data-ttu-id="6553a-149">Дата и время первого входа в</span><span class="sxs-lookup"><span data-stu-id="6553a-149">The date and time of the first sign-in</span></span>|
|<span data-ttu-id="6553a-150">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="6553a-150">riskEventDateTime</span></span>|<span data-ttu-id="6553a-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6553a-151">dateTimeOffset</span></span>| <span data-ttu-id="6553a-152">Дата и время второго входа в</span><span class="sxs-lookup"><span data-stu-id="6553a-152">The date and time of the second sign-in</span></span>|
|<span data-ttu-id="6553a-153">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="6553a-153">riskEventStatus</span></span>|<span data-ttu-id="6553a-154">string</span><span class="sxs-lookup"><span data-stu-id="6553a-154">string</span></span>| <span data-ttu-id="6553a-155">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="6553a-155">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="6553a-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="6553a-156">riskLevel</span></span>|<span data-ttu-id="6553a-157">string</span><span class="sxs-lookup"><span data-stu-id="6553a-157">string</span></span>| <span data-ttu-id="6553a-158">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="6553a-158">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="6553a-159">riskEventType</span><span class="sxs-lookup"><span data-stu-id="6553a-159">riskEventType</span></span>|<span data-ttu-id="6553a-160">string</span><span class="sxs-lookup"><span data-stu-id="6553a-160">string</span></span>| <span data-ttu-id="6553a-161">Тип риска</span><span class="sxs-lookup"><span data-stu-id="6553a-161">The type of risk</span></span>|
|<span data-ttu-id="6553a-162">userAgent</span><span class="sxs-lookup"><span data-stu-id="6553a-162">userAgent</span></span>|<span data-ttu-id="6553a-163">string</span><span class="sxs-lookup"><span data-stu-id="6553a-163">string</span></span>| <span data-ttu-id="6553a-164">Строка агента пользователя в браузере</span><span class="sxs-lookup"><span data-stu-id="6553a-164">The browser's user agent string</span></span>|
|<span data-ttu-id="6553a-165">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6553a-165">userDisplayName</span></span>|<span data-ttu-id="6553a-166">string</span><span class="sxs-lookup"><span data-stu-id="6553a-166">string</span></span>| <span data-ttu-id="6553a-167">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="6553a-167">The name of the user at risk</span></span>|
|<span data-ttu-id="6553a-168">userId</span><span class="sxs-lookup"><span data-stu-id="6553a-168">userId</span></span>|<span data-ttu-id="6553a-169">string</span><span class="sxs-lookup"><span data-stu-id="6553a-169">string</span></span>| <span data-ttu-id="6553a-170">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="6553a-170">The id of the user at risk</span></span>|
|<span data-ttu-id="6553a-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6553a-171">userPrincipalName</span></span>|<span data-ttu-id="6553a-172">string</span><span class="sxs-lookup"><span data-stu-id="6553a-172">string</span></span>| <span data-ttu-id="6553a-173">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="6553a-173">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="6553a-174">Связи</span><span class="sxs-lookup"><span data-stu-id="6553a-174">Relationships</span></span>
| <span data-ttu-id="6553a-175">Связь</span><span class="sxs-lookup"><span data-stu-id="6553a-175">Relationship</span></span> | <span data-ttu-id="6553a-176">Тип</span><span class="sxs-lookup"><span data-stu-id="6553a-176">Type</span></span>   |<span data-ttu-id="6553a-177">Description</span><span class="sxs-lookup"><span data-stu-id="6553a-177">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6553a-178">impactedUser</span><span class="sxs-lookup"><span data-stu-id="6553a-178">impactedUser</span></span>|[<span data-ttu-id="6553a-179">user</span><span class="sxs-lookup"><span data-stu-id="6553a-179">user</span></span>](user.md)| <span data-ttu-id="6553a-p103">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="6553a-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6553a-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6553a-182">JSON representation</span></span>

<span data-ttu-id="6553a-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6553a-183">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->