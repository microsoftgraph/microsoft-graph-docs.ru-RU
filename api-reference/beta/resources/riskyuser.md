---
title: Тип ресурса Рискюсер
description: Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7759a9c42ca9178dc95266ffa4630ef891832ecd
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062639"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="82476-105">Тип ресурса Рискюсер</span><span class="sxs-lookup"><span data-stu-id="82476-105">riskyUser resource type</span></span>

<span data-ttu-id="82476-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82476-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82476-107">Представляет пользователей Azure AD, которые находятся под угрозой.</span><span class="sxs-lookup"><span data-stu-id="82476-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="82476-108">Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="82476-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="82476-109">Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82476-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="82476-110">Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="82476-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="82476-111">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="82476-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="82476-112">Методы</span><span class="sxs-lookup"><span data-stu-id="82476-112">Methods</span></span>

| <span data-ttu-id="82476-113">Метод</span><span class="sxs-lookup"><span data-stu-id="82476-113">Method</span></span>   | <span data-ttu-id="82476-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="82476-114">Return Type</span></span>|<span data-ttu-id="82476-115">Описание</span><span class="sxs-lookup"><span data-stu-id="82476-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82476-116">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="82476-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="82476-117">Коллекция [рискюсер](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="82476-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="82476-118">Список рискованных пользователей и их свойств.</span><span class="sxs-lookup"><span data-stu-id="82476-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="82476-119">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="82476-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="82476-120">рискюсер</span><span class="sxs-lookup"><span data-stu-id="82476-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="82476-121">Получение определенного опасного пользователя и его свойств.</span><span class="sxs-lookup"><span data-stu-id="82476-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="82476-122">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="82476-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="82476-123">Коллекция [рискюсерхисторитем](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="82476-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="82476-124">Получение журнала рисков пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82476-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="82476-125">Подтверждение riskyUsers скомпрометированных атак</span><span class="sxs-lookup"><span data-stu-id="82476-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="82476-126">Нет</span><span class="sxs-lookup"><span data-stu-id="82476-126">None</span></span> |<span data-ttu-id="82476-127">Подтвердите опасного пользователя в качестве скомпрометированного.</span><span class="sxs-lookup"><span data-stu-id="82476-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="82476-128">Отклонить riskyUsers</span><span class="sxs-lookup"><span data-stu-id="82476-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="82476-129">Нет</span><span class="sxs-lookup"><span data-stu-id="82476-129">None</span></span> | <span data-ttu-id="82476-130">Отклонить риск опасного пользователя.</span><span class="sxs-lookup"><span data-stu-id="82476-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="82476-131">Свойства</span><span class="sxs-lookup"><span data-stu-id="82476-131">Properties</span></span>

| <span data-ttu-id="82476-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="82476-132">Property</span></span>   | <span data-ttu-id="82476-133">Тип</span><span class="sxs-lookup"><span data-stu-id="82476-133">Type</span></span>|<span data-ttu-id="82476-134">Описание</span><span class="sxs-lookup"><span data-stu-id="82476-134">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="82476-135">Уникальный идентификатор пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="82476-135">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="82476-136">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="82476-136">Indicates whether the user is deleted.</span></span> <span data-ttu-id="82476-137">Возможные значения: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="82476-137">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="82476-138">Указывает, является ли пользователь гостямй.</span><span class="sxs-lookup"><span data-stu-id="82476-138">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="82476-139">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="82476-139">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="82476-140">Имеет значение true, если удостоверение пользователя находится вне клиента.</span><span class="sxs-lookup"><span data-stu-id="82476-140">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="82476-141">Это может быть B2B или пользователь B2C с удостоверением в Azure AD, MSA или сторонним поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="82476-141">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="82476-142">False, если удостоверение пользователя находится внутри клиента в данный момент</span><span class="sxs-lookup"><span data-stu-id="82476-142">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="82476-143">Указывает, вехсер ли опасное состояние пользователя при обработке внутренней</span><span class="sxs-lookup"><span data-stu-id="82476-143">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="82476-144">Дата и время последнего обновления рискованного пользователя</span><span class="sxs-lookup"><span data-stu-id="82476-144">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="82476-145">Возможные значения: "минимум", "средний", "высокий", "скрытый", "нет", unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="82476-145">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="82476-146">Возможные значения: None, Конфирмедсафе, remediateо, Атриск, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="82476-146">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="82476-147">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="82476-147">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="82476-148">Опасное отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="82476-148">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="82476-149">Рискованное имя участника пользователя</span><span class="sxs-lookup"><span data-stu-id="82476-149">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="82476-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="82476-150">Relationships</span></span>

<span data-ttu-id="82476-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="82476-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82476-152">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="82476-152">JSON representation</span></span>

<span data-ttu-id="82476-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82476-153">The following is a JSON representation of the resource.</span></span>

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
"isGuest": "boolean",
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
