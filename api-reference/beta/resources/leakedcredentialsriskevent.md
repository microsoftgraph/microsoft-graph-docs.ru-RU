---
title: Тип ресурса leakedCredentialsRiskEvent
description: Событие риск, обнаруженных защитой Azure Active Directory Identity которых обнаружены учетные данные учетной записи в мире. Полные сведения о событиях риска можно найти в документации по Azure AD защиту.
ms.openlocfilehash: 2404564726c3ca7ee1f577b3d81daaa339941406
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081150"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="65411-104">Тип ресурса leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="65411-104">leakedCredentialsRiskEvent resource type</span></span>

> <span data-ttu-id="65411-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="65411-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65411-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65411-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="65411-107">Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , где в мире обнаружены учетные данные учетной записи.</span><span class="sxs-lookup"><span data-stu-id="65411-107">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="65411-108">Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="65411-108">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="65411-109">Методы</span><span class="sxs-lookup"><span data-stu-id="65411-109">Methods</span></span>

| <span data-ttu-id="65411-110">Метод</span><span class="sxs-lookup"><span data-stu-id="65411-110">Method</span></span>           | <span data-ttu-id="65411-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="65411-111">Return Type</span></span>    |<span data-ttu-id="65411-112">Описание</span><span class="sxs-lookup"><span data-stu-id="65411-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65411-113">Получение leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="65411-113">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="65411-114">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="65411-114">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="65411-115">Чтение свойства и связи объекта leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="65411-115">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="65411-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="65411-116">Properties</span></span>
| <span data-ttu-id="65411-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="65411-117">Property</span></span>     | <span data-ttu-id="65411-118">Тип</span><span class="sxs-lookup"><span data-stu-id="65411-118">Type</span></span>   |<span data-ttu-id="65411-119">Description</span><span class="sxs-lookup"><span data-stu-id="65411-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65411-120">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="65411-120">closedDateTime</span></span>|<span data-ttu-id="65411-121">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65411-121">dateTimeOffset</span></span>| <span data-ttu-id="65411-122">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="65411-122">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="65411-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65411-123">createdDateTime</span></span>|<span data-ttu-id="65411-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65411-124">dateTimeOffset</span></span>| <span data-ttu-id="65411-125">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="65411-125">The date and time that the risk event was created.</span></span> <span data-ttu-id="65411-126">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="65411-126">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="65411-127">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="65411-127">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="65411-128">id</span><span class="sxs-lookup"><span data-stu-id="65411-128">id</span></span>|<span data-ttu-id="65411-129">строка</span><span class="sxs-lookup"><span data-stu-id="65411-129">string</span></span>| <span data-ttu-id="65411-130">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="65411-130">Read-only</span></span>|
|<span data-ttu-id="65411-131">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="65411-131">riskEventDateTime</span></span>|<span data-ttu-id="65411-132">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65411-132">dateTimeOffset</span></span>| <span data-ttu-id="65411-133">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="65411-133">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="65411-134">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="65411-134">riskEventStatus</span></span>|<span data-ttu-id="65411-135">string</span><span class="sxs-lookup"><span data-stu-id="65411-135">string</span></span>| <span data-ttu-id="65411-136">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="65411-136">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="65411-137">riskLevel</span><span class="sxs-lookup"><span data-stu-id="65411-137">riskLevel</span></span>|<span data-ttu-id="65411-138">string</span><span class="sxs-lookup"><span data-stu-id="65411-138">string</span></span>| <span data-ttu-id="65411-139">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="65411-139">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="65411-140">riskEventType</span><span class="sxs-lookup"><span data-stu-id="65411-140">riskEventType</span></span>|<span data-ttu-id="65411-141">string</span><span class="sxs-lookup"><span data-stu-id="65411-141">string</span></span>| <span data-ttu-id="65411-142">Тип риска</span><span class="sxs-lookup"><span data-stu-id="65411-142">The type of risk</span></span>|
|<span data-ttu-id="65411-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="65411-143">userDisplayName</span></span>|<span data-ttu-id="65411-144">string</span><span class="sxs-lookup"><span data-stu-id="65411-144">string</span></span>| <span data-ttu-id="65411-145">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="65411-145">The name of the user at risk</span></span>|
|<span data-ttu-id="65411-146">userId</span><span class="sxs-lookup"><span data-stu-id="65411-146">userId</span></span>|<span data-ttu-id="65411-147">string</span><span class="sxs-lookup"><span data-stu-id="65411-147">string</span></span>| <span data-ttu-id="65411-148">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="65411-148">The id of the user at risk</span></span>|
|<span data-ttu-id="65411-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="65411-149">userPrincipalName</span></span>|<span data-ttu-id="65411-150">string</span><span class="sxs-lookup"><span data-stu-id="65411-150">string</span></span>| <span data-ttu-id="65411-151">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="65411-151">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="65411-152">Связи</span><span class="sxs-lookup"><span data-stu-id="65411-152">Relationships</span></span>
| <span data-ttu-id="65411-153">Связь</span><span class="sxs-lookup"><span data-stu-id="65411-153">Relationship</span></span> | <span data-ttu-id="65411-154">Тип</span><span class="sxs-lookup"><span data-stu-id="65411-154">Type</span></span>   |<span data-ttu-id="65411-155">Description</span><span class="sxs-lookup"><span data-stu-id="65411-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65411-156">impactedUser</span><span class="sxs-lookup"><span data-stu-id="65411-156">impactedUser</span></span>|[<span data-ttu-id="65411-157">user</span><span class="sxs-lookup"><span data-stu-id="65411-157">user</span></span>](user.md)| <span data-ttu-id="65411-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="65411-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65411-160">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65411-160">JSON representation</span></span>

<span data-ttu-id="65411-161">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65411-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
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
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->