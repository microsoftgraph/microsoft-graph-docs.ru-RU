---
title: тип ресурсов anonymousIpRiskEvent
description: Событие риска, обнаруженное Azure Active Directory identity Protection, в котором с IP-адреса, который кажется анонимным, попытается войти учетная запись. Полные сведения о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: d4acf5d9b3d5d05a2769178657b397b22f1cb3f2
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547550"
---
# <a name="anonymousipriskevent-resource-type-deprecated"></a><span data-ttu-id="1aa69-104">тип ресурсов anonymousIpRiskEvent (неподготовленный)</span><span class="sxs-lookup"><span data-stu-id="1aa69-104">anonymousIpRiskEvent resource type (deprecated)</span></span>

<span data-ttu-id="1aa69-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1aa69-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="1aa69-106">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="1aa69-106">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="1aa69-107">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="1aa69-107">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="1aa69-108">Событие риска, обнаруженное Azure Active Directory identity Protection, в котором с [IP-адреса,](/azure/active-directory/identity-protection/overview-identity-protection) который кажется анонимным, попытается войти учетная запись.</span><span class="sxs-lookup"><span data-stu-id="1aa69-108">A risk event detected by [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="1aa69-109">Полные сведения о событиях риска можно найти в документации [azure AD Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="1aa69-109">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>


## <a name="methods"></a><span data-ttu-id="1aa69-110">Методы</span><span class="sxs-lookup"><span data-stu-id="1aa69-110">Methods</span></span>

| <span data-ttu-id="1aa69-111">Метод</span><span class="sxs-lookup"><span data-stu-id="1aa69-111">Method</span></span>           | <span data-ttu-id="1aa69-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1aa69-112">Return Type</span></span>    |<span data-ttu-id="1aa69-113">Описание</span><span class="sxs-lookup"><span data-stu-id="1aa69-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1aa69-114">Получение объекта anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1aa69-114">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="1aa69-115">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="1aa69-115">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="1aa69-116">Чтение свойств и связей анонимного объектаIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="1aa69-116">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1aa69-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="1aa69-117">Properties</span></span>
| <span data-ttu-id="1aa69-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="1aa69-118">Property</span></span>     | <span data-ttu-id="1aa69-119">Тип</span><span class="sxs-lookup"><span data-stu-id="1aa69-119">Type</span></span>   |<span data-ttu-id="1aa69-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1aa69-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1aa69-121">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa69-121">closedDateTime</span></span>|<span data-ttu-id="1aa69-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa69-122">dateTimeOffset</span></span>| <span data-ttu-id="1aa69-123">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="1aa69-123">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="1aa69-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa69-124">createdDateTime</span></span>|<span data-ttu-id="1aa69-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa69-125">dateTimeOffset</span></span>| <span data-ttu-id="1aa69-126">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="1aa69-126">The date and time that the risk event was created.</span></span> <span data-ttu-id="1aa69-127">Это всегда больше или равно дате самого события риска.</span><span class="sxs-lookup"><span data-stu-id="1aa69-127">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="1aa69-128">Это правильное свойство, используемее в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="1aa69-128">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="1aa69-129">id</span><span class="sxs-lookup"><span data-stu-id="1aa69-129">id</span></span>|<span data-ttu-id="1aa69-130">string</span><span class="sxs-lookup"><span data-stu-id="1aa69-130">string</span></span>| <span data-ttu-id="1aa69-131">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="1aa69-131">Read-only</span></span>|
|<span data-ttu-id="1aa69-132">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1aa69-132">ipAddress</span></span>|<span data-ttu-id="1aa69-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1aa69-133">string</span></span>| <span data-ttu-id="1aa69-134">IP-адрес входного</span><span class="sxs-lookup"><span data-stu-id="1aa69-134">The IP address of the sign-in</span></span>|
|<span data-ttu-id="1aa69-135">location</span><span class="sxs-lookup"><span data-stu-id="1aa69-135">location</span></span>|<span data-ttu-id="1aa69-136">string</span><span class="sxs-lookup"><span data-stu-id="1aa69-136">string</span></span>| <span data-ttu-id="1aa69-137">Расположение, прикрепленное к IP-адресу входного</span><span class="sxs-lookup"><span data-stu-id="1aa69-137">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="1aa69-138">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa69-138">riskEventDateTime</span></span>|<span data-ttu-id="1aa69-139">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa69-139">dateTimeOffset</span></span>| <span data-ttu-id="1aa69-140">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="1aa69-140">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="1aa69-141">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="1aa69-141">riskEventStatus</span></span>|<span data-ttu-id="1aa69-142">Строка</span><span class="sxs-lookup"><span data-stu-id="1aa69-142">string</span></span>| <span data-ttu-id="1aa69-143">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="1aa69-143">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="1aa69-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="1aa69-144">riskLevel</span></span>|<span data-ttu-id="1aa69-145">string</span><span class="sxs-lookup"><span data-stu-id="1aa69-145">string</span></span>| <span data-ttu-id="1aa69-146">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="1aa69-146">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="1aa69-147">riskEventType</span><span class="sxs-lookup"><span data-stu-id="1aa69-147">riskEventType</span></span>|<span data-ttu-id="1aa69-148">Строка</span><span class="sxs-lookup"><span data-stu-id="1aa69-148">string</span></span>| <span data-ttu-id="1aa69-149">Тип риска</span><span class="sxs-lookup"><span data-stu-id="1aa69-149">The type of risk</span></span>|
|<span data-ttu-id="1aa69-150">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1aa69-150">userDisplayName</span></span>|<span data-ttu-id="1aa69-151">Строка</span><span class="sxs-lookup"><span data-stu-id="1aa69-151">string</span></span>| <span data-ttu-id="1aa69-152">Имя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="1aa69-152">The name of the user at risk</span></span>|
|<span data-ttu-id="1aa69-153">userId</span><span class="sxs-lookup"><span data-stu-id="1aa69-153">userId</span></span>|<span data-ttu-id="1aa69-154">строка</span><span class="sxs-lookup"><span data-stu-id="1aa69-154">string</span></span>| <span data-ttu-id="1aa69-155">ID пользователя, на который существует риск</span><span class="sxs-lookup"><span data-stu-id="1aa69-155">The id of the user at risk</span></span>|
|<span data-ttu-id="1aa69-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1aa69-156">userPrincipalName</span></span>|<span data-ttu-id="1aa69-157">string</span><span class="sxs-lookup"><span data-stu-id="1aa69-157">string</span></span>| <span data-ttu-id="1aa69-158">Основное имя пользователя пользователя, на которого существует риск</span><span class="sxs-lookup"><span data-stu-id="1aa69-158">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aa69-159">Связи</span><span class="sxs-lookup"><span data-stu-id="1aa69-159">Relationships</span></span>
| <span data-ttu-id="1aa69-160">Связь</span><span class="sxs-lookup"><span data-stu-id="1aa69-160">Relationship</span></span> | <span data-ttu-id="1aa69-161">Тип</span><span class="sxs-lookup"><span data-stu-id="1aa69-161">Type</span></span>   |<span data-ttu-id="1aa69-162">Описание</span><span class="sxs-lookup"><span data-stu-id="1aa69-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1aa69-163">impactedUser</span><span class="sxs-lookup"><span data-stu-id="1aa69-163">impactedUser</span></span>|[<span data-ttu-id="1aa69-164">user</span><span class="sxs-lookup"><span data-stu-id="1aa69-164">user</span></span>](user.md)| <span data-ttu-id="1aa69-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="1aa69-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1aa69-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1aa69-167">JSON representation</span></span>

<span data-ttu-id="1aa69-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1aa69-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
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
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
