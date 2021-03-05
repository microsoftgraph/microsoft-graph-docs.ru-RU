---
title: тип ресурса riskyUser
description: элемент рискованных пользователей
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 00a284f4a3592ccf378e0e6f218c56902c219d51
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448993"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="5bf19-103">тип ресурса riskyUser</span><span class="sxs-lookup"><span data-stu-id="5bf19-103">riskyUser resource type</span></span>

<span data-ttu-id="5bf19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bf19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5bf19-105">Представляет пользователей Azure AD, которые находятся в опасности.</span><span class="sxs-lookup"><span data-stu-id="5bf19-105">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="5bf19-106">Azure AD непрерывно оценивает риски пользователей на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="5bf19-106">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="5bf19-107">Этот API предоставляет программный доступ ко всем пользователям в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5bf19-107">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="5bf19-108">Дополнительные сведения о событиях с рисками см. в [видеоролике Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="5bf19-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="5bf19-109">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="5bf19-109">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="5bf19-110">Методы</span><span class="sxs-lookup"><span data-stu-id="5bf19-110">Methods</span></span>
|<span data-ttu-id="5bf19-111">Метод</span><span class="sxs-lookup"><span data-stu-id="5bf19-111">Method</span></span>|<span data-ttu-id="5bf19-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="5bf19-112">Return type</span></span>|<span data-ttu-id="5bf19-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5bf19-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5bf19-114">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="5bf19-114">List riskyUsers</span></span>](../api/riskyuser-list.md)|<span data-ttu-id="5bf19-115">[коллекция riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5bf19-115">[riskyUser](../resources/riskyuser.md) collection</span></span>|<span data-ttu-id="5bf19-116">Получите список объектов **riskyUser** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="5bf19-116">Get a list of the **riskyUser** objects and their properties.</span></span>|
|[<span data-ttu-id="5bf19-117">Get riskyUser</span><span class="sxs-lookup"><span data-stu-id="5bf19-117">Get riskyUser</span></span>](../api/riskyuser-get.md)|[<span data-ttu-id="5bf19-118">riskyUser</span><span class="sxs-lookup"><span data-stu-id="5bf19-118">riskyUser</span></span>](../resources/riskyuser.md)|<span data-ttu-id="5bf19-119">Ознакомьтесь с свойствами и отношениями объекта **riskyUser.**</span><span class="sxs-lookup"><span data-stu-id="5bf19-119">Read the properties and relationships of a **riskyUser** object.</span></span>|
|[<span data-ttu-id="5bf19-120">Отклонение riskyUser</span><span class="sxs-lookup"><span data-stu-id="5bf19-120">Dismiss a riskyUser</span></span>](../api/riskyuser-dismiss.md)|<span data-ttu-id="5bf19-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5bf19-121">None</span></span>|<span data-ttu-id="5bf19-122">Отклонять риск одного или более **объектов riskyUser.**</span><span class="sxs-lookup"><span data-stu-id="5bf19-122">Dismiss the risk of one or more **riskyUser** objects.</span></span> |
|[<span data-ttu-id="5bf19-123">Подтверждение riskyUser как скомпрометированного</span><span class="sxs-lookup"><span data-stu-id="5bf19-123">Confirm a riskyUser as compromised</span></span>](../api/riskyuser-confirmcompromised.md)|<span data-ttu-id="5bf19-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5bf19-124">None</span></span>|<span data-ttu-id="5bf19-125">Подтвердим, что один или несколько **объектов riskyUser** могут быть скомпрометированы.</span><span class="sxs-lookup"><span data-stu-id="5bf19-125">Confirm one or more **riskyUser** objects as compromised.</span></span>|
|[<span data-ttu-id="5bf19-126">История списка</span><span class="sxs-lookup"><span data-stu-id="5bf19-126">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="5bf19-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="5bf19-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="5bf19-128">Получите **свойство riskyUserHistoryItems из** свойства навигации по истории.</span><span class="sxs-lookup"><span data-stu-id="5bf19-128">Get the **riskyUserHistoryItems** from the history navigation property.</span></span>|
|[<span data-ttu-id="5bf19-129">Получить историю</span><span class="sxs-lookup"><span data-stu-id="5bf19-129">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="5bf19-130">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="5bf19-130">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="5bf19-131">Ознакомьтесь с свойствами и отношениями объекта [riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5bf19-131">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="5bf19-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bf19-132">Properties</span></span>
|<span data-ttu-id="5bf19-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bf19-133">Property</span></span>|<span data-ttu-id="5bf19-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5bf19-134">Type</span></span>|<span data-ttu-id="5bf19-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5bf19-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bf19-136">id</span><span class="sxs-lookup"><span data-stu-id="5bf19-136">id</span></span>|<span data-ttu-id="5bf19-137">String</span><span class="sxs-lookup"><span data-stu-id="5bf19-137">String</span></span>|<span data-ttu-id="5bf19-138">Уникальный ID пользователя в опасности.</span><span class="sxs-lookup"><span data-stu-id="5bf19-138">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="5bf19-139">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5bf19-139">isDeleted</span></span>|<span data-ttu-id="5bf19-140">Логический</span><span class="sxs-lookup"><span data-stu-id="5bf19-140">Boolean</span></span>|<span data-ttu-id="5bf19-141">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="5bf19-141">Indicates whether the user is deleted.</span></span> <span data-ttu-id="5bf19-142">Возможные значения: `true` , `false`</span><span class="sxs-lookup"><span data-stu-id="5bf19-142">Possible values are: `true`, `false`</span></span>|
|<span data-ttu-id="5bf19-143">isProcessing</span><span class="sxs-lookup"><span data-stu-id="5bf19-143">isProcessing</span></span>|<span data-ttu-id="5bf19-144">Логический</span><span class="sxs-lookup"><span data-stu-id="5bf19-144">Boolean</span></span>|<span data-ttu-id="5bf19-145">Указывает, что рискованное состояние пользователя обрабатывается backend</span><span class="sxs-lookup"><span data-stu-id="5bf19-145">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|<span data-ttu-id="5bf19-146">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5bf19-146">riskDetail</span></span>|<span data-ttu-id="5bf19-147">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5bf19-147">riskDetail</span></span>|<span data-ttu-id="5bf19-148">Сведения об обнаружении риска.</span><span class="sxs-lookup"><span data-stu-id="5bf19-148">Details of the detected risk.</span></span> <span data-ttu-id="5bf19-149">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5bf19-149">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5bf19-150">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5bf19-150">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="5bf19-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5bf19-151">DateTimeOffset</span></span>|<span data-ttu-id="5bf19-152">Дата и время последнего обновления рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bf19-152">The date and time that the risky user was last updated.</span></span>|
|<span data-ttu-id="5bf19-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5bf19-153">riskLevel</span></span>|<span data-ttu-id="5bf19-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5bf19-154">riskLevel</span></span>|<span data-ttu-id="5bf19-155">Уровень обнаруженного рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bf19-155">Level of the detected risky user.</span></span> <span data-ttu-id="5bf19-156">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5bf19-156">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5bf19-157">riskState</span><span class="sxs-lookup"><span data-stu-id="5bf19-157">riskState</span></span>|<span data-ttu-id="5bf19-158">riskState</span><span class="sxs-lookup"><span data-stu-id="5bf19-158">riskState</span></span>|<span data-ttu-id="5bf19-159">Состояние риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bf19-159">State of the user's risk.</span></span> <span data-ttu-id="5bf19-160">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5bf19-160">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5bf19-161">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5bf19-161">userDisplayName</span></span>|<span data-ttu-id="5bf19-162">String</span><span class="sxs-lookup"><span data-stu-id="5bf19-162">String</span></span>|<span data-ttu-id="5bf19-163">Рискованное имя отображения пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bf19-163">Risky user display name.</span></span>|
|<span data-ttu-id="5bf19-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5bf19-164">userPrincipalName</span></span>|<span data-ttu-id="5bf19-165">String</span><span class="sxs-lookup"><span data-stu-id="5bf19-165">String</span></span>|<span data-ttu-id="5bf19-166">Рискованное основное имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="5bf19-166">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5bf19-167">Связи</span><span class="sxs-lookup"><span data-stu-id="5bf19-167">Relationships</span></span>
|<span data-ttu-id="5bf19-168">Связь</span><span class="sxs-lookup"><span data-stu-id="5bf19-168">Relationship</span></span>|<span data-ttu-id="5bf19-169">Тип</span><span class="sxs-lookup"><span data-stu-id="5bf19-169">Type</span></span>|<span data-ttu-id="5bf19-170">Описание</span><span class="sxs-lookup"><span data-stu-id="5bf19-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bf19-171">история</span><span class="sxs-lookup"><span data-stu-id="5bf19-171">history</span></span>|<span data-ttu-id="5bf19-172">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="5bf19-172">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|   <span data-ttu-id="5bf19-173">Действие, связанное с изменением уровня риска пользователя</span><span class="sxs-lookup"><span data-stu-id="5bf19-173">The activity related to user risk level change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bf19-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bf19-174">JSON representation</span></span>
<span data-ttu-id="5bf19-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bf19-175">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
