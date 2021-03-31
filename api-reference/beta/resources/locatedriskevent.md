---
title: тип ресурса locatedRiskEvent
description: 'Событие риска, обнаруженное Azure Active Directory Identity Protection, основанное на данных расположения. Типы событий, связанных с расположенными рисками, включают:'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 902dc864ea16bd677d0499711faa078131ca015d
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469460"
---
# <a name="locatedriskevent-resource-type"></a><span data-ttu-id="830bc-104">тип ресурса locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="830bc-104">locatedRiskEvent resource type</span></span>

<span data-ttu-id="830bc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="830bc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="830bc-106">Событие риска, обнаруженное [Azure Active Directory Identity Protection,](/azure/active-directory/identity-protection/overview-identity-protection) основанное на данных расположения.</span><span class="sxs-lookup"><span data-stu-id="830bc-106">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) that is based on location data.</span></span> <span data-ttu-id="830bc-107">Типы событий, связанных с расположенными рисками, включают:</span><span class="sxs-lookup"><span data-stu-id="830bc-107">Located risk event types include:</span></span>
* [<span data-ttu-id="830bc-108">входы с анонимных IP-адресов</span><span class="sxs-lookup"><span data-stu-id="830bc-108">sign-ins from anonymous IP addresses</span></span>](anonymousipriskevent.md)
* [<span data-ttu-id="830bc-109">входы с устройств, зараженных вредоносными программами</span><span class="sxs-lookup"><span data-stu-id="830bc-109">sign-ins from malware-infected devices</span></span>](malwareriskevent.md)
* [<span data-ttu-id="830bc-110">невозможное путешествие в нетипичные расположения</span><span class="sxs-lookup"><span data-stu-id="830bc-110">impossible travel to atypical locations</span></span>](impossibletravelriskevent.md)
* [<span data-ttu-id="830bc-111">входы с подозрительных IP-адресов</span><span class="sxs-lookup"><span data-stu-id="830bc-111">sign-ins from suspicious IP addresses</span></span>](suspiciousipriskevent.md)
* <span data-ttu-id="830bc-112">[входы из незнакомых мест](unfamiliarlocationriskevent.md) Полные сведения о событиях риска можно найти в документации [azure AD Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="830bc-112">[sign-ins from unfamiliar locations](unfamiliarlocationriskevent.md) Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="830bc-113">Методы</span><span class="sxs-lookup"><span data-stu-id="830bc-113">Methods</span></span>

| <span data-ttu-id="830bc-114">Метод</span><span class="sxs-lookup"><span data-stu-id="830bc-114">Method</span></span>           | <span data-ttu-id="830bc-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="830bc-115">Return Type</span></span>    |<span data-ttu-id="830bc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="830bc-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="830bc-117">Get locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="830bc-117">Get locatedRiskEvent</span></span>](../api/locatedriskevent-get.md) | [<span data-ttu-id="830bc-118">locatedRiskEvent</span><span class="sxs-lookup"><span data-stu-id="830bc-118">locatedRiskEvent</span></span>](locatedriskevent.md) |<span data-ttu-id="830bc-119">Чтение свойств и связей объекта locatedRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="830bc-119">Read properties and relationships of locatedRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="830bc-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="830bc-120">Properties</span></span>
| <span data-ttu-id="830bc-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="830bc-121">Property</span></span>     | <span data-ttu-id="830bc-122">Тип</span><span class="sxs-lookup"><span data-stu-id="830bc-122">Type</span></span>   |<span data-ttu-id="830bc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="830bc-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="830bc-124">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="830bc-124">closedDateTime</span></span>|<span data-ttu-id="830bc-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="830bc-125">dateTimeOffset</span></span>| <span data-ttu-id="830bc-126">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="830bc-126">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="830bc-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="830bc-127">createdDateTime</span></span>|<span data-ttu-id="830bc-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="830bc-128">dateTimeOffset</span></span>| <span data-ttu-id="830bc-129">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="830bc-129">The date and time that the risk event was created.</span></span> <span data-ttu-id="830bc-130">Это всегда больше или равно дате самого события риска.</span><span class="sxs-lookup"><span data-stu-id="830bc-130">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="830bc-131">Это правильное свойство, используемее в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="830bc-131">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="830bc-132">id</span><span class="sxs-lookup"><span data-stu-id="830bc-132">id</span></span>|<span data-ttu-id="830bc-133">string</span><span class="sxs-lookup"><span data-stu-id="830bc-133">string</span></span>| <span data-ttu-id="830bc-134">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="830bc-134">Read-only</span></span>|
|<span data-ttu-id="830bc-135">ipAddress</span><span class="sxs-lookup"><span data-stu-id="830bc-135">ipAddress</span></span>|<span data-ttu-id="830bc-136">Строка</span><span class="sxs-lookup"><span data-stu-id="830bc-136">string</span></span>| <span data-ttu-id="830bc-137">IP-адрес входного</span><span class="sxs-lookup"><span data-stu-id="830bc-137">The IP address of the sign-in</span></span>|
|<span data-ttu-id="830bc-138">location</span><span class="sxs-lookup"><span data-stu-id="830bc-138">location</span></span>|<span data-ttu-id="830bc-139">string</span><span class="sxs-lookup"><span data-stu-id="830bc-139">string</span></span>| <span data-ttu-id="830bc-140">Расположение, прикрепленное к IP-адресу входного</span><span class="sxs-lookup"><span data-stu-id="830bc-140">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="830bc-141">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="830bc-141">riskEventDateTime</span></span>|<span data-ttu-id="830bc-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="830bc-142">dateTimeOffset</span></span>| <span data-ttu-id="830bc-143">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="830bc-143">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="830bc-144">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="830bc-144">riskEventStatus</span></span>|<span data-ttu-id="830bc-145">Строка</span><span class="sxs-lookup"><span data-stu-id="830bc-145">string</span></span>| <span data-ttu-id="830bc-146">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="830bc-146">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="830bc-147">riskLevel</span><span class="sxs-lookup"><span data-stu-id="830bc-147">riskLevel</span></span>|<span data-ttu-id="830bc-148">string</span><span class="sxs-lookup"><span data-stu-id="830bc-148">string</span></span>| <span data-ttu-id="830bc-149">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="830bc-149">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="830bc-150">riskEventType</span><span class="sxs-lookup"><span data-stu-id="830bc-150">riskEventType</span></span>|<span data-ttu-id="830bc-151">Строка</span><span class="sxs-lookup"><span data-stu-id="830bc-151">string</span></span>| <span data-ttu-id="830bc-152">Тип риска</span><span class="sxs-lookup"><span data-stu-id="830bc-152">The type of risk</span></span>|
|<span data-ttu-id="830bc-153">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="830bc-153">userDisplayName</span></span>|<span data-ttu-id="830bc-154">Строка</span><span class="sxs-lookup"><span data-stu-id="830bc-154">string</span></span>| <span data-ttu-id="830bc-155">Имя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="830bc-155">The name of the user at risk</span></span>|
|<span data-ttu-id="830bc-156">userId</span><span class="sxs-lookup"><span data-stu-id="830bc-156">userId</span></span>|<span data-ttu-id="830bc-157">строка</span><span class="sxs-lookup"><span data-stu-id="830bc-157">string</span></span>| <span data-ttu-id="830bc-158">ID пользователя, на который существует риск</span><span class="sxs-lookup"><span data-stu-id="830bc-158">The id of the user at risk</span></span>|
|<span data-ttu-id="830bc-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="830bc-159">userPrincipalName</span></span>|<span data-ttu-id="830bc-160">string</span><span class="sxs-lookup"><span data-stu-id="830bc-160">string</span></span>| <span data-ttu-id="830bc-161">Основное имя пользователя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="830bc-161">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="830bc-162">Связи</span><span class="sxs-lookup"><span data-stu-id="830bc-162">Relationships</span></span>
| <span data-ttu-id="830bc-163">Связь</span><span class="sxs-lookup"><span data-stu-id="830bc-163">Relationship</span></span> | <span data-ttu-id="830bc-164">Тип</span><span class="sxs-lookup"><span data-stu-id="830bc-164">Type</span></span>   |<span data-ttu-id="830bc-165">Описание</span><span class="sxs-lookup"><span data-stu-id="830bc-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="830bc-166">impactedUser</span><span class="sxs-lookup"><span data-stu-id="830bc-166">impactedUser</span></span>|[<span data-ttu-id="830bc-167">user</span><span class="sxs-lookup"><span data-stu-id="830bc-167">user</span></span>](user.md)| <span data-ttu-id="830bc-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="830bc-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="830bc-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="830bc-170">JSON representation</span></span>

<span data-ttu-id="830bc-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="830bc-171">Here is a JSON representation of the resource.</span></span>

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