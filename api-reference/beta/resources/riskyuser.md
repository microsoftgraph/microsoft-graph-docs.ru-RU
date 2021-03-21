---
title: тип ресурса riskyUser
description: Представляет пользователей Azure AD, которые находятся в опасности. Azure AD непрерывно оценивает риски пользователей на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям в Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: d2e0942e92b1dcd648812503a923dac51a640be1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960329"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="5108e-105">тип ресурса riskyUser</span><span class="sxs-lookup"><span data-stu-id="5108e-105">riskyUser resource type</span></span>

<span data-ttu-id="5108e-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5108e-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5108e-107">Представляет пользователей Azure AD, которые находятся в опасности.</span><span class="sxs-lookup"><span data-stu-id="5108e-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="5108e-108">Azure AD непрерывно оценивает риски пользователей на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="5108e-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="5108e-109">Этот API предоставляет программный доступ ко всем пользователям в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5108e-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="5108e-110">Дополнительные сведения о событиях с рисками см. в [видеоролике Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="5108e-110">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="5108e-111">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="5108e-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="5108e-112">Методы</span><span class="sxs-lookup"><span data-stu-id="5108e-112">Methods</span></span>

| <span data-ttu-id="5108e-113">Метод</span><span class="sxs-lookup"><span data-stu-id="5108e-113">Method</span></span>   | <span data-ttu-id="5108e-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5108e-114">Return Type</span></span>|<span data-ttu-id="5108e-115">Описание</span><span class="sxs-lookup"><span data-stu-id="5108e-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5108e-116">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="5108e-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="5108e-117">[коллекция riskyUser](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5108e-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="5108e-118">Список рискованных пользователей и их свойств.</span><span class="sxs-lookup"><span data-stu-id="5108e-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="5108e-119">Get riskyUser</span><span class="sxs-lookup"><span data-stu-id="5108e-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="5108e-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="5108e-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="5108e-121">Получите определенного рискованного пользователя и его свойства.</span><span class="sxs-lookup"><span data-stu-id="5108e-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="5108e-122">История списка</span><span class="sxs-lookup"><span data-stu-id="5108e-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="5108e-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="5108e-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="5108e-124">Получите историю рисков пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5108e-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="5108e-125">Подтверждение скомпрометации riskyUsers</span><span class="sxs-lookup"><span data-stu-id="5108e-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="5108e-126">Нет</span><span class="sxs-lookup"><span data-stu-id="5108e-126">None</span></span> |<span data-ttu-id="5108e-127">Подтвердит риск пользователя как скомпрометированного.</span><span class="sxs-lookup"><span data-stu-id="5108e-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="5108e-128">Увольнение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="5108e-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="5108e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="5108e-129">None</span></span> | <span data-ttu-id="5108e-130">Отклонять риск рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5108e-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="5108e-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="5108e-131">Properties</span></span>

| <span data-ttu-id="5108e-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="5108e-132">Property</span></span>   | <span data-ttu-id="5108e-133">Тип</span><span class="sxs-lookup"><span data-stu-id="5108e-133">Type</span></span>|<span data-ttu-id="5108e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5108e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5108e-135">id</span><span class="sxs-lookup"><span data-stu-id="5108e-135">id</span></span>|<span data-ttu-id="5108e-136">string</span><span class="sxs-lookup"><span data-stu-id="5108e-136">string</span></span>|<span data-ttu-id="5108e-137">Уникальный ID пользователя в опасности.</span><span class="sxs-lookup"><span data-stu-id="5108e-137">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="5108e-138">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5108e-138">isDeleted</span></span>|<span data-ttu-id="5108e-139">boolean</span><span class="sxs-lookup"><span data-stu-id="5108e-139">boolean</span></span>|<span data-ttu-id="5108e-140">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="5108e-140">Indicates whether the user is deleted.</span></span> <span data-ttu-id="5108e-141">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="5108e-141">Possible values are: `true`, `false`.</span></span>|
|<span data-ttu-id="5108e-142">isProcessing</span><span class="sxs-lookup"><span data-stu-id="5108e-142">isProcessing</span></span>|<span data-ttu-id="5108e-143">boolean</span><span class="sxs-lookup"><span data-stu-id="5108e-143">boolean</span></span>|<span data-ttu-id="5108e-144">Указывает, обрабатывается ли приложением рискованное состояние пользователя.</span><span class="sxs-lookup"><span data-stu-id="5108e-144">Indicates whether a user's risky state is being processed by the backend.</span></span>|
|<span data-ttu-id="5108e-145">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5108e-145">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="5108e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5108e-146">DateTimeOffset</span></span>|<span data-ttu-id="5108e-147">Дата и время последнего обновления рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5108e-147">The date and time that the risky user was last updated.</span></span>  <span data-ttu-id="5108e-148">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="5108e-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5108e-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5108e-149">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5108e-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5108e-150">riskLevel</span></span>|<span data-ttu-id="5108e-151">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5108e-151">riskLevel</span></span>| <span data-ttu-id="5108e-152">Уровень обнаруженного рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5108e-152">Level of the detected risky user.</span></span> <span data-ttu-id="5108e-153">Возможные значения `low` , `medium` `high` , , `hidden` , `none` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="5108e-153">The possible values are `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="5108e-154">riskState</span><span class="sxs-lookup"><span data-stu-id="5108e-154">riskState</span></span>|<span data-ttu-id="5108e-155">riskState</span><span class="sxs-lookup"><span data-stu-id="5108e-155">riskState</span></span>| <span data-ttu-id="5108e-156">Состояние риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="5108e-156">State of the user's risk.</span></span> <span data-ttu-id="5108e-157">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5108e-157">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="5108e-158">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5108e-158">riskDetail</span></span>|<span data-ttu-id="5108e-159">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5108e-159">riskDetail</span></span>| <span data-ttu-id="5108e-160">Возможные `none` значения: `adminGeneratedTemporaryPassword` , `userPerformedSecuredPasswordChange` , , , , `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` , `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` , .</span><span class="sxs-lookup"><span data-stu-id="5108e-160">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="5108e-161">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5108e-161">userDisplayName</span></span>|<span data-ttu-id="5108e-162">string</span><span class="sxs-lookup"><span data-stu-id="5108e-162">string</span></span>|<span data-ttu-id="5108e-163">Рискованное имя отображения пользователя.</span><span class="sxs-lookup"><span data-stu-id="5108e-163">Risky user display name.</span></span>|
|<span data-ttu-id="5108e-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5108e-164">userPrincipalName</span></span>|<span data-ttu-id="5108e-165">string</span><span class="sxs-lookup"><span data-stu-id="5108e-165">string</span></span>|<span data-ttu-id="5108e-166">Рискованное основное имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="5108e-166">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5108e-167">Связи</span><span class="sxs-lookup"><span data-stu-id="5108e-167">Relationships</span></span>

<span data-ttu-id="5108e-168">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5108e-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5108e-169">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5108e-169">JSON representation</span></span>

<span data-ttu-id="5108e-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5108e-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
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
