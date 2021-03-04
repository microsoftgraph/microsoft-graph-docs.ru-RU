---
title: тип ресурса riskyUser
description: Представляет пользователей Azure AD, которые находятся в опасности. Azure AD непрерывно оценивает риски пользователей на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям в Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9a234bc4c84ed6acc569f98c8c9b5d475a5b56be
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442861"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="f7ff4-105">тип ресурса riskyUser</span><span class="sxs-lookup"><span data-stu-id="f7ff4-105">riskyUser resource type</span></span>

<span data-ttu-id="f7ff4-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7ff4-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7ff4-107">Представляет пользователей Azure AD, которые находятся в опасности.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="f7ff4-108">Azure AD непрерывно оценивает риски пользователей на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="f7ff4-109">Этот API предоставляет программный доступ ко всем пользователям в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="f7ff4-110">Дополнительные сведения о событиях с рисками см. в [видеоролике Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="f7ff4-110">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="f7ff4-111">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="f7ff4-112">Методы</span><span class="sxs-lookup"><span data-stu-id="f7ff4-112">Methods</span></span>

| <span data-ttu-id="f7ff4-113">Метод</span><span class="sxs-lookup"><span data-stu-id="f7ff4-113">Method</span></span>   | <span data-ttu-id="f7ff4-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7ff4-114">Return Type</span></span>|<span data-ttu-id="f7ff4-115">Описание</span><span class="sxs-lookup"><span data-stu-id="f7ff4-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f7ff4-116">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="f7ff4-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="f7ff4-117">[коллекция riskyUser](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="f7ff4-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="f7ff4-118">Список рискованных пользователей и их свойств.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="f7ff4-119">Get riskyUser</span><span class="sxs-lookup"><span data-stu-id="f7ff4-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="f7ff4-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="f7ff4-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="f7ff4-121">Получите определенного рискованного пользователя и его свойства.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="f7ff4-122">История списка</span><span class="sxs-lookup"><span data-stu-id="f7ff4-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="f7ff4-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="f7ff4-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="f7ff4-124">Получите историю рисков пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="f7ff4-125">Подтверждение скомпрометации riskyUsers</span><span class="sxs-lookup"><span data-stu-id="f7ff4-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="f7ff4-126">Нет</span><span class="sxs-lookup"><span data-stu-id="f7ff4-126">None</span></span> |<span data-ttu-id="f7ff4-127">Подтвердит риск пользователя как скомпрометированного.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="f7ff4-128">Увольнение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="f7ff4-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="f7ff4-129">Нет</span><span class="sxs-lookup"><span data-stu-id="f7ff4-129">None</span></span> | <span data-ttu-id="f7ff4-130">Отклонять риск рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="f7ff4-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7ff4-131">Properties</span></span>

| <span data-ttu-id="f7ff4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7ff4-132">Property</span></span>   | <span data-ttu-id="f7ff4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="f7ff4-133">Type</span></span>|<span data-ttu-id="f7ff4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="f7ff4-134">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="f7ff4-135">Уникальный ID пользователя в опасности.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-135">Unique ID of the user at risk.</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="f7ff4-136">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-136">Indicates whether the user is deleted.</span></span> <span data-ttu-id="f7ff4-137">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-137">Possible values are: `true`, `false`.</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="f7ff4-138">Указывает, обрабатывается ли приложением рискованное состояние пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-138">Indicates whether a user's risky state is being processed by the backend.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="f7ff4-139">Дата и время последнего обновления рискованного пользователя</span><span class="sxs-lookup"><span data-stu-id="f7ff4-139">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="f7ff4-140">Возможные значения : низкие, средние, высокие, скрытые, неизвестные.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-140">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="f7ff4-141">Возможные значения не являются никакими, подтвержденнымиSafe, исправленными, atRisk, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-141">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="f7ff4-142">Возможные значения не являются никакими, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-142">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="f7ff4-143">Рискованное имя отображения пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-143">Risky user display name.</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="f7ff4-144">Рискованное основное имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-144">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7ff4-145">Связи</span><span class="sxs-lookup"><span data-stu-id="f7ff4-145">Relationships</span></span>

<span data-ttu-id="f7ff4-146">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7ff4-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f7ff4-147">JSON representation</span></span>

<span data-ttu-id="f7ff4-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7ff4-148">The following is a JSON representation of the resource.</span></span>

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
