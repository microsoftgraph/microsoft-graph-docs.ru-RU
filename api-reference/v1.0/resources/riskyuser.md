---
title: тип ресурса riskyUser
description: элемент рискованных пользователей
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 82b622838ddd5e7fb8c00a969184bdd729926b23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961085"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="f4fda-103">тип ресурса riskyUser</span><span class="sxs-lookup"><span data-stu-id="f4fda-103">riskyUser resource type</span></span>

<span data-ttu-id="f4fda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4fda-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4fda-105">Представляет пользователей Azure AD, которые находятся в опасности.</span><span class="sxs-lookup"><span data-stu-id="f4fda-105">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="f4fda-106">Azure AD непрерывно оценивает риски пользователей на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="f4fda-106">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="f4fda-107">Этот API предоставляет программный доступ ко всем пользователям в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f4fda-107">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="f4fda-108">Дополнительные сведения о событиях с рисками см. в [видеоролике Azure Active Directory Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="f4fda-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="f4fda-109">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="f4fda-109">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="f4fda-110">Методы</span><span class="sxs-lookup"><span data-stu-id="f4fda-110">Methods</span></span>
|<span data-ttu-id="f4fda-111">Метод</span><span class="sxs-lookup"><span data-stu-id="f4fda-111">Method</span></span>|<span data-ttu-id="f4fda-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="f4fda-112">Return type</span></span>|<span data-ttu-id="f4fda-113">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fda-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4fda-114">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="f4fda-114">List riskyUsers</span></span>](../api/riskyuser-list.md)|<span data-ttu-id="f4fda-115">[коллекция riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="f4fda-115">[riskyUser](../resources/riskyuser.md) collection</span></span>|<span data-ttu-id="f4fda-116">Получите список объектов **riskyUser** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="f4fda-116">Get a list of the **riskyUser** objects and their properties.</span></span>|
|[<span data-ttu-id="f4fda-117">Get riskyUser</span><span class="sxs-lookup"><span data-stu-id="f4fda-117">Get riskyUser</span></span>](../api/riskyuser-get.md)|[<span data-ttu-id="f4fda-118">riskyUser</span><span class="sxs-lookup"><span data-stu-id="f4fda-118">riskyUser</span></span>](../resources/riskyuser.md)|<span data-ttu-id="f4fda-119">Ознакомьтесь с свойствами и отношениями объекта **riskyUser.**</span><span class="sxs-lookup"><span data-stu-id="f4fda-119">Read the properties and relationships of a **riskyUser** object.</span></span>|
|[<span data-ttu-id="f4fda-120">Отклонение riskyUser</span><span class="sxs-lookup"><span data-stu-id="f4fda-120">Dismiss a riskyUser</span></span>](../api/riskyuser-dismiss.md)|<span data-ttu-id="f4fda-121">Нет</span><span class="sxs-lookup"><span data-stu-id="f4fda-121">None</span></span>|<span data-ttu-id="f4fda-122">Отклонять риск одного или более **объектов riskyUser.**</span><span class="sxs-lookup"><span data-stu-id="f4fda-122">Dismiss the risk of one or more **riskyUser** objects.</span></span> |
|[<span data-ttu-id="f4fda-123">Подтверждение riskyUser как скомпрометированного</span><span class="sxs-lookup"><span data-stu-id="f4fda-123">Confirm a riskyUser as compromised</span></span>](../api/riskyuser-confirmcompromised.md)|<span data-ttu-id="f4fda-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f4fda-124">None</span></span>|<span data-ttu-id="f4fda-125">Подтвердим, что один или несколько **объектов riskyUser** могут быть скомпрометированы.</span><span class="sxs-lookup"><span data-stu-id="f4fda-125">Confirm one or more **riskyUser** objects as compromised.</span></span>|
|[<span data-ttu-id="f4fda-126">История списка</span><span class="sxs-lookup"><span data-stu-id="f4fda-126">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="f4fda-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="f4fda-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="f4fda-128">Получите **свойство riskyUserHistoryItems из** свойства навигации по истории.</span><span class="sxs-lookup"><span data-stu-id="f4fda-128">Get the **riskyUserHistoryItems** from the history navigation property.</span></span>|
|[<span data-ttu-id="f4fda-129">Получить историю</span><span class="sxs-lookup"><span data-stu-id="f4fda-129">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="f4fda-130">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="f4fda-130">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="f4fda-131">Ознакомьтесь с свойствами и отношениями объекта [riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f4fda-131">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="f4fda-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4fda-132">Properties</span></span>
|<span data-ttu-id="f4fda-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4fda-133">Property</span></span>|<span data-ttu-id="f4fda-134">Тип</span><span class="sxs-lookup"><span data-stu-id="f4fda-134">Type</span></span>|<span data-ttu-id="f4fda-135">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fda-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4fda-136">id</span><span class="sxs-lookup"><span data-stu-id="f4fda-136">id</span></span>|<span data-ttu-id="f4fda-137">String</span><span class="sxs-lookup"><span data-stu-id="f4fda-137">String</span></span>|<span data-ttu-id="f4fda-138">Уникальный ID пользователя в опасности.</span><span class="sxs-lookup"><span data-stu-id="f4fda-138">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="f4fda-139">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f4fda-139">isDeleted</span></span>|<span data-ttu-id="f4fda-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4fda-140">Boolean</span></span>|<span data-ttu-id="f4fda-141">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="f4fda-141">Indicates whether the user is deleted.</span></span> <span data-ttu-id="f4fda-142">Возможные значения: `true`, `false`.</span><span class="sxs-lookup"><span data-stu-id="f4fda-142">Possible values are: `true`, `false`.</span></span>|
|<span data-ttu-id="f4fda-143">isProcessing</span><span class="sxs-lookup"><span data-stu-id="f4fda-143">isProcessing</span></span>|<span data-ttu-id="f4fda-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4fda-144">Boolean</span></span>|<span data-ttu-id="f4fda-145">Указывает, обрабатывается ли приложением рискованное состояние пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4fda-145">Indicates whether a user's risky state is being processed by the backend.</span></span>|
|<span data-ttu-id="f4fda-146">riskDetail</span><span class="sxs-lookup"><span data-stu-id="f4fda-146">riskDetail</span></span>|<span data-ttu-id="f4fda-147">riskDetail</span><span class="sxs-lookup"><span data-stu-id="f4fda-147">riskDetail</span></span>|<span data-ttu-id="f4fda-148">Сведения об обнаружении риска.</span><span class="sxs-lookup"><span data-stu-id="f4fda-148">Details of the detected risk.</span></span> <span data-ttu-id="f4fda-149">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f4fda-149">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f4fda-150">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4fda-150">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="f4fda-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4fda-151">DateTimeOffset</span></span>|<span data-ttu-id="f4fda-152">Дата и время последнего обновления рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4fda-152">The date and time that the risky user was last updated.</span></span>  <span data-ttu-id="f4fda-153">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="f4fda-153">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4fda-154">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f4fda-154">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f4fda-155">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f4fda-155">riskLevel</span></span>|<span data-ttu-id="f4fda-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f4fda-156">riskLevel</span></span>|<span data-ttu-id="f4fda-157">Уровень обнаруженного рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4fda-157">Level of the detected risky user.</span></span> <span data-ttu-id="f4fda-158">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f4fda-158">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f4fda-159">riskState</span><span class="sxs-lookup"><span data-stu-id="f4fda-159">riskState</span></span>|<span data-ttu-id="f4fda-160">riskState</span><span class="sxs-lookup"><span data-stu-id="f4fda-160">riskState</span></span>|<span data-ttu-id="f4fda-161">Состояние риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4fda-161">State of the user's risk.</span></span> <span data-ttu-id="f4fda-162">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f4fda-162">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f4fda-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4fda-163">userDisplayName</span></span>|<span data-ttu-id="f4fda-164">String</span><span class="sxs-lookup"><span data-stu-id="f4fda-164">String</span></span>|<span data-ttu-id="f4fda-165">Рискованное имя отображения пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4fda-165">Risky user display name.</span></span>|
|<span data-ttu-id="f4fda-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4fda-166">userPrincipalName</span></span>|<span data-ttu-id="f4fda-167">String</span><span class="sxs-lookup"><span data-stu-id="f4fda-167">String</span></span>|<span data-ttu-id="f4fda-168">Рискованное основное имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="f4fda-168">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4fda-169">Связи</span><span class="sxs-lookup"><span data-stu-id="f4fda-169">Relationships</span></span>
|<span data-ttu-id="f4fda-170">Связь</span><span class="sxs-lookup"><span data-stu-id="f4fda-170">Relationship</span></span>|<span data-ttu-id="f4fda-171">Тип</span><span class="sxs-lookup"><span data-stu-id="f4fda-171">Type</span></span>|<span data-ttu-id="f4fda-172">Описание</span><span class="sxs-lookup"><span data-stu-id="f4fda-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4fda-173">история</span><span class="sxs-lookup"><span data-stu-id="f4fda-173">history</span></span>|<span data-ttu-id="f4fda-174">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="f4fda-174">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|   <span data-ttu-id="f4fda-175">Действие, связанное с изменением уровня риска пользователя</span><span class="sxs-lookup"><span data-stu-id="f4fda-175">The activity related to user risk level change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4fda-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4fda-176">JSON representation</span></span>
<span data-ttu-id="f4fda-177">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4fda-177">The following is a JSON representation of the resource.</span></span>
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
