---
title: Тип ресурса riskyUsers
description: Представляет пользователей Azure AD, в группу риска. Постоянно Azure AD выполнена оценка риска пользователя на основе различных сигналы и машинного обучения. Этот интерфейс API позволяет получать доступ ко всем пользователям под риском в Azure AD.
author: cloudhandler
ms.openlocfilehash: bc8b64b93662511fffe709a18fb3e7210f3a941b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748264"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="d426c-105">Тип ресурса riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d426c-105">riskyUsers resource type</span></span>

> <span data-ttu-id="d426c-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d426c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d426c-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d426c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d426c-108">Представляет пользователей Azure AD, в группу риска.</span><span class="sxs-lookup"><span data-stu-id="d426c-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="d426c-109">Постоянно Azure AD выполнена оценка риска пользователя на основе различных сигналы и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="d426c-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="d426c-110">Этот интерфейс API позволяет получать доступ ко всем пользователям под риском в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d426c-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="d426c-111">**Примечание:** Этот интерфейс API требуется лицензия на P2 Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="d426c-111">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="d426c-112">Дополнительные сведения о событиях риска можно [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="d426c-112">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="d426c-113">Методы</span><span class="sxs-lookup"><span data-stu-id="d426c-113">Methods</span></span>

| <span data-ttu-id="d426c-114">Метод</span><span class="sxs-lookup"><span data-stu-id="d426c-114">Method</span></span>   | <span data-ttu-id="d426c-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d426c-115">Return Type</span></span>|<span data-ttu-id="d426c-116">Описание</span><span class="sxs-lookup"><span data-stu-id="d426c-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d426c-117">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d426c-117">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="d426c-118">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d426c-118">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="d426c-119">Список рискованный пользователей и их свойства.</span><span class="sxs-lookup"><span data-stu-id="d426c-119">List risky users and their properties.</span></span>|
|[<span data-ttu-id="d426c-120">Получение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d426c-120">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="d426c-121">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="d426c-121">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="d426c-122">Получите определенного пользователя рискованный и его свойства.</span><span class="sxs-lookup"><span data-stu-id="d426c-122">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="d426c-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="d426c-123">Properties</span></span>

| <span data-ttu-id="d426c-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="d426c-124">Property</span></span>   | <span data-ttu-id="d426c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="d426c-125">Type</span></span>|<span data-ttu-id="d426c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d426c-126">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="d426c-127">Уникальный идентификатор пользователя, под угрозой</span><span class="sxs-lookup"><span data-stu-id="d426c-127">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="d426c-128">Указывает, является ли пользователь удаляется.</span><span class="sxs-lookup"><span data-stu-id="d426c-128">Indicates whether the user is deleted.</span></span> <span data-ttu-id="d426c-129">Возможные значения: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="d426c-129">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="d426c-130">Указывает, является ли пользователь Гость.</span><span class="sxs-lookup"><span data-stu-id="d426c-130">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="d426c-131">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="d426c-131">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="d426c-132">Значение true, если удостоверение пользователя находится за пределами клиента в расчет.</span><span class="sxs-lookup"><span data-stu-id="d426c-132">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="d426c-133">Этот пользователь может быть B2B или B2C пользователя с удостоверением в Azure AD, MSA или стороннего поставщика удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d426c-133">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="d426c-134">False, если удостоверение пользователя размещен внутри клиента в расчет</span><span class="sxs-lookup"><span data-stu-id="d426c-134">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="d426c-135">Предоставляет «причина» за с определенным состоянием рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="d426c-135">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="d426c-136">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d426c-136">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="d426c-137">Значение `none` означает, что никакие действия не выполнены на пользователя или входа в данный момент.</span><span class="sxs-lookup"><span data-stu-id="d426c-137">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="d426c-138">Предоставляет общий уровень риска рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="d426c-138">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="d426c-139">Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d426c-139">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="d426c-140">Значение `hidden` означает, что пользователь или входа в не был включен для защиты удостоверения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d426c-140">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="d426c-141">Предоставляет «состояние риска» рискованный пользователя, входа или события риска.</span><span class="sxs-lookup"><span data-stu-id="d426c-141">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="d426c-142">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d426c-142">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="d426c-143">Дата и время последнего обновления рискованный пользователя</span><span class="sxs-lookup"><span data-stu-id="d426c-143">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="d426c-144">Отображаемое имя рискованный пользователя</span><span class="sxs-lookup"><span data-stu-id="d426c-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="d426c-145">Имя участника-пользователя рискующий</span><span class="sxs-lookup"><span data-stu-id="d426c-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="d426c-146">Связи</span><span class="sxs-lookup"><span data-stu-id="d426c-146">Relationships</span></span>

| <span data-ttu-id="d426c-147">Связь</span><span class="sxs-lookup"><span data-stu-id="d426c-147">Relationship</span></span> | <span data-ttu-id="d426c-148">Тип</span><span class="sxs-lookup"><span data-stu-id="d426c-148">Type</span></span> |<span data-ttu-id="d426c-149">Описание</span><span class="sxs-lookup"><span data-stu-id="d426c-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d426c-150">id</span><span class="sxs-lookup"><span data-stu-id="d426c-150">id</span></span>|<span data-ttu-id="d426c-151">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="d426c-151">UserObjectId</span></span>| <span data-ttu-id="d426c-152">Уникальный идентификатор пользователя, с которым связано событие данного риска с.</span><span class="sxs-lookup"><span data-stu-id="d426c-152">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="d426c-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="d426c-153">isGuest</span></span>|<span data-ttu-id="d426c-154">isGuest</span><span class="sxs-lookup"><span data-stu-id="d426c-154">isGuest</span></span>| <span data-ttu-id="d426c-155">Рискованный пользователя может быть Домашняя страница пользователя (B2E) или Гость (B2B, B2C).</span><span class="sxs-lookup"><span data-stu-id="d426c-155">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="d426c-156">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d426c-156">isDeleted</span></span>|<span data-ttu-id="d426c-157">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d426c-157">isDeleted</span></span>| <span data-ttu-id="d426c-158">Пользователь может или не может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="d426c-158">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="d426c-159">riskState</span><span class="sxs-lookup"><span data-stu-id="d426c-159">riskState</span></span>|<span data-ttu-id="d426c-160">riskState</span><span class="sxs-lookup"><span data-stu-id="d426c-160">riskState</span></span>| <span data-ttu-id="d426c-161">Рискованный пользователя может присутствовать в одном из нескольких состояний.</span><span class="sxs-lookup"><span data-stu-id="d426c-161">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="d426c-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="d426c-162">riskDetail</span></span>|<span data-ttu-id="d426c-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="d426c-163">riskDetail</span></span>| <span data-ttu-id="d426c-164">Рискованный пользователь сможет в определенном состоянии нескольким причинам.</span><span class="sxs-lookup"><span data-stu-id="d426c-164">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="d426c-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="d426c-165">riskLevel</span></span>|<span data-ttu-id="d426c-166">riskLevel</span><span class="sxs-lookup"><span data-stu-id="d426c-166">riskLevel</span></span>| <span data-ttu-id="d426c-167">Рискованный пользователь может рассматриваться как один из нескольких уровней риска.</span><span class="sxs-lookup"><span data-stu-id="d426c-167">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d426c-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d426c-168">JSON representation</span></span>

<span data-ttu-id="d426c-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d426c-169">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
