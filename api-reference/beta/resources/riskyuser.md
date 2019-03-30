---
title: Тип ресурса riskyUsers
description: Представляет пользователей Azure AD, которые находятся под угрозой. Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения. Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3265ea40903ca2c5c10272f5df280bd3715af366
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/30/2019
ms.locfileid: "31003722"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="178bd-105">Тип ресурса riskyUsers</span><span class="sxs-lookup"><span data-stu-id="178bd-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="178bd-106">Представляет пользователей Azure AD, которые находятся под угрозой.</span><span class="sxs-lookup"><span data-stu-id="178bd-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="178bd-107">Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="178bd-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="178bd-108">Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="178bd-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="178bd-109">Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="178bd-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="178bd-110">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="178bd-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="178bd-111">Методы</span><span class="sxs-lookup"><span data-stu-id="178bd-111">Methods</span></span>

| <span data-ttu-id="178bd-112">Метод</span><span class="sxs-lookup"><span data-stu-id="178bd-112">Method</span></span>   | <span data-ttu-id="178bd-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="178bd-113">Return Type</span></span>|<span data-ttu-id="178bd-114">Описание</span><span class="sxs-lookup"><span data-stu-id="178bd-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="178bd-115">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="178bd-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="178bd-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="178bd-116">riskyUsers</span></span>](riskyUser.md) |<span data-ttu-id="178bd-117">Список рискованных пользователей и их свойств.</span><span class="sxs-lookup"><span data-stu-id="178bd-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="178bd-118">Получение riskyUsers</span><span class="sxs-lookup"><span data-stu-id="178bd-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="178bd-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="178bd-119">riskyUsers</span></span>](riskyUser.md)|<span data-ttu-id="178bd-120">Получение определенного опасного пользователя и его свойств.</span><span class="sxs-lookup"><span data-stu-id="178bd-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="178bd-121">Подтверждение riskyUsers скомпрометированных атак</span><span class="sxs-lookup"><span data-stu-id="178bd-121">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="178bd-122">Подтвердите опасного пользователя в качестве скомпрометированного.</span><span class="sxs-lookup"><span data-stu-id="178bd-122">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="178bd-123">ОтКлонить riskyUsers</span><span class="sxs-lookup"><span data-stu-id="178bd-123">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="178bd-124">ОтКлонить риск опасного пользователя.</span><span class="sxs-lookup"><span data-stu-id="178bd-124">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="178bd-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="178bd-125">Properties</span></span>

| <span data-ttu-id="178bd-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="178bd-126">Property</span></span>   | <span data-ttu-id="178bd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="178bd-127">Type</span></span>|<span data-ttu-id="178bd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="178bd-128">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="178bd-129">Уникальный идентификатор пользователя под угрозой</span><span class="sxs-lookup"><span data-stu-id="178bd-129">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="178bd-130">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="178bd-130">Indicates whether the user is deleted.</span></span> <span data-ttu-id="178bd-131">Возможные значения: `true`,`false`</span><span class="sxs-lookup"><span data-stu-id="178bd-131">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="178bd-132">Указывает, является ли пользователь гостямй.</span><span class="sxs-lookup"><span data-stu-id="178bd-132">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="178bd-133">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="178bd-133">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="178bd-134">Имеет значение true, если удостоверение пользователя находится вне клиента.</span><span class="sxs-lookup"><span data-stu-id="178bd-134">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="178bd-135">Это может быть B2B или пользователь B2C с удостоверением в Azure AD, MSA или сторонним поставщиком удостоверений.</span><span class="sxs-lookup"><span data-stu-id="178bd-135">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="178bd-136">False, если удостоверение пользователя находится внутри клиента в данный момент</span><span class="sxs-lookup"><span data-stu-id="178bd-136">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="178bd-137">Указывает, вехсер ли опасное состояние пользователя при обработке внутренней</span><span class="sxs-lookup"><span data-stu-id="178bd-137">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`risk`|[<span data-ttu-id="178bd-138">особой</span><span class="sxs-lookup"><span data-stu-id="178bd-138">risk</span></span>](risk.md)|<span data-ttu-id="178bd-139">Опасное состояние пользователя</span><span class="sxs-lookup"><span data-stu-id="178bd-139">Risky user state</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="178bd-140">Дата и время последнего обновления рискованного пользователя</span><span class="sxs-lookup"><span data-stu-id="178bd-140">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="178bd-141">Опасное отображаемое имя пользователя</span><span class="sxs-lookup"><span data-stu-id="178bd-141">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="178bd-142">Рискованное имя участника пользователя</span><span class="sxs-lookup"><span data-stu-id="178bd-142">Risky user principal name</span></span>|


## <a name="json-representation"></a><span data-ttu-id="178bd-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="178bd-143">JSON representation</span></span>

<span data-ttu-id="178bd-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="178bd-144">Here is a JSON representation of the resource.</span></span>

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
"isProcessing": "boolean",
"isDeleted": "boolean",
"risk": {"@odata.type": "microsoft.graph.risk"},
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
