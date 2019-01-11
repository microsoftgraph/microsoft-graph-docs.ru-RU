---
title: Тип ресурса anonymousIpRiskEvent
description: Событие риск, обнаруженных защитой Azure Active Directory Identity которых учетной записи входа в попытке от IP-адрес, который отображается для анонимного. Полные сведения о событиях риска можно найти в документации по Azure AD защиту.
localization_priority: Normal
ms.openlocfilehash: 9c170e234116ca76e4dabe021c0aa7949d1a66ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848302"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="ebf6c-104">Тип ресурса anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ebf6c-104">anonymousIpRiskEvent resource type</span></span>

> <span data-ttu-id="ebf6c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ebf6c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ebf6c-107">Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) где учетной записи входа в предпринимается попытка из IP-адрес, который будет иметь анонимный.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="ebf6c-108">Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="ebf6c-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="ebf6c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ebf6c-109">Methods</span></span>

| <span data-ttu-id="ebf6c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ebf6c-110">Method</span></span>           | <span data-ttu-id="ebf6c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ebf6c-111">Return Type</span></span>    |<span data-ttu-id="ebf6c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ebf6c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ebf6c-113">Получение anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ebf6c-113">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="ebf6c-114">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="ebf6c-114">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="ebf6c-115">Чтение свойства и связи объекта anonymousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-115">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ebf6c-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebf6c-116">Properties</span></span>
| <span data-ttu-id="ebf6c-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebf6c-117">Property</span></span>     | <span data-ttu-id="ebf6c-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ebf6c-118">Type</span></span>   |<span data-ttu-id="ebf6c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ebf6c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebf6c-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebf6c-120">closedDateTime</span></span>|<span data-ttu-id="ebf6c-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebf6c-121">dateTimeOffset</span></span>| <span data-ttu-id="ebf6c-122">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="ebf6c-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="ebf6c-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ebf6c-123">createdDateTime</span></span>|<span data-ttu-id="ebf6c-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebf6c-124">dateTimeOffset</span></span>| <span data-ttu-id="ebf6c-125">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="ebf6c-126">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="ebf6c-127">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="ebf6c-128">id</span><span class="sxs-lookup"><span data-stu-id="ebf6c-128">id</span></span>|<span data-ttu-id="ebf6c-129">строка</span><span class="sxs-lookup"><span data-stu-id="ebf6c-129">string</span></span>| <span data-ttu-id="ebf6c-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="ebf6c-130">Read-only</span></span>|
|<span data-ttu-id="ebf6c-131">ipAddress</span><span class="sxs-lookup"><span data-stu-id="ebf6c-131">ipAddress</span></span>|<span data-ttu-id="ebf6c-132">string</span><span class="sxs-lookup"><span data-stu-id="ebf6c-132">string</span></span>| <span data-ttu-id="ebf6c-133">IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="ebf6c-133">The IP address of the sign-in</span></span>|
|<span data-ttu-id="ebf6c-134">location</span><span class="sxs-lookup"><span data-stu-id="ebf6c-134">location</span></span>|<span data-ttu-id="ebf6c-135">string</span><span class="sxs-lookup"><span data-stu-id="ebf6c-135">string</span></span>| <span data-ttu-id="ebf6c-136">Расположение, подключенного к IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="ebf6c-136">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="ebf6c-137">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="ebf6c-137">riskEventDateTime</span></span>|<span data-ttu-id="ebf6c-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebf6c-138">dateTimeOffset</span></span>| <span data-ttu-id="ebf6c-139">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="ebf6c-139">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="ebf6c-140">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="ebf6c-140">riskEventStatus</span></span>|<span data-ttu-id="ebf6c-141">string</span><span class="sxs-lookup"><span data-stu-id="ebf6c-141">string</span></span>| <span data-ttu-id="ebf6c-142">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-142">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="ebf6c-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ebf6c-143">riskLevel</span></span>|<span data-ttu-id="ebf6c-144">string</span><span class="sxs-lookup"><span data-stu-id="ebf6c-144">string</span></span>| <span data-ttu-id="ebf6c-145">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-145">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="ebf6c-146">riskEventType</span><span class="sxs-lookup"><span data-stu-id="ebf6c-146">riskEventType</span></span>|<span data-ttu-id="ebf6c-147">string</span><span class="sxs-lookup"><span data-stu-id="ebf6c-147">string</span></span>| <span data-ttu-id="ebf6c-148">Тип риска</span><span class="sxs-lookup"><span data-stu-id="ebf6c-148">The type of risk</span></span>|
|<span data-ttu-id="ebf6c-149">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ebf6c-149">userDisplayName</span></span>|<span data-ttu-id="ebf6c-150">string</span><span class="sxs-lookup"><span data-stu-id="ebf6c-150">string</span></span>| <span data-ttu-id="ebf6c-151">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="ebf6c-151">The name of the user at risk</span></span>|
|<span data-ttu-id="ebf6c-152">userId</span><span class="sxs-lookup"><span data-stu-id="ebf6c-152">userId</span></span>|<span data-ttu-id="ebf6c-153">string</span><span class="sxs-lookup"><span data-stu-id="ebf6c-153">string</span></span>| <span data-ttu-id="ebf6c-154">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="ebf6c-154">The id of the user at risk</span></span>|
|<span data-ttu-id="ebf6c-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ebf6c-155">userPrincipalName</span></span>|<span data-ttu-id="ebf6c-156">string</span><span class="sxs-lookup"><span data-stu-id="ebf6c-156">string</span></span>| <span data-ttu-id="ebf6c-157">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="ebf6c-157">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebf6c-158">Связи</span><span class="sxs-lookup"><span data-stu-id="ebf6c-158">Relationships</span></span>
| <span data-ttu-id="ebf6c-159">Связь</span><span class="sxs-lookup"><span data-stu-id="ebf6c-159">Relationship</span></span> | <span data-ttu-id="ebf6c-160">Тип</span><span class="sxs-lookup"><span data-stu-id="ebf6c-160">Type</span></span>   |<span data-ttu-id="ebf6c-161">Описание</span><span class="sxs-lookup"><span data-stu-id="ebf6c-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebf6c-162">impactedUser</span><span class="sxs-lookup"><span data-stu-id="ebf6c-162">impactedUser</span></span>|[<span data-ttu-id="ebf6c-163">user</span><span class="sxs-lookup"><span data-stu-id="ebf6c-163">user</span></span>](user.md)| <span data-ttu-id="ebf6c-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebf6c-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ebf6c-166">JSON representation</span></span>

<span data-ttu-id="ebf6c-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ebf6c-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
