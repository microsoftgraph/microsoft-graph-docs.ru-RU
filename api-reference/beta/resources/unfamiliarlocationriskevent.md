---
title: Тип ресурса Унфамилиарлокатионрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором выполняется попытка входа учетной записи из нового расположения для этого пользователя. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c6f46c1440ccc83dac7e57044e3758f6faf96cee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519626"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a><span data-ttu-id="09273-104">Тип ресурса Унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="09273-104">unfamiliarLocationRiskEvent resource type</span></span>

<span data-ttu-id="09273-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09273-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="09273-106">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="09273-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="09273-107">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="09273-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="09273-108">Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) , в котором выполняется попытка входа учетной записи из нового расположения для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="09273-108">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from a new location for that user.</span></span> <span data-ttu-id="09273-109">Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="09273-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="09273-110">Методы</span><span class="sxs-lookup"><span data-stu-id="09273-110">Methods</span></span>

| <span data-ttu-id="09273-111">Метод</span><span class="sxs-lookup"><span data-stu-id="09273-111">Method</span></span>           | <span data-ttu-id="09273-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="09273-112">Return Type</span></span>    |<span data-ttu-id="09273-113">Описание</span><span class="sxs-lookup"><span data-stu-id="09273-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09273-114">Получение объекта unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="09273-114">Get unfamiliarLocationRiskEvent</span></span>](../api/unfamiliarlocationriskevent-get.md) | [<span data-ttu-id="09273-115">унфамилиарлокатионрискевент</span><span class="sxs-lookup"><span data-stu-id="09273-115">unfamiliarLocationRiskEvent</span></span>](unfamiliarlocationriskevent.md) |<span data-ttu-id="09273-116">Чтение свойств и связей объекта Унфамилиарлокатионрискевент.</span><span class="sxs-lookup"><span data-stu-id="09273-116">Read properties and relationships of unfamiliarLocationRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="09273-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="09273-117">Properties</span></span>
| <span data-ttu-id="09273-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="09273-118">Property</span></span>     | <span data-ttu-id="09273-119">Тип</span><span class="sxs-lookup"><span data-stu-id="09273-119">Type</span></span>   |<span data-ttu-id="09273-120">Описание</span><span class="sxs-lookup"><span data-stu-id="09273-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09273-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="09273-121">closedDateTime</span></span>|<span data-ttu-id="09273-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09273-122">dateTimeOffset</span></span>| <span data-ttu-id="09273-123">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="09273-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="09273-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09273-124">createdDateTime</span></span>|<span data-ttu-id="09273-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09273-125">dateTimeOffset</span></span>| <span data-ttu-id="09273-126">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="09273-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="09273-127">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="09273-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="09273-128">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="09273-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="09273-129">id</span><span class="sxs-lookup"><span data-stu-id="09273-129">id</span></span>|<span data-ttu-id="09273-130">string</span><span class="sxs-lookup"><span data-stu-id="09273-130">string</span></span>| <span data-ttu-id="09273-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="09273-131">Read-only</span></span>|
|<span data-ttu-id="09273-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="09273-132">ipAddress</span></span>|<span data-ttu-id="09273-133">string</span><span class="sxs-lookup"><span data-stu-id="09273-133">string</span></span>| <span data-ttu-id="09273-134">IP-адрес входа</span><span class="sxs-lookup"><span data-stu-id="09273-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="09273-135">location</span><span class="sxs-lookup"><span data-stu-id="09273-135">location</span></span>|<span data-ttu-id="09273-136">string</span><span class="sxs-lookup"><span data-stu-id="09273-136">string</span></span>| <span data-ttu-id="09273-137">Расположение, подключенное к IP-адресу входа</span><span class="sxs-lookup"><span data-stu-id="09273-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="09273-138">рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="09273-138">riskEventDateTime</span></span>|<span data-ttu-id="09273-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09273-139">dateTimeOffset</span></span>| <span data-ttu-id="09273-140">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="09273-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="09273-141">рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="09273-141">riskEventStatus</span></span>|<span data-ttu-id="09273-142">string</span><span class="sxs-lookup"><span data-stu-id="09273-142">string</span></span>| <span data-ttu-id="09273-143">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="09273-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="09273-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="09273-144">riskLevel</span></span>|<span data-ttu-id="09273-145">string</span><span class="sxs-lookup"><span data-stu-id="09273-145">string</span></span>| <span data-ttu-id="09273-146">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="09273-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="09273-147">рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="09273-147">riskEventType</span></span>|<span data-ttu-id="09273-148">string</span><span class="sxs-lookup"><span data-stu-id="09273-148">string</span></span>| <span data-ttu-id="09273-149">Тип риска</span><span class="sxs-lookup"><span data-stu-id="09273-149">The type of risk</span></span>|
|<span data-ttu-id="09273-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="09273-150">userDisplayName</span></span>|<span data-ttu-id="09273-151">string</span><span class="sxs-lookup"><span data-stu-id="09273-151">string</span></span>| <span data-ttu-id="09273-152">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="09273-152">The name of the user at risk</span></span>|
|<span data-ttu-id="09273-153">userId</span><span class="sxs-lookup"><span data-stu-id="09273-153">userId</span></span>|<span data-ttu-id="09273-154">строка</span><span class="sxs-lookup"><span data-stu-id="09273-154">string</span></span>| <span data-ttu-id="09273-155">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="09273-155">The id of the user at risk</span></span>|
|<span data-ttu-id="09273-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="09273-156">userPrincipalName</span></span>|<span data-ttu-id="09273-157">string</span><span class="sxs-lookup"><span data-stu-id="09273-157">string</span></span>| <span data-ttu-id="09273-158">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="09273-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="09273-159">Связи</span><span class="sxs-lookup"><span data-stu-id="09273-159">Relationships</span></span>
| <span data-ttu-id="09273-160">Связь</span><span class="sxs-lookup"><span data-stu-id="09273-160">Relationship</span></span> | <span data-ttu-id="09273-161">Тип</span><span class="sxs-lookup"><span data-stu-id="09273-161">Type</span></span>   |<span data-ttu-id="09273-162">Описание</span><span class="sxs-lookup"><span data-stu-id="09273-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09273-163">импактедусер</span><span class="sxs-lookup"><span data-stu-id="09273-163">impactedUser</span></span>|[<span data-ttu-id="09273-164">user</span><span class="sxs-lookup"><span data-stu-id="09273-164">user</span></span>](user.md)| <span data-ttu-id="09273-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="09273-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09273-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09273-167">JSON representation</span></span>

<span data-ttu-id="09273-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09273-168">Here is a JSON representation of the resource.</span></span>

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
