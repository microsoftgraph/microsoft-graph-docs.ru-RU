---
title: Тип ресурса riskyUsers
description: Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 927e4eb519f8a849ac2cb259bed962bad44d9a6d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563184"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="c6a23-105">Тип ресурса riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c6a23-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6a23-106">Представляет пользователей Azure AD, которые находятся под угрозой.</span><span class="sxs-lookup"><span data-stu-id="c6a23-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="c6a23-107">Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="c6a23-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="c6a23-108">Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c6a23-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="c6a23-109">Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="c6a23-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="c6a23-110">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="c6a23-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="c6a23-111">Методы</span><span class="sxs-lookup"><span data-stu-id="c6a23-111">Methods</span></span>

| <span data-ttu-id="c6a23-112">Метод</span><span class="sxs-lookup"><span data-stu-id="c6a23-112">Method</span></span>   | <span data-ttu-id="c6a23-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c6a23-113">Return Type</span></span>|<span data-ttu-id="c6a23-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c6a23-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c6a23-115">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c6a23-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="c6a23-116">Коллекция [рискюсер](riskyUser.md)</span><span class="sxs-lookup"><span data-stu-id="c6a23-116">[riskyUser](riskyUser.md) collection</span></span>|<span data-ttu-id="c6a23-117">Список рискованных пользователей и их свойств.</span><span class="sxs-lookup"><span data-stu-id="c6a23-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="c6a23-118">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="c6a23-118">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="c6a23-119">Рискюсер</span><span class="sxs-lookup"><span data-stu-id="c6a23-119">riskyUser</span></span>](riskyUser.md)|<span data-ttu-id="c6a23-120">Получение определенного опасного пользователя и его свойств.</span><span class="sxs-lookup"><span data-stu-id="c6a23-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="c6a23-121">Подтверждение riskyUsers скомпрометированных атак</span><span class="sxs-lookup"><span data-stu-id="c6a23-121">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="c6a23-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c6a23-122">None</span></span> |<span data-ttu-id="c6a23-123">Подтвердите опасного пользователя в качестве скомпрометированного.</span><span class="sxs-lookup"><span data-stu-id="c6a23-123">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="c6a23-124">ОтКлонить riskyUsers</span><span class="sxs-lookup"><span data-stu-id="c6a23-124">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="c6a23-125">Нет</span><span class="sxs-lookup"><span data-stu-id="c6a23-125">None</span></span> | <span data-ttu-id="c6a23-126">ОтКлонить риск опасного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6a23-126">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6a23-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6a23-127">Properties</span></span>

| <span data-ttu-id="c6a23-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6a23-128">Property</span></span>   | <span data-ttu-id="c6a23-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c6a23-129">Type</span></span>|<span data-ttu-id="c6a23-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c6a23-130">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="c6a23-131">Уникальный идентификатор пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="c6a23-131">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="c6a23-132">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="c6a23-132">Indicates whether the user is deleted.</span></span> <span data-ttu-id="c6a23-133">Возможные значения: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="c6a23-133">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="c6a23-134">Указывает, является ли пользователь гостямй.</span><span class="sxs-lookup"><span data-stu-id="c6a23-134">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="c6a23-135">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="c6a23-135">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="c6a23-136">Имеет значение true, если удостоверение пользователя находится вне клиента.</span><span class="sxs-lookup"><span data-stu-id="c6a23-136">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="c6a23-137">Это может быть B2B или пользователь B2C с удостоверением в Azure AD, MSA или сторонним поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="c6a23-137">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="c6a23-138">False, если удостоверение пользователя находится внутри клиента в данный момент</span><span class="sxs-lookup"><span data-stu-id="c6a23-138">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="c6a23-139">Указывает, вехсер ли опасное состояние пользователя при обработке внутренней</span><span class="sxs-lookup"><span data-stu-id="c6a23-139">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="c6a23-140">Дата и время последнего обновления рискованного пользователя</span><span class="sxs-lookup"><span data-stu-id="c6a23-140">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="c6a23-141">Возможные значения: "минимум", "средний", "высокий", "скрытый", "нет", unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="c6a23-141">Possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="c6a23-142">Возможные значения: None, Конфирмедсафе, remediateо, Атриск, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="c6a23-142">Possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="c6a23-143">Возможные значения: None, Админженератедтемпорарипассворд, Усерперформедсекуредпассвордчанже, Усерперформедсекуредпассвордресет, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, Админдисмисседаллрискфорусер, Админконфирмедсигнинкомпромисед, Hidden, Админконфирмедусеркомпромисед, unknownFutureValue.</span><span class="sxs-lookup"><span data-stu-id="c6a23-143">Possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="c6a23-144">Опасное отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="c6a23-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="c6a23-145">Рискованное имя участника пользователя</span><span class="sxs-lookup"><span data-stu-id="c6a23-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6a23-146">Связи</span><span class="sxs-lookup"><span data-stu-id="c6a23-146">Relationships</span></span>
| <span data-ttu-id="c6a23-147">Отношение</span><span class="sxs-lookup"><span data-stu-id="c6a23-147">Relationship</span></span> | <span data-ttu-id="c6a23-148">Тип</span><span class="sxs-lookup"><span data-stu-id="c6a23-148">Type</span></span>   |<span data-ttu-id="c6a23-149">Описание</span><span class="sxs-lookup"><span data-stu-id="c6a23-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6a23-150">лист</span><span class="sxs-lookup"><span data-stu-id="c6a23-150">history</span></span>|<span data-ttu-id="c6a23-151">Коллекция [рискюсерхисторитем](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c6a23-151">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>| |

## <a name="json-representation"></a><span data-ttu-id="c6a23-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6a23-152">JSON representation</span></span>

<span data-ttu-id="c6a23-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6a23-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
