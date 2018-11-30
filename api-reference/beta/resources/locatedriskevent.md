---
title: Тип ресурса locatedRiskEvent
description: 'Событие риск, обнаруживается Azure Active Directory защиту, основанный на данные о размещении. Типы событий расположены риска:'
ms.openlocfilehash: e84cff5985905977b6b1eeb75a9ef9703a2a2078
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077732"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="c3c92-104">Тип ресурса locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c3c92-104">locatedRiskEvent resource type</span></span>

> <span data-ttu-id="c3c92-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3c92-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3c92-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3c92-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3c92-107">Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , основанный на данные о размещении.</span><span class="sxs-lookup"><span data-stu-id="c3c92-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="c3c92-108">Типы событий расположены риска:</span><span class="sxs-lookup"><span data-stu-id="c3c92-108">Located risk event types include:</span></span>
* [<span data-ttu-id="c3c92-109">войти в систему с анонимным IP-адресов</span><span class="sxs-lookup"><span data-stu-id="c3c92-109">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="c3c92-110">войти в систему с помощью устройств зараженный вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="c3c92-110">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="c3c92-111">Невозможно поездок в необычных расположений</span><span class="sxs-lookup"><span data-stu-id="c3c92-111">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="c3c92-112">войти в систему с подозрительные IP-адресов</span><span class="sxs-lookup"><span data-stu-id="c3c92-112">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="c3c92-113">[войти в систему из незнакомы расположений.](unfamiliarlocationriskevent.md) Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="c3c92-113">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="c3c92-114">Методы</span><span class="sxs-lookup"><span data-stu-id="c3c92-114">Methods</span></span>

| <span data-ttu-id="c3c92-115">Метод</span><span class="sxs-lookup"><span data-stu-id="c3c92-115">Method</span></span>           | <span data-ttu-id="c3c92-116">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c3c92-116">Return Type</span></span>    |<span data-ttu-id="c3c92-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c3c92-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c3c92-118">Получение locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c3c92-118">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="c3c92-119">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="c3c92-119">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="c3c92-120">Чтение свойства и связи объекта locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="c3c92-120">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3c92-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3c92-121">Properties</span></span>
| <span data-ttu-id="c3c92-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3c92-122">Property</span></span>     | <span data-ttu-id="c3c92-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c3c92-123">Type</span></span>   |<span data-ttu-id="c3c92-124">Description</span><span class="sxs-lookup"><span data-stu-id="c3c92-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3c92-125">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3c92-125">closedDateTime</span></span>|<span data-ttu-id="c3c92-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3c92-126">dateTimeOffset</span></span>| <span data-ttu-id="c3c92-127">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="c3c92-127">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="c3c92-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3c92-128">createdDateTime</span></span>|<span data-ttu-id="c3c92-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3c92-129">dateTimeOffset</span></span>| <span data-ttu-id="c3c92-130">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="c3c92-130">The date and time that the risk event was created.</span></span> <span data-ttu-id="c3c92-131">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="c3c92-131">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="c3c92-132">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="c3c92-132">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="c3c92-133">id</span><span class="sxs-lookup"><span data-stu-id="c3c92-133">id</span></span>|<span data-ttu-id="c3c92-134">строка</span><span class="sxs-lookup"><span data-stu-id="c3c92-134">string</span></span>| <span data-ttu-id="c3c92-135">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c3c92-135">Read-only</span></span>|
|<span data-ttu-id="c3c92-136">ipAddress</span><span class="sxs-lookup"><span data-stu-id="c3c92-136">ipAddress</span></span>|<span data-ttu-id="c3c92-137">string</span><span class="sxs-lookup"><span data-stu-id="c3c92-137">string</span></span>| <span data-ttu-id="c3c92-138">IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="c3c92-138">The IP address of the sign-in</span></span>|
|<span data-ttu-id="c3c92-139">location</span><span class="sxs-lookup"><span data-stu-id="c3c92-139">location</span></span>|<span data-ttu-id="c3c92-140">string</span><span class="sxs-lookup"><span data-stu-id="c3c92-140">string</span></span>| <span data-ttu-id="c3c92-141">Расположение, подключенного к IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="c3c92-141">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="c3c92-142">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="c3c92-142">riskEventDateTime</span></span>|<span data-ttu-id="c3c92-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3c92-143">dateTimeOffset</span></span>| <span data-ttu-id="c3c92-144">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="c3c92-144">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="c3c92-145">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="c3c92-145">riskEventStatus</span></span>|<span data-ttu-id="c3c92-146">string</span><span class="sxs-lookup"><span data-stu-id="c3c92-146">string</span></span>| <span data-ttu-id="c3c92-147">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="c3c92-147">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="c3c92-148">riskLevel</span><span class="sxs-lookup"><span data-stu-id="c3c92-148">riskLevel</span></span>|<span data-ttu-id="c3c92-149">string</span><span class="sxs-lookup"><span data-stu-id="c3c92-149">string</span></span>| <span data-ttu-id="c3c92-150">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="c3c92-150">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="c3c92-151">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c3c92-151">riskEventType</span></span>|<span data-ttu-id="c3c92-152">string</span><span class="sxs-lookup"><span data-stu-id="c3c92-152">string</span></span>| <span data-ttu-id="c3c92-153">Тип риска</span><span class="sxs-lookup"><span data-stu-id="c3c92-153">The type of risk</span></span>|
|<span data-ttu-id="c3c92-154">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c3c92-154">userDisplayName</span></span>|<span data-ttu-id="c3c92-155">string</span><span class="sxs-lookup"><span data-stu-id="c3c92-155">string</span></span>| <span data-ttu-id="c3c92-156">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="c3c92-156">The name of the user at risk</span></span>|
|<span data-ttu-id="c3c92-157">userId</span><span class="sxs-lookup"><span data-stu-id="c3c92-157">userId</span></span>|<span data-ttu-id="c3c92-158">string</span><span class="sxs-lookup"><span data-stu-id="c3c92-158">string</span></span>| <span data-ttu-id="c3c92-159">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="c3c92-159">The id of the user at risk</span></span>|
|<span data-ttu-id="c3c92-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c3c92-160">userPrincipalName</span></span>|<span data-ttu-id="c3c92-161">string</span><span class="sxs-lookup"><span data-stu-id="c3c92-161">string</span></span>| <span data-ttu-id="c3c92-162">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="c3c92-162">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3c92-163">Связи</span><span class="sxs-lookup"><span data-stu-id="c3c92-163">Relationships</span></span>
| <span data-ttu-id="c3c92-164">Связь</span><span class="sxs-lookup"><span data-stu-id="c3c92-164">Relationship</span></span> | <span data-ttu-id="c3c92-165">Тип</span><span class="sxs-lookup"><span data-stu-id="c3c92-165">Type</span></span>   |<span data-ttu-id="c3c92-166">Description</span><span class="sxs-lookup"><span data-stu-id="c3c92-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3c92-167">impactedUser</span><span class="sxs-lookup"><span data-stu-id="c3c92-167">impactedUser</span></span>|[<span data-ttu-id="c3c92-168">user</span><span class="sxs-lookup"><span data-stu-id="c3c92-168">user</span></span>](user.md)| <span data-ttu-id="c3c92-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c3c92-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3c92-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3c92-171">JSON representation</span></span>

<span data-ttu-id="c3c92-172">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3c92-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locatedRiskEvent"
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
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->