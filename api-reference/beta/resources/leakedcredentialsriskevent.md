---
title: Тип ресурса leakedCredentialsRiskEvent
description: Событие риск, обнаруженных защитой Azure Active Directory Identity которых обнаружены учетные данные учетной записи в мире. Полные сведения о событиях риска можно найти в документации по Azure AD защиту.
localization_priority: Normal
ms.openlocfilehash: 0884da08195ffa2bee38c943d27b1d25aef02e49
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510990"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="5bd9d-104">Тип ресурса leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="5bd9d-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bd9d-105">Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , где в мире обнаружены учетные данные учетной записи.</span><span class="sxs-lookup"><span data-stu-id="5bd9d-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="5bd9d-106">Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="5bd9d-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="5bd9d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5bd9d-107">Methods</span></span>

| <span data-ttu-id="5bd9d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5bd9d-108">Method</span></span>           | <span data-ttu-id="5bd9d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5bd9d-109">Return Type</span></span>    |<span data-ttu-id="5bd9d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd9d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5bd9d-111">Получение leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="5bd9d-111">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="5bd9d-112">leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="5bd9d-112">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="5bd9d-113">Чтение свойства и связи объекта leakedCredentialsRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="5bd9d-113">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5bd9d-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bd9d-114">Properties</span></span>
| <span data-ttu-id="5bd9d-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bd9d-115">Property</span></span>     | <span data-ttu-id="5bd9d-116">Тип</span><span class="sxs-lookup"><span data-stu-id="5bd9d-116">Type</span></span>   |<span data-ttu-id="5bd9d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd9d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bd9d-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd9d-118">closedDateTime</span></span>|<span data-ttu-id="5bd9d-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd9d-119">dateTimeOffset</span></span>| <span data-ttu-id="5bd9d-120">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="5bd9d-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="5bd9d-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd9d-121">createdDateTime</span></span>|<span data-ttu-id="5bd9d-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd9d-122">dateTimeOffset</span></span>| <span data-ttu-id="5bd9d-123">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="5bd9d-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="5bd9d-124">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="5bd9d-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="5bd9d-125">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="5bd9d-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="5bd9d-126">id</span><span class="sxs-lookup"><span data-stu-id="5bd9d-126">id</span></span>|<span data-ttu-id="5bd9d-127">string</span><span class="sxs-lookup"><span data-stu-id="5bd9d-127">string</span></span>| <span data-ttu-id="5bd9d-128">Только чтение</span><span class="sxs-lookup"><span data-stu-id="5bd9d-128">Read-only</span></span>|
|<span data-ttu-id="5bd9d-129">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="5bd9d-129">riskEventDateTime</span></span>|<span data-ttu-id="5bd9d-130">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bd9d-130">dateTimeOffset</span></span>| <span data-ttu-id="5bd9d-131">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="5bd9d-131">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="5bd9d-132">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="5bd9d-132">riskEventStatus</span></span>|<span data-ttu-id="5bd9d-133">string</span><span class="sxs-lookup"><span data-stu-id="5bd9d-133">string</span></span>| <span data-ttu-id="5bd9d-134">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="5bd9d-134">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="5bd9d-135">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5bd9d-135">riskLevel</span></span>|<span data-ttu-id="5bd9d-136">string</span><span class="sxs-lookup"><span data-stu-id="5bd9d-136">string</span></span>| <span data-ttu-id="5bd9d-137">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="5bd9d-137">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="5bd9d-138">riskEventType</span><span class="sxs-lookup"><span data-stu-id="5bd9d-138">riskEventType</span></span>|<span data-ttu-id="5bd9d-139">string</span><span class="sxs-lookup"><span data-stu-id="5bd9d-139">string</span></span>| <span data-ttu-id="5bd9d-140">Тип риска</span><span class="sxs-lookup"><span data-stu-id="5bd9d-140">The type of risk</span></span>|
|<span data-ttu-id="5bd9d-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5bd9d-141">userDisplayName</span></span>|<span data-ttu-id="5bd9d-142">string</span><span class="sxs-lookup"><span data-stu-id="5bd9d-142">string</span></span>| <span data-ttu-id="5bd9d-143">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="5bd9d-143">The name of the user at risk</span></span>|
|<span data-ttu-id="5bd9d-144">userId</span><span class="sxs-lookup"><span data-stu-id="5bd9d-144">userId</span></span>|<span data-ttu-id="5bd9d-145">string</span><span class="sxs-lookup"><span data-stu-id="5bd9d-145">string</span></span>| <span data-ttu-id="5bd9d-146">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="5bd9d-146">The id of the user at risk</span></span>|
|<span data-ttu-id="5bd9d-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5bd9d-147">userPrincipalName</span></span>|<span data-ttu-id="5bd9d-148">string</span><span class="sxs-lookup"><span data-stu-id="5bd9d-148">string</span></span>| <span data-ttu-id="5bd9d-149">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="5bd9d-149">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bd9d-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="5bd9d-150">Relationships</span></span>
| <span data-ttu-id="5bd9d-151">Связь</span><span class="sxs-lookup"><span data-stu-id="5bd9d-151">Relationship</span></span> | <span data-ttu-id="5bd9d-152">Тип</span><span class="sxs-lookup"><span data-stu-id="5bd9d-152">Type</span></span>   |<span data-ttu-id="5bd9d-153">Описание</span><span class="sxs-lookup"><span data-stu-id="5bd9d-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bd9d-154">impactedUser</span><span class="sxs-lookup"><span data-stu-id="5bd9d-154">impactedUser</span></span>|[<span data-ttu-id="5bd9d-155">user</span><span class="sxs-lookup"><span data-stu-id="5bd9d-155">user</span></span>](user.md)| <span data-ttu-id="5bd9d-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5bd9d-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bd9d-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bd9d-158">JSON representation</span></span>

<span data-ttu-id="5bd9d-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bd9d-159">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "leakedCredentialsRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/leakedcredentialsriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
