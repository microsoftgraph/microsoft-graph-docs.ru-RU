---
title: Тип ресурса suspiciousIpRiskEvent
description: Событие риск, обнаруженных защитой Azure Active Directory Identity которых учетной записи входа в попытке с подозрительные IP-адреса. Полные сведения о событиях риска можно найти в документации по Azure AD защиту.
ms.openlocfilehash: 5d5b2da25c926a88eb7b589d562e6fa9ec914338
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080807"
---
# <a name="suspiciousipriskevent-resource-type"></a><span data-ttu-id="34f60-104">Тип ресурса suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34f60-104">suspiciousIpRiskEvent resource type</span></span>

> <span data-ttu-id="34f60-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="34f60-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34f60-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34f60-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34f60-107">Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , где учетной записи входа в попытке с подозрительные IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="34f60-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a suspicious IP address.</span></span> <span data-ttu-id="34f60-108">Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="34f60-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="34f60-109">Методы</span><span class="sxs-lookup"><span data-stu-id="34f60-109">Methods</span></span>

| <span data-ttu-id="34f60-110">Метод</span><span class="sxs-lookup"><span data-stu-id="34f60-110">Method</span></span>           | <span data-ttu-id="34f60-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="34f60-111">Return Type</span></span>    |<span data-ttu-id="34f60-112">Описание</span><span class="sxs-lookup"><span data-stu-id="34f60-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="34f60-113">Получение suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34f60-113">Get suspiciousIpRiskEvent</span></span>](../api/suspiciousipriskevent-get.md) | [<span data-ttu-id="34f60-114">suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="34f60-114">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) |<span data-ttu-id="34f60-115">Чтение свойства и связи объекта suspiciousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="34f60-115">Read properties and relationships of suspiciousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="34f60-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="34f60-116">Properties</span></span>
| <span data-ttu-id="34f60-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="34f60-117">Property</span></span>     | <span data-ttu-id="34f60-118">Тип</span><span class="sxs-lookup"><span data-stu-id="34f60-118">Type</span></span>   |<span data-ttu-id="34f60-119">Description</span><span class="sxs-lookup"><span data-stu-id="34f60-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34f60-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="34f60-120">closedDateTime</span></span>|<span data-ttu-id="34f60-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34f60-121">dateTimeOffset</span></span>| <span data-ttu-id="34f60-122">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="34f60-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="34f60-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34f60-123">createdDateTime</span></span>|<span data-ttu-id="34f60-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34f60-124">dateTimeOffset</span></span>| <span data-ttu-id="34f60-125">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="34f60-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="34f60-126">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="34f60-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="34f60-127">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="34f60-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="34f60-128">id</span><span class="sxs-lookup"><span data-stu-id="34f60-128">id</span></span>|<span data-ttu-id="34f60-129">строка</span><span class="sxs-lookup"><span data-stu-id="34f60-129">string</span></span>| <span data-ttu-id="34f60-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="34f60-130">Read-only</span></span>|
|<span data-ttu-id="34f60-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="34f60-131">ipAddress</span></span>|<span data-ttu-id="34f60-132">string</span><span class="sxs-lookup"><span data-stu-id="34f60-132">string</span></span>| <span data-ttu-id="34f60-133">IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="34f60-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="34f60-134">location</span><span class="sxs-lookup"><span data-stu-id="34f60-134">location</span></span>|<span data-ttu-id="34f60-135">string</span><span class="sxs-lookup"><span data-stu-id="34f60-135">string</span></span>| <span data-ttu-id="34f60-136">Расположение, подключенного к IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="34f60-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="34f60-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="34f60-137">riskEventDateTime</span></span>|<span data-ttu-id="34f60-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34f60-138">dateTimeOffset</span></span>| <span data-ttu-id="34f60-139">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="34f60-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="34f60-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="34f60-140">riskEventStatus</span></span>|<span data-ttu-id="34f60-141">string</span><span class="sxs-lookup"><span data-stu-id="34f60-141">string</span></span>| <span data-ttu-id="34f60-142">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="34f60-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="34f60-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="34f60-143">riskLevel</span></span>|<span data-ttu-id="34f60-144">string</span><span class="sxs-lookup"><span data-stu-id="34f60-144">string</span></span>| <span data-ttu-id="34f60-145">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="34f60-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="34f60-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="34f60-146">riskEventType</span></span>|<span data-ttu-id="34f60-147">string</span><span class="sxs-lookup"><span data-stu-id="34f60-147">string</span></span>| <span data-ttu-id="34f60-148">Тип риска</span><span class="sxs-lookup"><span data-stu-id="34f60-148">The type of risk</span></span>|
|<span data-ttu-id="34f60-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="34f60-149">userDisplayName</span></span>|<span data-ttu-id="34f60-150">string</span><span class="sxs-lookup"><span data-stu-id="34f60-150">string</span></span>| <span data-ttu-id="34f60-151">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="34f60-151">The name of the user at risk</span></span>|
|<span data-ttu-id="34f60-152">userId</span><span class="sxs-lookup"><span data-stu-id="34f60-152">userId</span></span>|<span data-ttu-id="34f60-153">string</span><span class="sxs-lookup"><span data-stu-id="34f60-153">string</span></span>| <span data-ttu-id="34f60-154">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="34f60-154">The id of the user at risk</span></span>|
|<span data-ttu-id="34f60-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34f60-155">userPrincipalName</span></span>|<span data-ttu-id="34f60-156">string</span><span class="sxs-lookup"><span data-stu-id="34f60-156">string</span></span>| <span data-ttu-id="34f60-157">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="34f60-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="34f60-158">Связи</span><span class="sxs-lookup"><span data-stu-id="34f60-158">Relationships</span></span>
| <span data-ttu-id="34f60-159">Связь</span><span class="sxs-lookup"><span data-stu-id="34f60-159">Relationship</span></span> | <span data-ttu-id="34f60-160">Тип</span><span class="sxs-lookup"><span data-stu-id="34f60-160">Type</span></span>   |<span data-ttu-id="34f60-161">Description</span><span class="sxs-lookup"><span data-stu-id="34f60-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34f60-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="34f60-162">impactedUser</span></span>|[<span data-ttu-id="34f60-163">user</span><span class="sxs-lookup"><span data-stu-id="34f60-163">user</span></span>](user.md)| <span data-ttu-id="34f60-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="34f60-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34f60-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34f60-166">JSON representation</span></span>

<span data-ttu-id="34f60-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34f60-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
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
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->