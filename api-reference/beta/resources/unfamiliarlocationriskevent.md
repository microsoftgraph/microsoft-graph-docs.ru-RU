---
title: Тип ресурса Унфамилиарлокатионрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором выполняется попытка входа учетной записи из нового расположения для этого пользователя. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 106310a0ed0f3294842fbe7e2afd29e1d906cdec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007559"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="3de75-104">Тип ресурса Унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="3de75-104">unfamiliarLocationRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3de75-105">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , в котором выполняется попытка входа учетной записи из нового расположения для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="3de75-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="3de75-106">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="3de75-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="3de75-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3de75-107">Methods</span></span>

| <span data-ttu-id="3de75-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3de75-108">Method</span></span>           | <span data-ttu-id="3de75-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3de75-109">Return Type</span></span>    |<span data-ttu-id="3de75-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3de75-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3de75-111">Получение объекта unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="3de75-111">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="3de75-112">Унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="3de75-112">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="3de75-113">Чтение свойств и связей объекта Унфамилиарлокатионрискевент.</span><span class="sxs-lookup"><span data-stu-id="3de75-113">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3de75-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="3de75-114">Properties</span></span>
| <span data-ttu-id="3de75-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="3de75-115">Property</span></span>     | <span data-ttu-id="3de75-116">Тип</span><span class="sxs-lookup"><span data-stu-id="3de75-116">Type</span></span>   |<span data-ttu-id="3de75-117">Описание</span><span class="sxs-lookup"><span data-stu-id="3de75-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3de75-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="3de75-118">closedDateTime</span></span>|<span data-ttu-id="3de75-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de75-119">dateTimeOffset</span></span>| <span data-ttu-id="3de75-120">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="3de75-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="3de75-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3de75-121">createdDateTime</span></span>|<span data-ttu-id="3de75-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de75-122">dateTimeOffset</span></span>| <span data-ttu-id="3de75-123">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="3de75-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="3de75-124">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="3de75-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="3de75-125">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="3de75-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="3de75-126">id</span><span class="sxs-lookup"><span data-stu-id="3de75-126">id</span></span>|<span data-ttu-id="3de75-127">string</span><span class="sxs-lookup"><span data-stu-id="3de75-127">string</span></span>| <span data-ttu-id="3de75-128">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="3de75-128">Read-only</span></span>|
|<span data-ttu-id="3de75-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3de75-129">ipAddress</span></span>|<span data-ttu-id="3de75-130">string</span><span class="sxs-lookup"><span data-stu-id="3de75-130">string</span></span>| <span data-ttu-id="3de75-131">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="3de75-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="3de75-132">location</span><span class="sxs-lookup"><span data-stu-id="3de75-132">location</span></span>|<span data-ttu-id="3de75-133">string</span><span class="sxs-lookup"><span data-stu-id="3de75-133">string</span></span>| <span data-ttu-id="3de75-134">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="3de75-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="3de75-135">Рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="3de75-135">riskEventDateTime</span></span>|<span data-ttu-id="3de75-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de75-136">dateTimeOffset</span></span>| <span data-ttu-id="3de75-137">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="3de75-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="3de75-138">Рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="3de75-138">riskEventStatus</span></span>|<span data-ttu-id="3de75-139">string</span><span class="sxs-lookup"><span data-stu-id="3de75-139">string</span></span>| <span data-ttu-id="3de75-140">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="3de75-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="3de75-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="3de75-141">riskLevel</span></span>|<span data-ttu-id="3de75-142">string</span><span class="sxs-lookup"><span data-stu-id="3de75-142">string</span></span>| <span data-ttu-id="3de75-143">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="3de75-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="3de75-144">Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="3de75-144">riskEventType</span></span>|<span data-ttu-id="3de75-145">string</span><span class="sxs-lookup"><span data-stu-id="3de75-145">string</span></span>| <span data-ttu-id="3de75-146">Тип риска</span><span class="sxs-lookup"><span data-stu-id="3de75-146">The type of risk</span></span>|
|<span data-ttu-id="3de75-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3de75-147">userDisplayName</span></span>|<span data-ttu-id="3de75-148">string</span><span class="sxs-lookup"><span data-stu-id="3de75-148">string</span></span>| <span data-ttu-id="3de75-149">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="3de75-149">The name of the user at risk</span></span>|
|<span data-ttu-id="3de75-150">userId</span><span class="sxs-lookup"><span data-stu-id="3de75-150">userId</span></span>|<span data-ttu-id="3de75-151">string</span><span class="sxs-lookup"><span data-stu-id="3de75-151">string</span></span>| <span data-ttu-id="3de75-152">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="3de75-152">The id of the user at risk</span></span>|
|<span data-ttu-id="3de75-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3de75-153">userPrincipalName</span></span>|<span data-ttu-id="3de75-154">string</span><span class="sxs-lookup"><span data-stu-id="3de75-154">string</span></span>| <span data-ttu-id="3de75-155">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="3de75-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="3de75-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="3de75-156">Relationships</span></span>
| <span data-ttu-id="3de75-157">Отношение</span><span class="sxs-lookup"><span data-stu-id="3de75-157">Relationship</span></span> | <span data-ttu-id="3de75-158">Тип</span><span class="sxs-lookup"><span data-stu-id="3de75-158">Type</span></span>   |<span data-ttu-id="3de75-159">Описание</span><span class="sxs-lookup"><span data-stu-id="3de75-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3de75-160">Импактедусер</span><span class="sxs-lookup"><span data-stu-id="3de75-160">impactedUser</span></span>|[<span data-ttu-id="3de75-161">user</span><span class="sxs-lookup"><span data-stu-id="3de75-161">user</span></span>](user.md)| <span data-ttu-id="3de75-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="3de75-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3de75-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3de75-164">JSON representation</span></span>

<span data-ttu-id="3de75-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3de75-165">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
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
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
