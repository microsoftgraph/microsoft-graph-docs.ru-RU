---
title: Тип ресурса Рискюсер
description: Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3548be0439eaa5335d710a35f51fdbaecb19060c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008728"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="24cb1-105">Тип ресурса Рискюсер</span><span class="sxs-lookup"><span data-stu-id="24cb1-105">riskyUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24cb1-106">Представляет пользователей Azure AD, которые находятся под угрозой.</span><span class="sxs-lookup"><span data-stu-id="24cb1-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="24cb1-107">Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="24cb1-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="24cb1-108">Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24cb1-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="24cb1-109">Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="24cb1-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="24cb1-110">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="24cb1-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="24cb1-111">Методы</span><span class="sxs-lookup"><span data-stu-id="24cb1-111">Methods</span></span>

| <span data-ttu-id="24cb1-112">Метод</span><span class="sxs-lookup"><span data-stu-id="24cb1-112">Method</span></span>   | <span data-ttu-id="24cb1-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="24cb1-113">Return Type</span></span>|<span data-ttu-id="24cb1-114">Описание</span><span class="sxs-lookup"><span data-stu-id="24cb1-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="24cb1-115">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="24cb1-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="24cb1-116">Коллекция [рискюсер](riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="24cb1-116">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="24cb1-117">Список рискованных пользователей и их свойств.</span><span class="sxs-lookup"><span data-stu-id="24cb1-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="24cb1-118">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="24cb1-118">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="24cb1-119">Рискюсер</span><span class="sxs-lookup"><span data-stu-id="24cb1-119">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="24cb1-120">Получение определенного опасного пользователя и его свойств.</span><span class="sxs-lookup"><span data-stu-id="24cb1-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="24cb1-121">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="24cb1-121">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="24cb1-122">Коллекция [рискюсерхисторитем](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="24cb1-122">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="24cb1-123">Получение журнала рисков пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24cb1-123">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="24cb1-124">Подтверждение riskyUsers скомпрометированных атак</span><span class="sxs-lookup"><span data-stu-id="24cb1-124">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="24cb1-125">Нет</span><span class="sxs-lookup"><span data-stu-id="24cb1-125">None</span></span> |<span data-ttu-id="24cb1-126">Подтвердите опасного пользователя в качестве скомпрометированного.</span><span class="sxs-lookup"><span data-stu-id="24cb1-126">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="24cb1-127">Отклонить riskyUsers</span><span class="sxs-lookup"><span data-stu-id="24cb1-127">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="24cb1-128">Нет</span><span class="sxs-lookup"><span data-stu-id="24cb1-128">None</span></span> | <span data-ttu-id="24cb1-129">Отклонить риск опасного пользователя.</span><span class="sxs-lookup"><span data-stu-id="24cb1-129">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="24cb1-130">Свойства</span><span class="sxs-lookup"><span data-stu-id="24cb1-130">Properties</span></span>

| <span data-ttu-id="24cb1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="24cb1-131">Property</span></span>   | <span data-ttu-id="24cb1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="24cb1-132">Type</span></span>|<span data-ttu-id="24cb1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="24cb1-133">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="24cb1-134">Уникальный идентификатор пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="24cb1-134">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="24cb1-135">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="24cb1-135">Indicates whether the user is deleted.</span></span> <span data-ttu-id="24cb1-136">Возможные значения: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="24cb1-136">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="24cb1-137">Указывает, является ли пользователь гостямй.</span><span class="sxs-lookup"><span data-stu-id="24cb1-137">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="24cb1-138">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="24cb1-138">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="24cb1-139">Имеет значение true, если удостоверение пользователя находится вне клиента.</span><span class="sxs-lookup"><span data-stu-id="24cb1-139">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="24cb1-140">Это может быть B2B или пользователь B2C с удостоверением в Azure AD, MSA или сторонним поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="24cb1-140">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="24cb1-141">False, если удостоверение пользователя находится внутри клиента в данный момент</span><span class="sxs-lookup"><span data-stu-id="24cb1-141">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="24cb1-142">Указывает, вехсер ли опасное состояние пользователя при обработке внутренней</span><span class="sxs-lookup"><span data-stu-id="24cb1-142">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="24cb1-143">Дата и время последнего обновления рискованного пользователя</span><span class="sxs-lookup"><span data-stu-id="24cb1-143">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="24cb1-144">Возможные значения: "минимум", "средний", "высокий", "скрытый", "нет", unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="24cb1-144">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="24cb1-145">Возможные значения: None, Конфирмедсафе, remediateо, Атриск, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="24cb1-145">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="24cb1-146">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="24cb1-146">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="24cb1-147">Опасное отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="24cb1-147">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="24cb1-148">Рискованное имя участника пользователя</span><span class="sxs-lookup"><span data-stu-id="24cb1-148">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="24cb1-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="24cb1-149">Relationships</span></span>
| <span data-ttu-id="24cb1-150">Отношение</span><span class="sxs-lookup"><span data-stu-id="24cb1-150">Relationship</span></span> | <span data-ttu-id="24cb1-151">Тип</span><span class="sxs-lookup"><span data-stu-id="24cb1-151">Type</span></span>   |<span data-ttu-id="24cb1-152">Описание</span><span class="sxs-lookup"><span data-stu-id="24cb1-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24cb1-153">лист</span><span class="sxs-lookup"><span data-stu-id="24cb1-153">history</span></span>|<span data-ttu-id="24cb1-154">Коллекция [рискюсерхисторитем](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="24cb1-154">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="24cb1-155">Представляет историю риска пользователя Azure AD, определенная службой защиты удостоверений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24cb1-155">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24cb1-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24cb1-156">JSON representation</span></span>

<span data-ttu-id="24cb1-157">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24cb1-157">Here is a JSON representation of the resource.</span></span>

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
