---
title: Тип ресурса locatedRiskEvent
description: 'Событие риск, обнаруживается Azure Active Directory защиту, основанный на данные о размещении. Типы событий расположены риска:'
localization_priority: Normal
ms.openlocfilehash: 20fe76099c511483144b42e33fc260910debb5ed
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510262"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="674ae-104">Тип ресурса locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="674ae-104">locatedRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="674ae-105">Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , основанный на данные о размещении.</span><span class="sxs-lookup"><span data-stu-id="674ae-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="674ae-106">Типы событий расположены риска:</span><span class="sxs-lookup"><span data-stu-id="674ae-106">Located risk event types include:</span></span>
* [<span data-ttu-id="674ae-107">войти в систему с анонимным IP-адресов</span><span class="sxs-lookup"><span data-stu-id="674ae-107">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="674ae-108">войти в систему с помощью устройств зараженный вредоносных программ</span><span class="sxs-lookup"><span data-stu-id="674ae-108">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="674ae-109">Невозможно поездок в необычных расположений</span><span class="sxs-lookup"><span data-stu-id="674ae-109">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="674ae-110">войти в систему с подозрительные IP-адресов</span><span class="sxs-lookup"><span data-stu-id="674ae-110">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="674ae-111">[войти в систему из незнакомы расположений.](unfamiliarlocationriskevent.md) Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="674ae-111">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="674ae-112">Методы</span><span class="sxs-lookup"><span data-stu-id="674ae-112">Methods</span></span>

| <span data-ttu-id="674ae-113">Метод</span><span class="sxs-lookup"><span data-stu-id="674ae-113">Method</span></span>           | <span data-ttu-id="674ae-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="674ae-114">Return Type</span></span>    |<span data-ttu-id="674ae-115">Описание</span><span class="sxs-lookup"><span data-stu-id="674ae-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="674ae-116">Получение locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="674ae-116">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="674ae-117">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="674ae-117">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="674ae-118">Чтение свойства и связи объекта locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="674ae-118">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="674ae-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="674ae-119">Properties</span></span>
| <span data-ttu-id="674ae-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="674ae-120">Property</span></span>     | <span data-ttu-id="674ae-121">Тип</span><span class="sxs-lookup"><span data-stu-id="674ae-121">Type</span></span>   |<span data-ttu-id="674ae-122">Описание</span><span class="sxs-lookup"><span data-stu-id="674ae-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="674ae-123">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="674ae-123">closedDateTime</span></span>|<span data-ttu-id="674ae-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="674ae-124">dateTimeOffset</span></span>| <span data-ttu-id="674ae-125">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="674ae-125">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="674ae-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="674ae-126">createdDateTime</span></span>|<span data-ttu-id="674ae-127">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="674ae-127">dateTimeOffset</span></span>| <span data-ttu-id="674ae-128">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="674ae-128">The date and time that the risk event was created.</span></span> <span data-ttu-id="674ae-129">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="674ae-129">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="674ae-130">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="674ae-130">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="674ae-131">id</span><span class="sxs-lookup"><span data-stu-id="674ae-131">id</span></span>|<span data-ttu-id="674ae-132">string</span><span class="sxs-lookup"><span data-stu-id="674ae-132">string</span></span>| <span data-ttu-id="674ae-133">Только чтение</span><span class="sxs-lookup"><span data-stu-id="674ae-133">Read-only</span></span>|
|<span data-ttu-id="674ae-134">ipAddress</span><span class="sxs-lookup"><span data-stu-id="674ae-134">ipAddress</span></span>|<span data-ttu-id="674ae-135">string</span><span class="sxs-lookup"><span data-stu-id="674ae-135">string</span></span>| <span data-ttu-id="674ae-136">IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="674ae-136">The IP address of the sign-in</span></span>|
|<span data-ttu-id="674ae-137">location</span><span class="sxs-lookup"><span data-stu-id="674ae-137">location</span></span>|<span data-ttu-id="674ae-138">string</span><span class="sxs-lookup"><span data-stu-id="674ae-138">string</span></span>| <span data-ttu-id="674ae-139">Расположение, подключенного к IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="674ae-139">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="674ae-140">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="674ae-140">riskEventDateTime</span></span>|<span data-ttu-id="674ae-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="674ae-141">dateTimeOffset</span></span>| <span data-ttu-id="674ae-142">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="674ae-142">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="674ae-143">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="674ae-143">riskEventStatus</span></span>|<span data-ttu-id="674ae-144">string</span><span class="sxs-lookup"><span data-stu-id="674ae-144">string</span></span>| <span data-ttu-id="674ae-145">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="674ae-145">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="674ae-146">riskLevel</span><span class="sxs-lookup"><span data-stu-id="674ae-146">riskLevel</span></span>|<span data-ttu-id="674ae-147">string</span><span class="sxs-lookup"><span data-stu-id="674ae-147">string</span></span>| <span data-ttu-id="674ae-148">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="674ae-148">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="674ae-149">riskEventType</span><span class="sxs-lookup"><span data-stu-id="674ae-149">riskEventType</span></span>|<span data-ttu-id="674ae-150">string</span><span class="sxs-lookup"><span data-stu-id="674ae-150">string</span></span>| <span data-ttu-id="674ae-151">Тип риска</span><span class="sxs-lookup"><span data-stu-id="674ae-151">The type of risk</span></span>|
|<span data-ttu-id="674ae-152">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="674ae-152">userDisplayName</span></span>|<span data-ttu-id="674ae-153">string</span><span class="sxs-lookup"><span data-stu-id="674ae-153">string</span></span>| <span data-ttu-id="674ae-154">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="674ae-154">The name of the user at risk</span></span>|
|<span data-ttu-id="674ae-155">userId</span><span class="sxs-lookup"><span data-stu-id="674ae-155">userId</span></span>|<span data-ttu-id="674ae-156">string</span><span class="sxs-lookup"><span data-stu-id="674ae-156">string</span></span>| <span data-ttu-id="674ae-157">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="674ae-157">The id of the user at risk</span></span>|
|<span data-ttu-id="674ae-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="674ae-158">userPrincipalName</span></span>|<span data-ttu-id="674ae-159">string</span><span class="sxs-lookup"><span data-stu-id="674ae-159">string</span></span>| <span data-ttu-id="674ae-160">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="674ae-160">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="674ae-161">Отношения</span><span class="sxs-lookup"><span data-stu-id="674ae-161">Relationships</span></span>
| <span data-ttu-id="674ae-162">Связь</span><span class="sxs-lookup"><span data-stu-id="674ae-162">Relationship</span></span> | <span data-ttu-id="674ae-163">Тип</span><span class="sxs-lookup"><span data-stu-id="674ae-163">Type</span></span>   |<span data-ttu-id="674ae-164">Описание</span><span class="sxs-lookup"><span data-stu-id="674ae-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="674ae-165">impactedUser</span><span class="sxs-lookup"><span data-stu-id="674ae-165">impactedUser</span></span>|[<span data-ttu-id="674ae-166">user</span><span class="sxs-lookup"><span data-stu-id="674ae-166">user</span></span>](user.md)| <span data-ttu-id="674ae-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="674ae-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="674ae-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="674ae-169">JSON representation</span></span>

<span data-ttu-id="674ae-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="674ae-170">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locatedriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
