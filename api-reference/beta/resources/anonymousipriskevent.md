---
title: Тип ресурса anonymousIpRiskEvent
description: Событие риск, обнаруженных защитой Azure Active Directory Identity которых учетной записи входа в попытке от IP-адрес, который отображается для анонимного. Полные сведения о событиях риска можно найти в документации по Azure AD защиту.
localization_priority: Normal
ms.openlocfilehash: 5f428a99466e67dfbbe4ef9b4ebe0006b56f99e9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519768"
---
# <a name="anonymousipriskevent-resource-type"></a><span data-ttu-id="e676c-104">Тип ресурса anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e676c-104">anonymousIpRiskEvent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e676c-105">Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) где учетной записи входа в предпринимается попытка из IP-адрес, который будет иметь анонимный.</span><span class="sxs-lookup"><span data-stu-id="e676c-105">A risk event detected by [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) where an account sign-in is attempted from an IP address that appears to be anonymous.</span></span> <span data-ttu-id="e676c-106">Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span><span class="sxs-lookup"><span data-stu-id="e676c-106">Complete information about risk events can be found in the [Azure AD Identity Protection documentation](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).</span></span>


## <a name="methods"></a><span data-ttu-id="e676c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e676c-107">Methods</span></span>

| <span data-ttu-id="e676c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="e676c-108">Method</span></span>           | <span data-ttu-id="e676c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e676c-109">Return Type</span></span>    |<span data-ttu-id="e676c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e676c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e676c-111">Получение anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e676c-111">Get anonymousIpRiskEvent</span></span>](../api/anonymousipriskevent-get.md) | [<span data-ttu-id="e676c-112">anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e676c-112">anonymousIpRiskEvent</span></span>](anonymousipriskevent.md) |<span data-ttu-id="e676c-113">Чтение свойства и связи объекта anonymousIpRiskEvent.</span><span class="sxs-lookup"><span data-stu-id="e676c-113">Read properties and relationships of anonymousIpRiskEvent object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e676c-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="e676c-114">Properties</span></span>
| <span data-ttu-id="e676c-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="e676c-115">Property</span></span>     | <span data-ttu-id="e676c-116">Тип</span><span class="sxs-lookup"><span data-stu-id="e676c-116">Type</span></span>   |<span data-ttu-id="e676c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="e676c-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e676c-118">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="e676c-118">closedDateTime</span></span>|<span data-ttu-id="e676c-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e676c-119">dateTimeOffset</span></span>| <span data-ttu-id="e676c-120">Дата и время закрытия события риска</span><span class="sxs-lookup"><span data-stu-id="e676c-120">The date and time that the risk event was closed</span></span>|
|<span data-ttu-id="e676c-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e676c-121">createdDateTime</span></span>|<span data-ttu-id="e676c-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e676c-122">dateTimeOffset</span></span>| <span data-ttu-id="e676c-123">Дата и время создания события риска.</span><span class="sxs-lookup"><span data-stu-id="e676c-123">The date and time that the risk event was created.</span></span> <span data-ttu-id="e676c-124">Это всегда больше или равно datetime самого события риска.</span><span class="sxs-lookup"><span data-stu-id="e676c-124">This is always greater than or equal to the datetime of the risk event itself.</span></span> <span data-ttu-id="e676c-125">Это правильное свойство для использования в качестве фильтра при запросе события рисков.</span><span class="sxs-lookup"><span data-stu-id="e676c-125">This is the correct property to use as a filter when querying risk events.</span></span>|
|<span data-ttu-id="e676c-126">id</span><span class="sxs-lookup"><span data-stu-id="e676c-126">id</span></span>|<span data-ttu-id="e676c-127">string</span><span class="sxs-lookup"><span data-stu-id="e676c-127">string</span></span>| <span data-ttu-id="e676c-128">Только чтение</span><span class="sxs-lookup"><span data-stu-id="e676c-128">Read-only</span></span>|
|<span data-ttu-id="e676c-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e676c-129">ipAddress</span></span>|<span data-ttu-id="e676c-130">string</span><span class="sxs-lookup"><span data-stu-id="e676c-130">string</span></span>| <span data-ttu-id="e676c-131">IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="e676c-131">The IP address of the sign-in</span></span>|
|<span data-ttu-id="e676c-132">location</span><span class="sxs-lookup"><span data-stu-id="e676c-132">location</span></span>|<span data-ttu-id="e676c-133">string</span><span class="sxs-lookup"><span data-stu-id="e676c-133">string</span></span>| <span data-ttu-id="e676c-134">Расположение, подключенного к IP-адрес входа в</span><span class="sxs-lookup"><span data-stu-id="e676c-134">The location attached to the IP address of the sign-in</span></span>|
|<span data-ttu-id="e676c-135">riskEventDateTime</span><span class="sxs-lookup"><span data-stu-id="e676c-135">riskEventDateTime</span></span>|<span data-ttu-id="e676c-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e676c-136">dateTimeOffset</span></span>| <span data-ttu-id="e676c-137">Дата и время возникновения события риска</span><span class="sxs-lookup"><span data-stu-id="e676c-137">The date and time when the risk event occurred</span></span>|
|<span data-ttu-id="e676c-138">riskEventStatus</span><span class="sxs-lookup"><span data-stu-id="e676c-138">riskEventStatus</span></span>|<span data-ttu-id="e676c-139">string</span><span class="sxs-lookup"><span data-stu-id="e676c-139">string</span></span>| <span data-ttu-id="e676c-140">Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span><span class="sxs-lookup"><span data-stu-id="e676c-140">Possible values are: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.</span></span>|
|<span data-ttu-id="e676c-141">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e676c-141">riskLevel</span></span>|<span data-ttu-id="e676c-142">string</span><span class="sxs-lookup"><span data-stu-id="e676c-142">string</span></span>| <span data-ttu-id="e676c-143">Возможные значения: `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="e676c-143">Possible values are: `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="e676c-144">riskEventType</span><span class="sxs-lookup"><span data-stu-id="e676c-144">riskEventType</span></span>|<span data-ttu-id="e676c-145">string</span><span class="sxs-lookup"><span data-stu-id="e676c-145">string</span></span>| <span data-ttu-id="e676c-146">Тип риска</span><span class="sxs-lookup"><span data-stu-id="e676c-146">The type of risk</span></span>|
|<span data-ttu-id="e676c-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e676c-147">userDisplayName</span></span>|<span data-ttu-id="e676c-148">string</span><span class="sxs-lookup"><span data-stu-id="e676c-148">string</span></span>| <span data-ttu-id="e676c-149">Имя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="e676c-149">The name of the user at risk</span></span>|
|<span data-ttu-id="e676c-150">userId</span><span class="sxs-lookup"><span data-stu-id="e676c-150">userId</span></span>|<span data-ttu-id="e676c-151">string</span><span class="sxs-lookup"><span data-stu-id="e676c-151">string</span></span>| <span data-ttu-id="e676c-152">Идентификатор пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="e676c-152">The id of the user at risk</span></span>|
|<span data-ttu-id="e676c-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e676c-153">userPrincipalName</span></span>|<span data-ttu-id="e676c-154">string</span><span class="sxs-lookup"><span data-stu-id="e676c-154">string</span></span>| <span data-ttu-id="e676c-155">Имя участника-пользователя пользователя в группу риска</span><span class="sxs-lookup"><span data-stu-id="e676c-155">The user principal name of the user at risk</span></span>|

## <a name="relationships"></a><span data-ttu-id="e676c-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="e676c-156">Relationships</span></span>
| <span data-ttu-id="e676c-157">Связь</span><span class="sxs-lookup"><span data-stu-id="e676c-157">Relationship</span></span> | <span data-ttu-id="e676c-158">Тип</span><span class="sxs-lookup"><span data-stu-id="e676c-158">Type</span></span>   |<span data-ttu-id="e676c-159">Описание</span><span class="sxs-lookup"><span data-stu-id="e676c-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e676c-160">impactedUser</span><span class="sxs-lookup"><span data-stu-id="e676c-160">impactedUser</span></span>|[<span data-ttu-id="e676c-161">user</span><span class="sxs-lookup"><span data-stu-id="e676c-161">user</span></span>](user.md)| <span data-ttu-id="e676c-p104">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="e676c-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e676c-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e676c-164">JSON representation</span></span>

<span data-ttu-id="e676c-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e676c-165">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/anonymousipriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
