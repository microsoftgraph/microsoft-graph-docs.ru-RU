---
title: тип ресурса riskyUser
description: Представляет учетную запись, помеченную для риска для каждого управляемого клиента.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3f66998080abcf9580cdd36e0f3e4b24edab2d2d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403165"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="ca9e8-103">тип ресурса riskyUser</span><span class="sxs-lookup"><span data-stu-id="ca9e8-103">riskyUser resource type</span></span>

<span data-ttu-id="ca9e8-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ca9e8-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca9e8-105">Представляет учетную запись, помеченную для риска для каждого управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-105">Represents an account flagged for risk across each managed tenants.</span></span>

## <a name="methods"></a><span data-ttu-id="ca9e8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="ca9e8-106">Methods</span></span>
|<span data-ttu-id="ca9e8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="ca9e8-107">Method</span></span>|<span data-ttu-id="ca9e8-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="ca9e8-108">Return type</span></span>|<span data-ttu-id="ca9e8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ca9e8-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ca9e8-110">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="ca9e8-110">List riskyUsers</span></span>](../api/managedtenants-managedtenant-list-riskyusers.md)|<span data-ttu-id="ca9e8-111">[коллекция microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="ca9e8-111">[microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md) collection</span></span>|<span data-ttu-id="ca9e8-112">Получите список объектов [riskyUser](../resources/managedtenants-riskyuser.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-112">Get a list of the [riskyUser](../resources/managedtenants-riskyuser.md) objects and their properties.</span></span>|
|[<span data-ttu-id="ca9e8-113">Get riskyUser</span><span class="sxs-lookup"><span data-stu-id="ca9e8-113">Get riskyUser</span></span>](../api/managedtenants-riskyuser-get.md)|[<span data-ttu-id="ca9e8-114">microsoft.graph.managedTenants.riskyUser</span><span class="sxs-lookup"><span data-stu-id="ca9e8-114">microsoft.graph.managedTenants.riskyUser</span></span>](../resources/managedtenants-riskyuser.md)|<span data-ttu-id="ca9e8-115">Ознакомьтесь с свойствами и отношениями объекта [riskyUser.](../resources/managedtenants-riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="ca9e8-115">Read the properties and relationships of a [riskyUser](../resources/managedtenants-riskyuser.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca9e8-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca9e8-116">Properties</span></span>
|<span data-ttu-id="ca9e8-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca9e8-117">Property</span></span>|<span data-ttu-id="ca9e8-118">Тип</span><span class="sxs-lookup"><span data-stu-id="ca9e8-118">Type</span></span>|<span data-ttu-id="ca9e8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ca9e8-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca9e8-120">id</span><span class="sxs-lookup"><span data-stu-id="ca9e8-120">id</span></span>|<span data-ttu-id="ca9e8-121">String</span><span class="sxs-lookup"><span data-stu-id="ca9e8-121">String</span></span>|<span data-ttu-id="ca9e8-122">Уникальный идентификатор для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-122">The unique identifier for this entity.</span></span> <span data-ttu-id="ca9e8-123">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-123">Required.</span></span> <span data-ttu-id="ca9e8-124">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-124">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-125">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ca9e8-125">isDeleted</span></span>|<span data-ttu-id="ca9e8-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca9e8-126">Boolean</span></span>|<span data-ttu-id="ca9e8-127">Флаг, указывающий, удалена ли учетная запись.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-127">A flag indicating whether the account has been deleted.</span></span> <span data-ttu-id="ca9e8-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-128">Optional.</span></span> <span data-ttu-id="ca9e8-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-129">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-130">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca9e8-130">lastRefreshedDateTime</span></span>|<span data-ttu-id="ca9e8-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca9e8-131">DateTimeOffset</span></span>|<span data-ttu-id="ca9e8-132">Дата и время последнего обновления объекта на платформе управления с несколькими клиентами.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-132">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="ca9e8-133">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-133">Optional.</span></span> <span data-ttu-id="ca9e8-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-134">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-135">riskDetail</span><span class="sxs-lookup"><span data-stu-id="ca9e8-135">riskDetail</span></span>|<span data-ttu-id="ca9e8-136">String</span><span class="sxs-lookup"><span data-stu-id="ca9e8-136">String</span></span>|<span data-ttu-id="ca9e8-137">Сведения о рисках для учетной записи, помеченной для риска.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-137">The risk details for the account flagged for risk.</span></span> <span data-ttu-id="ca9e8-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-138">Optional.</span></span> <span data-ttu-id="ca9e8-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-139">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca9e8-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="ca9e8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca9e8-141">DateTimeOffset</span></span>|<span data-ttu-id="ca9e8-142">Дата и время последнего обновления сведений о рисках.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-142">The date and time when the risk information was last updated.</span></span> <span data-ttu-id="ca9e8-143">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-143">Optional.</span></span> <span data-ttu-id="ca9e8-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-144">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-145">riskLevel</span><span class="sxs-lookup"><span data-stu-id="ca9e8-145">riskLevel</span></span>|<span data-ttu-id="ca9e8-146">String</span><span class="sxs-lookup"><span data-stu-id="ca9e8-146">String</span></span>|<span data-ttu-id="ca9e8-147">Уровень риска, который был обнаружен.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-147">The level of risk that was detected.</span></span> <span data-ttu-id="ca9e8-148">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-148">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span> <span data-ttu-id="ca9e8-149">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-149">Optional.</span></span> <span data-ttu-id="ca9e8-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-150">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-151">riskState</span><span class="sxs-lookup"><span data-stu-id="ca9e8-151">riskState</span></span>|<span data-ttu-id="ca9e8-152">String</span><span class="sxs-lookup"><span data-stu-id="ca9e8-152">String</span></span>|<span data-ttu-id="ca9e8-153">Обнаружено состояние риска.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-153">The state of risk that was detected.</span></span> <span data-ttu-id="ca9e8-154">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-154">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="ca9e8-155">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-155">Optional.</span></span> <span data-ttu-id="ca9e8-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-156">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-157">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="ca9e8-157">tenantDisplayName</span></span>|<span data-ttu-id="ca9e8-158">String</span><span class="sxs-lookup"><span data-stu-id="ca9e8-158">String</span></span>|<span data-ttu-id="ca9e8-159">Имя отображения управляемого клиента.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-159">The display name for the managed tenant.</span></span> <span data-ttu-id="ca9e8-160">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-160">Optional.</span></span> <span data-ttu-id="ca9e8-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-161">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-162">tenantId</span><span class="sxs-lookup"><span data-stu-id="ca9e8-162">tenantId</span></span>|<span data-ttu-id="ca9e8-163">String</span><span class="sxs-lookup"><span data-stu-id="ca9e8-163">String</span></span>|<span data-ttu-id="ca9e8-164">Идентификатор Azure Active Directory клиента для [управляемого клиента.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="ca9e8-164">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="ca9e8-165">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-165">Required.</span></span> <span data-ttu-id="ca9e8-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-166">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-167">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ca9e8-167">userDisplayName</span></span>|<span data-ttu-id="ca9e8-168">String</span><span class="sxs-lookup"><span data-stu-id="ca9e8-168">String</span></span>|<span data-ttu-id="ca9e8-169">Имя отображения учетной записи, в которой был обнаружен риск.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-169">The display name for the account where risk was detected.</span></span> <span data-ttu-id="ca9e8-170">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-170">Optional.</span></span> <span data-ttu-id="ca9e8-171">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-171">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-172">userId</span><span class="sxs-lookup"><span data-stu-id="ca9e8-172">userId</span></span>|<span data-ttu-id="ca9e8-173">String</span><span class="sxs-lookup"><span data-stu-id="ca9e8-173">String</span></span>|<span data-ttu-id="ca9e8-174">Идентификатор учетной записи пользователя, в которой был обнаружен риск.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-174">The identifier for the user account where risk was detected.</span></span> <span data-ttu-id="ca9e8-175">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-175">Required.</span></span> <span data-ttu-id="ca9e8-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-176">Read-only.</span></span>|
|<span data-ttu-id="ca9e8-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ca9e8-177">userPrincipalName</span></span>|<span data-ttu-id="ca9e8-178">String</span><span class="sxs-lookup"><span data-stu-id="ca9e8-178">String</span></span>|<span data-ttu-id="ca9e8-179">Основное имя пользователя (UPN) для учетной записи, где был обнаружен риск.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-179">The user principal name (UPN) for the account where risk was detected.</span></span> <span data-ttu-id="ca9e8-180">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-180">Optional.</span></span> <span data-ttu-id="ca9e8-181">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-181">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca9e8-182">Связи</span><span class="sxs-lookup"><span data-stu-id="ca9e8-182">Relationships</span></span>
<span data-ttu-id="ca9e8-183">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-183">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca9e8-184">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ca9e8-184">JSON representation</span></span>
<span data-ttu-id="ca9e8-185">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca9e8-185">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.riskyUser",
  "id": "String (identifier)",
  "userId": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "isDeleted": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
