---
title: Тип ресурса riskyUsers
description: Представляет пользователей Azure AD, в группу риска. Постоянно Azure AD выполнена оценка риска пользователя на основе различных сигналы и машинного обучения. Этот интерфейс API позволяет получать доступ ко всем пользователям под риском в Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 27c189a81d6ba4e088c1242acfd2cf0d0f5c56c5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643911"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="b51eb-105">Тип ресурса riskyUsers</span><span class="sxs-lookup"><span data-stu-id="b51eb-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b51eb-106">Представляет пользователей Azure AD, в группу риска.</span><span class="sxs-lookup"><span data-stu-id="b51eb-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="b51eb-107">Постоянно Azure AD выполнена оценка риска пользователя на основе различных сигналы и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="b51eb-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="b51eb-108">Этот интерфейс API позволяет получать доступ ко всем пользователям под риском в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b51eb-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="b51eb-109">**Примечание:** Этот интерфейс API требуется лицензия на P2 Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="b51eb-109">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="b51eb-110">Дополнительные сведения о событиях риска можно [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="b51eb-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="b51eb-111">Методы</span><span class="sxs-lookup"><span data-stu-id="b51eb-111">Methods</span></span>

| <span data-ttu-id="b51eb-112">Метод</span><span class="sxs-lookup"><span data-stu-id="b51eb-112">Method</span></span>   | <span data-ttu-id="b51eb-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b51eb-113">Return Type</span></span>|<span data-ttu-id="b51eb-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b51eb-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b51eb-115">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="b51eb-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="b51eb-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="b51eb-116">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="b51eb-117">Список рискованный пользователей и их свойства.</span><span class="sxs-lookup"><span data-stu-id="b51eb-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="b51eb-118">Получение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="b51eb-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="b51eb-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="b51eb-119">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="b51eb-120">Получите определенного пользователя рискованный и его свойства.</span><span class="sxs-lookup"><span data-stu-id="b51eb-120">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="b51eb-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="b51eb-121">Properties</span></span>

| <span data-ttu-id="b51eb-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="b51eb-122">Property</span></span>   | <span data-ttu-id="b51eb-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b51eb-123">Type</span></span>|<span data-ttu-id="b51eb-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b51eb-124">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="b51eb-125">Уникальный идентификатор пользователя, под угрозой</span><span class="sxs-lookup"><span data-stu-id="b51eb-125">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="b51eb-126">Указывает, является ли пользователь удаляется.</span><span class="sxs-lookup"><span data-stu-id="b51eb-126">Indicates whether the user is deleted.</span></span> <span data-ttu-id="b51eb-127">Возможные значения: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="b51eb-127">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="b51eb-128">Указывает, является ли пользователь Гость.</span><span class="sxs-lookup"><span data-stu-id="b51eb-128">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="b51eb-129">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="b51eb-129">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="b51eb-130">Значение true, если удостоверение пользователя находится за пределами клиента в расчет.</span><span class="sxs-lookup"><span data-stu-id="b51eb-130">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="b51eb-131">Этот пользователь может быть B2B или B2C пользователя с удостоверением в Azure AD, MSA или стороннего поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="b51eb-131">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="b51eb-132">False, если удостоверение пользователя размещен внутри клиента в расчет</span><span class="sxs-lookup"><span data-stu-id="b51eb-132">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="b51eb-133">Предоставляет "причину" определенного состояния пользователя с риском, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="b51eb-133">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b51eb-134">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b51eb-134">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="b51eb-135">Значение `none` означает, что действия для пользователя или входа пока не выполнялись.</span><span class="sxs-lookup"><span data-stu-id="b51eb-135">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="b51eb-136">Предоставляет общий уровень риска рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="b51eb-136">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b51eb-137">Допустимые значения: `none`, `low`, `medium`, `high`, `hidden` и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b51eb-137">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="b51eb-138">Значение `hidden` означает, что пользователь или вход не разрешены в службе защиты идентификации Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b51eb-138">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="b51eb-139">Представляет "состояние риска" пользователя с риском, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="b51eb-139">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="b51eb-140">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b51eb-140">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="b51eb-141">Дата и время последнего обновления рискованный пользователя</span><span class="sxs-lookup"><span data-stu-id="b51eb-141">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="b51eb-142">Отображаемое имя рискованный пользователя</span><span class="sxs-lookup"><span data-stu-id="b51eb-142">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="b51eb-143">Имя участника-пользователя рискующий</span><span class="sxs-lookup"><span data-stu-id="b51eb-143">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="b51eb-144">Связи</span><span class="sxs-lookup"><span data-stu-id="b51eb-144">Relationships</span></span>

| <span data-ttu-id="b51eb-145">Связь</span><span class="sxs-lookup"><span data-stu-id="b51eb-145">Relationship</span></span> | <span data-ttu-id="b51eb-146">Тип</span><span class="sxs-lookup"><span data-stu-id="b51eb-146">Type</span></span> |<span data-ttu-id="b51eb-147">Описание</span><span class="sxs-lookup"><span data-stu-id="b51eb-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b51eb-148">id</span><span class="sxs-lookup"><span data-stu-id="b51eb-148">id</span></span>|<span data-ttu-id="b51eb-149">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="b51eb-149">UserObjectId</span></span>| <span data-ttu-id="b51eb-150">Уникальный идентификатор пользователя, с которым связано событие данного риска с.</span><span class="sxs-lookup"><span data-stu-id="b51eb-150">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="b51eb-151">isGuest</span><span class="sxs-lookup"><span data-stu-id="b51eb-151">isGuest</span></span>|<span data-ttu-id="b51eb-152">isGuest</span><span class="sxs-lookup"><span data-stu-id="b51eb-152">isGuest</span></span>| <span data-ttu-id="b51eb-153">Рискованный пользователя может быть Домашняя страница пользователя (B2E) или Гость (B2B, B2C).</span><span class="sxs-lookup"><span data-stu-id="b51eb-153">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="b51eb-154">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b51eb-154">isDeleted</span></span>|<span data-ttu-id="b51eb-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b51eb-155">isDeleted</span></span>| <span data-ttu-id="b51eb-156">Пользователь может или не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="b51eb-156">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="b51eb-157">riskState</span><span class="sxs-lookup"><span data-stu-id="b51eb-157">riskState</span></span>|<span data-ttu-id="b51eb-158">riskState</span><span class="sxs-lookup"><span data-stu-id="b51eb-158">riskState</span></span>| <span data-ttu-id="b51eb-159">Рискованный пользователя может присутствовать в одном из нескольких состояний.</span><span class="sxs-lookup"><span data-stu-id="b51eb-159">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="b51eb-160">riskDetail</span><span class="sxs-lookup"><span data-stu-id="b51eb-160">riskDetail</span></span>|<span data-ttu-id="b51eb-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="b51eb-161">riskDetail</span></span>| <span data-ttu-id="b51eb-162">Рискованный пользователь сможет в определенном состоянии нескольким причинам.</span><span class="sxs-lookup"><span data-stu-id="b51eb-162">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="b51eb-163">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b51eb-163">riskLevel</span></span>|<span data-ttu-id="b51eb-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b51eb-164">riskLevel</span></span>| <span data-ttu-id="b51eb-165">Рискованный пользователь может рассматриваться как один из нескольких уровней риска.</span><span class="sxs-lookup"><span data-stu-id="b51eb-165">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b51eb-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b51eb-166">JSON representation</span></span>

<span data-ttu-id="b51eb-167">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b51eb-167">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"},
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/riskyuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
