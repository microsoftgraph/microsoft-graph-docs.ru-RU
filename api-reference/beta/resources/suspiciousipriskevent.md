---
title: Тип ресурса СуспиЦиаусиприскевент
description: Событие риска, обнаруженное при попытке входа учетной записи с подозрительным IP-адресом с помощью средства защиты удостоверений Azure Active Directory. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a774c94d8e4ade2067e3aa784c42bee5db6ee3b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008049"
---
# <a name="suspiciousipriskevent-resource-type"></a><span data-ttu-id="1b405-104">Тип ресурса СуспиЦиаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="1b405-104">suspiciousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b405-105">Событие риска, обнаруженное при попытке входа учетной записи с подозрительным IP-адресом с помощью средства [защиты удостоверений Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) .</span><span class="sxs-lookup"><span data-stu-id="1b405-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a suspicious IP address.</span></span> <span data-ttu-id="1b405-106">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="1b405-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="1b405-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1b405-107">Methods</span></span>

| <span data-ttu-id="1b405-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1b405-108">Method</span></span>           | <span data-ttu-id="1b405-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1b405-109">Return Type</span></span>    |<span data-ttu-id="1b405-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1b405-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b405-111">Получение объекта suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1b405-111">Get suspiciousIpRiskEvent</span></span>](../api/suspiciousipriskevent-get.md) | [<span data-ttu-id="1b405-112">СуспиЦиаусиприскевент</span><span class="sxs-lookup"><span data-stu-id="1b405-112">suspiciousIpRiskEvent</span></span>](suspiciousipriskevent.md) |<span data-ttu-id="1b405-113">Чтение свойств и связей объекта СуспиЦиаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="1b405-113">Read properties and relationships of suspiciousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b405-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b405-114">Properties</span></span>
| <span data-ttu-id="1b405-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b405-115">Property</span></span>     | <span data-ttu-id="1b405-116">Тип</span><span class="sxs-lookup"><span data-stu-id="1b405-116">Type</span></span>   |<span data-ttu-id="1b405-117">Описание</span><span class="sxs-lookup"><span data-stu-id="1b405-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b405-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b405-118">closedDateTime</span></span>|<span data-ttu-id="1b405-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b405-119">dateTimeOffset</span></span>| <span data-ttu-id="1b405-120">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="1b405-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="1b405-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b405-121">createdDateTime</span></span>|<span data-ttu-id="1b405-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b405-122">dateTimeOffset</span></span>| <span data-ttu-id="1b405-123">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="1b405-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="1b405-124">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="1b405-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="1b405-125">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="1b405-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="1b405-126">id</span><span class="sxs-lookup"><span data-stu-id="1b405-126">id</span></span>|<span data-ttu-id="1b405-127">string</span><span class="sxs-lookup"><span data-stu-id="1b405-127">string</span></span>| <span data-ttu-id="1b405-128">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="1b405-128">Read-only</span></span>|
|<span data-ttu-id="1b405-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1b405-129">ipAddress</span></span>|<span data-ttu-id="1b405-130">string</span><span class="sxs-lookup"><span data-stu-id="1b405-130">string</span></span>| <span data-ttu-id="1b405-131">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="1b405-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="1b405-132">location</span><span class="sxs-lookup"><span data-stu-id="1b405-132">location</span></span>|<span data-ttu-id="1b405-133">string</span><span class="sxs-lookup"><span data-stu-id="1b405-133">string</span></span>| <span data-ttu-id="1b405-134">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="1b405-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="1b405-135">Рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="1b405-135">riskEventDateTime</span></span>|<span data-ttu-id="1b405-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b405-136">dateTimeOffset</span></span>| <span data-ttu-id="1b405-137">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="1b405-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="1b405-138">Рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="1b405-138">riskEventStatus</span></span>|<span data-ttu-id="1b405-139">string</span><span class="sxs-lookup"><span data-stu-id="1b405-139">string</span></span>| <span data-ttu-id="1b405-140">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="1b405-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="1b405-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="1b405-141">riskLevel</span></span>|<span data-ttu-id="1b405-142">string</span><span class="sxs-lookup"><span data-stu-id="1b405-142">string</span></span>| <span data-ttu-id="1b405-143">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="1b405-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="1b405-144">Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="1b405-144">riskEventType</span></span>|<span data-ttu-id="1b405-145">string</span><span class="sxs-lookup"><span data-stu-id="1b405-145">string</span></span>| <span data-ttu-id="1b405-146">Тип риска</span><span class="sxs-lookup"><span data-stu-id="1b405-146">The type of risk</span></span>|
|<span data-ttu-id="1b405-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1b405-147">userDisplayName</span></span>|<span data-ttu-id="1b405-148">string</span><span class="sxs-lookup"><span data-stu-id="1b405-148">string</span></span>| <span data-ttu-id="1b405-149">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="1b405-149">The name of the user at risk</span></span>|
|<span data-ttu-id="1b405-150">userId</span><span class="sxs-lookup"><span data-stu-id="1b405-150">userId</span></span>|<span data-ttu-id="1b405-151">string</span><span class="sxs-lookup"><span data-stu-id="1b405-151">string</span></span>| <span data-ttu-id="1b405-152">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="1b405-152">The id of the user at risk</span></span>|
|<span data-ttu-id="1b405-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1b405-153">userPrincipalName</span></span>|<span data-ttu-id="1b405-154">string</span><span class="sxs-lookup"><span data-stu-id="1b405-154">string</span></span>| <span data-ttu-id="1b405-155">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="1b405-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b405-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="1b405-156">Relationships</span></span>
| <span data-ttu-id="1b405-157">Отношение</span><span class="sxs-lookup"><span data-stu-id="1b405-157">Relationship</span></span> | <span data-ttu-id="1b405-158">Тип</span><span class="sxs-lookup"><span data-stu-id="1b405-158">Type</span></span>   |<span data-ttu-id="1b405-159">Описание</span><span class="sxs-lookup"><span data-stu-id="1b405-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b405-160">Импактедусер</span><span class="sxs-lookup"><span data-stu-id="1b405-160">impactedUser</span></span>|[<span data-ttu-id="1b405-161">user</span><span class="sxs-lookup"><span data-stu-id="1b405-161">user</span></span>](user.md)| <span data-ttu-id="1b405-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1b405-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b405-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b405-164">JSON representation</span></span>

<span data-ttu-id="1b405-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b405-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "suspiciousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
