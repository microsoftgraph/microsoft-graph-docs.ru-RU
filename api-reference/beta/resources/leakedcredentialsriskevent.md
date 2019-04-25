---
title: Тип ресурса Леакедкредентиалсрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором были обнаружены учетные данные учетной записи в подстановке. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
ms.openlocfilehash: 0884da08195ffa2bee38c943d27b1d25aef02e49
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581098"
---
# <a name="leakedcredentialsriskevent-resource-type"></a><span data-ttu-id="feddf-104">Тип ресурса Леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="feddf-104">leakedCredentialsRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feddf-105">Событие риска, обнаруженное службой [удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , в котором были обнаружены учетные данные учетной записи в подстановке.</span><span class="sxs-lookup"><span data-stu-id="feddf-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account's credentials have been detected in the wild.</span></span> <span data-ttu-id="feddf-106">Полную информацию о событиях риска можно найти в [документации по защите удостоверенИй Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="feddf-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="feddf-107">Методы</span><span class="sxs-lookup"><span data-stu-id="feddf-107">Methods</span></span>

| <span data-ttu-id="feddf-108">Метод</span><span class="sxs-lookup"><span data-stu-id="feddf-108">Method</span></span>           | <span data-ttu-id="feddf-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="feddf-109">Return Type</span></span>    |<span data-ttu-id="feddf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="feddf-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="feddf-111">Получение объекта leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="feddf-111">Get leakedCredentialsRiskEvent</span></span>](../api/leakedcredentialsriskevent-get.md) | [<span data-ttu-id="feddf-112">Леакедкредентиалсрискевент</span><span class="sxs-lookup"><span data-stu-id="feddf-112">leakedCredentialsRiskEvent</span></span>](leakedcredentialsriskevent.md) |<span data-ttu-id="feddf-113">Чтение свойств и связей объекта Леакедкредентиалсрискевент.</span><span class="sxs-lookup"><span data-stu-id="feddf-113">Read properties and relationships of leakedCredentialsRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="feddf-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="feddf-114">Properties</span></span>
| <span data-ttu-id="feddf-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="feddf-115">Property</span></span>     | <span data-ttu-id="feddf-116">Тип</span><span class="sxs-lookup"><span data-stu-id="feddf-116">Type</span></span>   |<span data-ttu-id="feddf-117">Описание</span><span class="sxs-lookup"><span data-stu-id="feddf-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="feddf-118">Клоседдатетиме</span><span class="sxs-lookup"><span data-stu-id="feddf-118">closedDateTime</span></span>|<span data-ttu-id="feddf-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feddf-119">dateTimeOffset</span></span>| <span data-ttu-id="feddf-120">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="feddf-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="feddf-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="feddf-121">createdDateTime</span></span>|<span data-ttu-id="feddf-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feddf-122">dateTimeOffset</span></span>| <span data-ttu-id="feddf-123">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="feddf-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="feddf-124">Он всегда больше или равен значению DateTime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="feddf-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="feddf-125">Это правильное свойство, используемое в качестве фильтра при запросе событий риска.</span><span class="sxs-lookup"><span data-stu-id="feddf-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="feddf-126">id</span><span class="sxs-lookup"><span data-stu-id="feddf-126">id</span></span>|<span data-ttu-id="feddf-127">string</span><span class="sxs-lookup"><span data-stu-id="feddf-127">string</span></span>| <span data-ttu-id="feddf-128">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="feddf-128">Read-only</span></span>|
|<span data-ttu-id="feddf-129">Рискевентдатетиме</span><span class="sxs-lookup"><span data-stu-id="feddf-129">riskEventDateTime</span></span>|<span data-ttu-id="feddf-130">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feddf-130">dateTimeOffset</span></span>| <span data-ttu-id="feddf-131">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="feddf-131">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="feddf-132">Рискевентстатус</span><span class="sxs-lookup"><span data-stu-id="feddf-132">riskEventStatus</span></span>|<span data-ttu-id="feddf-133">string</span><span class="sxs-lookup"><span data-stu-id="feddf-133">string</span></span>| <span data-ttu-id="feddf-134">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="feddf-134">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="feddf-135">riskLevel</span><span class="sxs-lookup"><span data-stu-id="feddf-135">riskLevel</span></span>|<span data-ttu-id="feddf-136">string</span><span class="sxs-lookup"><span data-stu-id="feddf-136">string</span></span>| <span data-ttu-id="feddf-137">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="feddf-137">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="feddf-138">Рискевенттипе</span><span class="sxs-lookup"><span data-stu-id="feddf-138">riskEventType</span></span>|<span data-ttu-id="feddf-139">string</span><span class="sxs-lookup"><span data-stu-id="feddf-139">string</span></span>| <span data-ttu-id="feddf-140">Тип риска</span><span class="sxs-lookup"><span data-stu-id="feddf-140">The type of risk</span></span>|
|<span data-ttu-id="feddf-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="feddf-141">userDisplayName</span></span>|<span data-ttu-id="feddf-142">string</span><span class="sxs-lookup"><span data-stu-id="feddf-142">string</span></span>| <span data-ttu-id="feddf-143">Имя пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="feddf-143">The name of the user at risk</span></span>|
|<span data-ttu-id="feddf-144">userId</span><span class="sxs-lookup"><span data-stu-id="feddf-144">userId</span></span>|<span data-ttu-id="feddf-145">string</span><span class="sxs-lookup"><span data-stu-id="feddf-145">string</span></span>| <span data-ttu-id="feddf-146">Идентификатор пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="feddf-146">The id of the user at risk</span></span>|
|<span data-ttu-id="feddf-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="feddf-147">userPrincipalName</span></span>|<span data-ttu-id="feddf-148">string</span><span class="sxs-lookup"><span data-stu-id="feddf-148">string</span></span>| <span data-ttu-id="feddf-149">Имя участника пользователя, который подвергается риску</span><span class="sxs-lookup"><span data-stu-id="feddf-149">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="feddf-150">Связи</span><span class="sxs-lookup"><span data-stu-id="feddf-150">Relationships</span></span>
| <span data-ttu-id="feddf-151">Отношение</span><span class="sxs-lookup"><span data-stu-id="feddf-151">Relationship</span></span> | <span data-ttu-id="feddf-152">Тип</span><span class="sxs-lookup"><span data-stu-id="feddf-152">Type</span></span>   |<span data-ttu-id="feddf-153">Описание</span><span class="sxs-lookup"><span data-stu-id="feddf-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="feddf-154">Импактедусер</span><span class="sxs-lookup"><span data-stu-id="feddf-154">impactedUser</span></span>|[<span data-ttu-id="feddf-155">user</span><span class="sxs-lookup"><span data-stu-id="feddf-155">user</span></span>](user.md)| <span data-ttu-id="feddf-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="feddf-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="feddf-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="feddf-158">JSON representation</span></span>

<span data-ttu-id="feddf-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feddf-159">Here is a JSON representation of the resource.</span></span>

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
