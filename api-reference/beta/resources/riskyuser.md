---
title: Тип ресурса riskyUsers
description: Представляет пользователей Azure AD, в группу риска. Постоянно Azure AD выполнена оценка риска пользователя на основе различных сигналы и машинного обучения. Этот интерфейс API позволяет получать доступ ко всем пользователям под риском в Azure AD.
ms.openlocfilehash: 5d51c303d25a781f8e432badb42acb48cf135217
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076634"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="37d44-105">Тип ресурса riskyUsers</span><span class="sxs-lookup"><span data-stu-id="37d44-105">riskyUsers resource type</span></span>

> <span data-ttu-id="37d44-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37d44-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37d44-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37d44-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37d44-108">Представляет пользователей Azure AD, в группу риска.</span><span class="sxs-lookup"><span data-stu-id="37d44-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="37d44-109">Постоянно Azure AD выполнена оценка риска пользователя на основе различных сигналы и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="37d44-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="37d44-110">Этот интерфейс API позволяет получать доступ ко всем пользователям под риском в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37d44-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="37d44-111">Дополнительные сведения о событиях риска можно [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="37d44-111">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="37d44-112">Методы</span><span class="sxs-lookup"><span data-stu-id="37d44-112">Methods</span></span>

| <span data-ttu-id="37d44-113">Метод</span><span class="sxs-lookup"><span data-stu-id="37d44-113">Method</span></span>   | <span data-ttu-id="37d44-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="37d44-114">Return Type</span></span>|<span data-ttu-id="37d44-115">Описание</span><span class="sxs-lookup"><span data-stu-id="37d44-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37d44-116">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="37d44-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="37d44-117">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="37d44-117">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="37d44-118">Список рискованный пользователей и их свойства.</span><span class="sxs-lookup"><span data-stu-id="37d44-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="37d44-119">Получение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="37d44-119">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="37d44-120">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="37d44-120">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="37d44-121">Получите определенного пользователя рискованный и его свойства.</span><span class="sxs-lookup"><span data-stu-id="37d44-121">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="37d44-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="37d44-122">Properties</span></span>

| <span data-ttu-id="37d44-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="37d44-123">Property</span></span>   | <span data-ttu-id="37d44-124">Тип</span><span class="sxs-lookup"><span data-stu-id="37d44-124">Type</span></span>|<span data-ttu-id="37d44-125">Description</span><span class="sxs-lookup"><span data-stu-id="37d44-125">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="37d44-126">Уникальный идентификатор пользователя, под угрозой</span><span class="sxs-lookup"><span data-stu-id="37d44-126">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="37d44-127">Указывает, является ли пользователь удаляется.</span><span class="sxs-lookup"><span data-stu-id="37d44-127">Indicates whether the user is deleted.</span></span> <span data-ttu-id="37d44-128">Возможные значения: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="37d44-128">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="37d44-129">Указывает, является ли пользователь Гость.</span><span class="sxs-lookup"><span data-stu-id="37d44-129">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="37d44-130">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="37d44-130">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="37d44-131">Значение true, если удостоверение пользователя находится за пределами клиента в расчет.</span><span class="sxs-lookup"><span data-stu-id="37d44-131">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="37d44-132">Этот пользователь может быть B2B или B2C пользователя с удостоверением в Azure AD, MSA или стороннего поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="37d44-132">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="37d44-133">False, если удостоверение пользователя размещен внутри клиента в расчет</span><span class="sxs-lookup"><span data-stu-id="37d44-133">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="37d44-134">Предоставляет «причина» за с определенным состоянием рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="37d44-134">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="37d44-135">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="37d44-135">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="37d44-136">Значение `none` означает, что никакие действия не выполнены на пользователя или входа в данный момент.</span><span class="sxs-lookup"><span data-stu-id="37d44-136">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="37d44-137">Предоставляет общий уровень риска рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="37d44-137">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="37d44-138">Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="37d44-138">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="37d44-139">Значение `hidden` означает, что пользователь или входа в не был включен для защиты удостоверения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37d44-139">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="37d44-140">Предоставляет «состояние риска» рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="37d44-140">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="37d44-141">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="37d44-141">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="37d44-142">Дата и время последнего обновления рискованный пользователя</span><span class="sxs-lookup"><span data-stu-id="37d44-142">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="37d44-143">Отображаемое имя рискованный пользователя</span><span class="sxs-lookup"><span data-stu-id="37d44-143">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="37d44-144">Имя участника-пользователя рискующий</span><span class="sxs-lookup"><span data-stu-id="37d44-144">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="37d44-145">Связи</span><span class="sxs-lookup"><span data-stu-id="37d44-145">Relationships</span></span>

| <span data-ttu-id="37d44-146">Связь</span><span class="sxs-lookup"><span data-stu-id="37d44-146">Relationship</span></span> | <span data-ttu-id="37d44-147">Тип</span><span class="sxs-lookup"><span data-stu-id="37d44-147">Type</span></span> |<span data-ttu-id="37d44-148">Описание</span><span class="sxs-lookup"><span data-stu-id="37d44-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37d44-149">id</span><span class="sxs-lookup"><span data-stu-id="37d44-149">id</span></span>|<span data-ttu-id="37d44-150">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="37d44-150">UserObjectId</span></span>| <span data-ttu-id="37d44-151">Уникальный идентификатор пользователя, с которым связано событие данного риска с.</span><span class="sxs-lookup"><span data-stu-id="37d44-151">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="37d44-152">isGuest</span><span class="sxs-lookup"><span data-stu-id="37d44-152">isGuest</span></span>|<span data-ttu-id="37d44-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="37d44-153">isGuest</span></span>| <span data-ttu-id="37d44-154">Рискованный пользователя может быть Домашняя страница пользователя (B2E) или Гость (B2B, B2C).</span><span class="sxs-lookup"><span data-stu-id="37d44-154">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="37d44-155">isDeleted</span><span class="sxs-lookup"><span data-stu-id="37d44-155">isDeleted</span></span>|<span data-ttu-id="37d44-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="37d44-156">isDeleted</span></span>| <span data-ttu-id="37d44-157">Пользователь может или не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="37d44-157">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="37d44-158">riskState</span><span class="sxs-lookup"><span data-stu-id="37d44-158">riskState</span></span>|<span data-ttu-id="37d44-159">riskState</span><span class="sxs-lookup"><span data-stu-id="37d44-159">riskState</span></span>| <span data-ttu-id="37d44-160">Рискованный пользователя может присутствовать в одном из нескольких состояний.</span><span class="sxs-lookup"><span data-stu-id="37d44-160">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="37d44-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="37d44-161">riskDetail</span></span>|<span data-ttu-id="37d44-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="37d44-162">riskDetail</span></span>| <span data-ttu-id="37d44-163">Рискованный пользователь сможет в определенном состоянии нескольким причинам.</span><span class="sxs-lookup"><span data-stu-id="37d44-163">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="37d44-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="37d44-164">riskLevel</span></span>|<span data-ttu-id="37d44-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="37d44-165">riskLevel</span></span>| <span data-ttu-id="37d44-166">Рискованный пользователь может рассматриваться как один из нескольких уровней риска.</span><span class="sxs-lookup"><span data-stu-id="37d44-166">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="37d44-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37d44-167">JSON representation</span></span>

<span data-ttu-id="37d44-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37d44-168">Here is a JSON representation of the resource.</span></span>

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
"riskState":  {"@odata.type": "microsoft.graph.riskState"}
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
