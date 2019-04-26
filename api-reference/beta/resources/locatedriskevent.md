---
title: Тип ресурса Локатедрискевент
description: Событие риска, обнаруженное защитой удостоверений Azure Active Directory на основе данных о расположении. К найденным относятся следующие типы событий риска.
localization_priority: Normal
ms.openlocfilehash: 2c7503c08700a0d7c2d2ad67e8868901bdb008e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345377"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="79b21-104">Тип ресурса Локатедрискевент</span><span class="sxs-lookup"><span data-stu-id="79b21-104">locatedRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79b21-105">Событие риска, обнаруженное [защитОй удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) на основе данных о расположении.</span><span class="sxs-lookup"><span data-stu-id="79b21-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) that is based on location data.</span></span> <span data-ttu-id="79b21-106">К найденным относятся следующие типы событий риска.</span><span class="sxs-lookup"><span data-stu-id="79b21-106">Located risk event types include:</span></span>
* [<span data-ttu-id="79b21-107">входы с анонимными IP-адресами</span><span class="sxs-lookup"><span data-stu-id="79b21-107">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="79b21-108">входы с зараженных вредоносными программами устройств</span><span class="sxs-lookup"><span data-stu-id="79b21-108">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="79b21-109">невозможность перемещаться к необычным расположениям</span><span class="sxs-lookup"><span data-stu-id="79b21-109">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="79b21-110">входы из подозрительных IP-адресов</span><span class="sxs-lookup"><span data-stu-id="79b21-110">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="79b21-111">[входы из](unfamiliarlocationriskevent.md) незнакомых расположений Полную информацию о событиях риска можно найти в [документации по защите удостоверенИй Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="79b21-111">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="79b21-112">Методы</span><span class="sxs-lookup"><span data-stu-id="79b21-112">Methods</span></span>

| <span data-ttu-id="79b21-113">Метод</span><span class="sxs-lookup"><span data-stu-id="79b21-113">Method</span></span>           | <span data-ttu-id="79b21-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="79b21-114">Return Type</span></span>    |<span data-ttu-id="79b21-115">Описание</span><span class="sxs-lookup"><span data-stu-id="79b21-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79b21-116">Получение Локатедрискевент</span><span class="sxs-lookup"><span data-stu-id="79b21-116">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="79b21-117">Локатедрискевент</span><span class="sxs-lookup"><span data-stu-id="79b21-117">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="79b21-118">Чтение свойств и связей объекта Локатедрискевент.</span><span class="sxs-lookup"><span data-stu-id="79b21-118">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="79b21-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="79b21-119">Properties</span></span>
| <span data-ttu-id="79b21-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="79b21-120">Property</span></span>     | <span data-ttu-id="79b21-121">Тип</span><span class="sxs-lookup"><span data-stu-id="79b21-121">Type</span></span>   |<span data-ttu-id="79b21-122">Описание</span><span class="sxs-lookup"><span data-stu-id="79b21-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79b21-123">Клоседдатетиме</span><span class="sxs-lookup"><span data-stu-id="79b21-123">closedDateTime</span></span>|<span data-ttu-id="79b21-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79b21-124">dateTimeOffset</span></span>| <span data-ttu-id="79b21-125">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="79b21-125">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="79b21-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79b21-126">createdDateTime</span></span>|<span data-ttu-id="79b21-127">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79b21-127">dateTimeOffset</span></span>| <span data-ttu-id="79b21-128">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="79b21-128">The date and time that the risk event was created.</span></span> <span data-ttu-id="79b21-129">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="79b21-129">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="79b21-130">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="79b21-130">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="79b21-131">id</span><span class="sxs-lookup"><span data-stu-id="79b21-131">id</span></span>|<span data-ttu-id="79b21-132">строка</span><span class="sxs-lookup"><span data-stu-id="79b21-132">string</span></span>| <span data-ttu-id="79b21-133">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="79b21-133">Read-only</span></span>|
|<span data-ttu-id="79b21-134">ipAddress</span><span class="sxs-lookup"><span data-stu-id="79b21-134">ipAddress</span></span>|<span data-ttu-id="79b21-135">строка</span><span class="sxs-lookup"><span data-stu-id="79b21-135">string</span></span>| <span data-ttu-id="79b21-136">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="79b21-136">The IP address of the sign-in</span></span>|
|<span data-ttu-id="79b21-137">location</span><span class="sxs-lookup"><span data-stu-id="79b21-137">location</span></span>|<span data-ttu-id="79b21-138">строка</span><span class="sxs-lookup"><span data-stu-id="79b21-138">string</span></span>| <span data-ttu-id="79b21-139">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="79b21-139">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="79b21-140">Рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="79b21-140">riskEventDateTime</span></span>|<span data-ttu-id="79b21-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79b21-141">dateTimeOffset</span></span>| <span data-ttu-id="79b21-142">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="79b21-142">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="79b21-143">Рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="79b21-143">riskEventStatus</span></span>|<span data-ttu-id="79b21-144">строка</span><span class="sxs-lookup"><span data-stu-id="79b21-144">string</span></span>| <span data-ttu-id="79b21-145">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="79b21-145">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="79b21-146">riskLevel</span><span class="sxs-lookup"><span data-stu-id="79b21-146">riskLevel</span></span>|<span data-ttu-id="79b21-147">string</span><span class="sxs-lookup"><span data-stu-id="79b21-147">string</span></span>| <span data-ttu-id="79b21-148">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="79b21-148">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="79b21-149">Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="79b21-149">riskEventType</span></span>|<span data-ttu-id="79b21-150">строка</span><span class="sxs-lookup"><span data-stu-id="79b21-150">string</span></span>| <span data-ttu-id="79b21-151">Тип риска</span><span class="sxs-lookup"><span data-stu-id="79b21-151">The type of risk</span></span>|
|<span data-ttu-id="79b21-152">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="79b21-152">userDisplayName</span></span>|<span data-ttu-id="79b21-153">строка</span><span class="sxs-lookup"><span data-stu-id="79b21-153">string</span></span>| <span data-ttu-id="79b21-154">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="79b21-154">The name of the user at risk</span></span>|
|<span data-ttu-id="79b21-155">userId</span><span class="sxs-lookup"><span data-stu-id="79b21-155">userId</span></span>|<span data-ttu-id="79b21-156">строка</span><span class="sxs-lookup"><span data-stu-id="79b21-156">string</span></span>| <span data-ttu-id="79b21-157">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="79b21-157">The id of the user at risk</span></span>|
|<span data-ttu-id="79b21-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="79b21-158">userPrincipalName</span></span>|<span data-ttu-id="79b21-159">string</span><span class="sxs-lookup"><span data-stu-id="79b21-159">string</span></span>| <span data-ttu-id="79b21-160">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="79b21-160">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="79b21-161">Связи</span><span class="sxs-lookup"><span data-stu-id="79b21-161">Relationships</span></span>
| <span data-ttu-id="79b21-162">Отношение</span><span class="sxs-lookup"><span data-stu-id="79b21-162">Relationship</span></span> | <span data-ttu-id="79b21-163">Тип</span><span class="sxs-lookup"><span data-stu-id="79b21-163">Type</span></span>   |<span data-ttu-id="79b21-164">Описание</span><span class="sxs-lookup"><span data-stu-id="79b21-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79b21-165">Импактедусер</span><span class="sxs-lookup"><span data-stu-id="79b21-165">impactedUser</span></span>|[<span data-ttu-id="79b21-166">user</span><span class="sxs-lookup"><span data-stu-id="79b21-166">user</span></span>](user.md)| <span data-ttu-id="79b21-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="79b21-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79b21-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79b21-169">JSON representation</span></span>

<span data-ttu-id="79b21-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79b21-170">Here is a JSON representation of the resource.</span></span>

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
