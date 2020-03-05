---
title: Тип ресурса Локатедрискевент
description: Событие риска, обнаруженное защитой удостоверений Azure Active Directory на основе данных о расположении. К найденным относятся следующие типы событий риска.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b7abb10417e7659e923eddf04990067c8b979ce9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522927"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="12056-104">Тип ресурса Локатедрискевент</span><span class="sxs-lookup"><span data-stu-id="12056-104">locatedRiskEvent resource type</span></span>

<span data-ttu-id="12056-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="12056-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12056-106">Событие риска, обнаруженное [защитой удостоверений Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) на основе данных о расположении.</span><span class="sxs-lookup"><span data-stu-id="12056-106">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="12056-107">К найденным относятся следующие типы событий риска.</span><span class="sxs-lookup"><span data-stu-id="12056-107">Located risk event types include:</span></span>
* [<span data-ttu-id="12056-108">входы с анонимными IP-адресами</span><span class="sxs-lookup"><span data-stu-id="12056-108">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="12056-109">входы с зараженных вредоносными программами устройств</span><span class="sxs-lookup"><span data-stu-id="12056-109">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="12056-110">невозможность перемещаться к необычным расположениям</span><span class="sxs-lookup"><span data-stu-id="12056-110">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="12056-111">входы из подозрительных IP-адресов</span><span class="sxs-lookup"><span data-stu-id="12056-111">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="12056-112">[входы из незнакомых расположений](unfamiliarlocationriskevent.md) Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="12056-112">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="12056-113">Методы</span><span class="sxs-lookup"><span data-stu-id="12056-113">Methods</span></span>

| <span data-ttu-id="12056-114">Метод</span><span class="sxs-lookup"><span data-stu-id="12056-114">Method</span></span>           | <span data-ttu-id="12056-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="12056-115">Return Type</span></span>    |<span data-ttu-id="12056-116">Описание</span><span class="sxs-lookup"><span data-stu-id="12056-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12056-117">Получение Локатедрискевент</span><span class="sxs-lookup"><span data-stu-id="12056-117">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="12056-118">локатедрискевент</span><span class="sxs-lookup"><span data-stu-id="12056-118">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="12056-119">Чтение свойств и связей объекта Локатедрискевент.</span><span class="sxs-lookup"><span data-stu-id="12056-119">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="12056-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="12056-120">Properties</span></span>
| <span data-ttu-id="12056-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="12056-121">Property</span></span>     | <span data-ttu-id="12056-122">Тип</span><span class="sxs-lookup"><span data-stu-id="12056-122">Type</span></span>   |<span data-ttu-id="12056-123">Описание</span><span class="sxs-lookup"><span data-stu-id="12056-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12056-124">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="12056-124">closedDateTime</span></span>|<span data-ttu-id="12056-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12056-125">dateTimeOffset</span></span>| <span data-ttu-id="12056-126">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="12056-126">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="12056-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12056-127">createdDateTime</span></span>|<span data-ttu-id="12056-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12056-128">dateTimeOffset</span></span>| <span data-ttu-id="12056-129">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="12056-129">The date and time that the risk event was created.</span></span> <span data-ttu-id="12056-130">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="12056-130">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="12056-131">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="12056-131">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="12056-132">id</span><span class="sxs-lookup"><span data-stu-id="12056-132">id</span></span>|<span data-ttu-id="12056-133">string</span><span class="sxs-lookup"><span data-stu-id="12056-133">string</span></span>| <span data-ttu-id="12056-134">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="12056-134">Read-only</span></span>|
|<span data-ttu-id="12056-135">ipAddress</span><span class="sxs-lookup"><span data-stu-id="12056-135">ipAddress</span></span>|<span data-ttu-id="12056-136">строка</span><span class="sxs-lookup"><span data-stu-id="12056-136">string</span></span>| <span data-ttu-id="12056-137">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="12056-137">The IP address of the sign-in</span></span>|
|<span data-ttu-id="12056-138">location</span><span class="sxs-lookup"><span data-stu-id="12056-138">location</span></span>|<span data-ttu-id="12056-139">строка</span><span class="sxs-lookup"><span data-stu-id="12056-139">string</span></span>| <span data-ttu-id="12056-140">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="12056-140">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="12056-141">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="12056-141">riskEventDateTime</span></span>|<span data-ttu-id="12056-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12056-142">dateTimeOffset</span></span>| <span data-ttu-id="12056-143">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="12056-143">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="12056-144">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="12056-144">riskEventStatus</span></span>|<span data-ttu-id="12056-145">строка</span><span class="sxs-lookup"><span data-stu-id="12056-145">string</span></span>| <span data-ttu-id="12056-146">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="12056-146">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="12056-147">riskLevel</span><span class="sxs-lookup"><span data-stu-id="12056-147">riskLevel</span></span>|<span data-ttu-id="12056-148">string</span><span class="sxs-lookup"><span data-stu-id="12056-148">string</span></span>| <span data-ttu-id="12056-149">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="12056-149">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="12056-150">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="12056-150">riskEventType</span></span>|<span data-ttu-id="12056-151">строка</span><span class="sxs-lookup"><span data-stu-id="12056-151">string</span></span>| <span data-ttu-id="12056-152">Тип риска</span><span class="sxs-lookup"><span data-stu-id="12056-152">The type of risk</span></span>|
|<span data-ttu-id="12056-153">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="12056-153">userDisplayName</span></span>|<span data-ttu-id="12056-154">строка</span><span class="sxs-lookup"><span data-stu-id="12056-154">string</span></span>| <span data-ttu-id="12056-155">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="12056-155">The name of the user at risk</span></span>|
|<span data-ttu-id="12056-156">userId</span><span class="sxs-lookup"><span data-stu-id="12056-156">userId</span></span>|<span data-ttu-id="12056-157">строка</span><span class="sxs-lookup"><span data-stu-id="12056-157">string</span></span>| <span data-ttu-id="12056-158">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="12056-158">The id of the user at risk</span></span>|
|<span data-ttu-id="12056-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="12056-159">userPrincipalName</span></span>|<span data-ttu-id="12056-160">string</span><span class="sxs-lookup"><span data-stu-id="12056-160">string</span></span>| <span data-ttu-id="12056-161">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="12056-161">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="12056-162">Связи</span><span class="sxs-lookup"><span data-stu-id="12056-162">Relationships</span></span>
| <span data-ttu-id="12056-163">Связь</span><span class="sxs-lookup"><span data-stu-id="12056-163">Relationship</span></span> | <span data-ttu-id="12056-164">Тип</span><span class="sxs-lookup"><span data-stu-id="12056-164">Type</span></span>   |<span data-ttu-id="12056-165">Описание</span><span class="sxs-lookup"><span data-stu-id="12056-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12056-166">импактедусер</span><span class="sxs-lookup"><span data-stu-id="12056-166">impactedUser</span></span>|[<span data-ttu-id="12056-167">user</span><span class="sxs-lookup"><span data-stu-id="12056-167">user</span></span>](user.md)| <span data-ttu-id="12056-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="12056-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12056-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12056-170">JSON representation</span></span>

<span data-ttu-id="12056-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="12056-171">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "abstract": true,
   "keyProperty": "id",
   "baseType":"microsoft.graph.identityRiskEvent",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
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
  "suppressions": []
}
-->
