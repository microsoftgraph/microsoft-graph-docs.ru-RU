---
title: Тип ресурса Рискюсер
description: элемент рискованных пользователей
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2989b0f74243679daaebcb482c0640a78bc9effa
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581290"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="05ef1-103">Тип ресурса Рискюсер</span><span class="sxs-lookup"><span data-stu-id="05ef1-103">riskyUser resource type</span></span>

<span data-ttu-id="05ef1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05ef1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05ef1-105">Представляет пользователей Azure AD, которые находятся под угрозой.</span><span class="sxs-lookup"><span data-stu-id="05ef1-105">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="05ef1-106">Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="05ef1-106">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="05ef1-107">Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="05ef1-107">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="05ef1-108">Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection).</span><span class="sxs-lookup"><span data-stu-id="05ef1-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="05ef1-109">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="05ef1-109">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="05ef1-110">Методы</span><span class="sxs-lookup"><span data-stu-id="05ef1-110">Methods</span></span>
|<span data-ttu-id="05ef1-111">Метод</span><span class="sxs-lookup"><span data-stu-id="05ef1-111">Method</span></span>|<span data-ttu-id="05ef1-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="05ef1-112">Return type</span></span>|<span data-ttu-id="05ef1-113">Описание</span><span class="sxs-lookup"><span data-stu-id="05ef1-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="05ef1-114">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="05ef1-114">List riskyUsers</span></span>](../api/riskyuser-list.md)|<span data-ttu-id="05ef1-115">Коллекция [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="05ef1-115">[riskyUser](../resources/riskyuser.md) collection</span></span>|<span data-ttu-id="05ef1-116">Получение списка объектов **рискюсер** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="05ef1-116">Get a list of the **riskyUser** objects and their properties.</span></span>|
|[<span data-ttu-id="05ef1-117">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="05ef1-117">Get riskyUser</span></span>](../api/riskyuser-get.md)|[<span data-ttu-id="05ef1-118">рискюсер</span><span class="sxs-lookup"><span data-stu-id="05ef1-118">riskyUser</span></span>](../resources/riskyuser.md)|<span data-ttu-id="05ef1-119">Чтение свойств и связей объекта **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="05ef1-119">Read the properties and relationships of a **riskyUser** object.</span></span>|
|[<span data-ttu-id="05ef1-120">Отклонение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="05ef1-120">Dismiss a riskyUser</span></span>](../api/riskyuser-dismiss.md)|<span data-ttu-id="05ef1-121">Нет</span><span class="sxs-lookup"><span data-stu-id="05ef1-121">None</span></span>|<span data-ttu-id="05ef1-122">Отклонить риск одного или нескольких объектов **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="05ef1-122">Dismiss the risk of one or more **riskyUser** objects.</span></span> |
|[<span data-ttu-id="05ef1-123">Подтверждение Рискюсер в качестве скомпрометированного</span><span class="sxs-lookup"><span data-stu-id="05ef1-123">Confirm a riskyUser as compromised</span></span>](../api/riskyuser-confirmcompromised.md)|<span data-ttu-id="05ef1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="05ef1-124">None</span></span>|<span data-ttu-id="05ef1-125">Подтвердите, что один или несколько объектов **рискюсер** считаются скомпрометированными.</span><span class="sxs-lookup"><span data-stu-id="05ef1-125">Confirm one or more **riskyUser** objects as compromised.</span></span>|
|[<span data-ttu-id="05ef1-126">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="05ef1-126">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="05ef1-127">Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="05ef1-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="05ef1-128">Получение **рискюсерхисторитемс** из свойства навигации по журналу.</span><span class="sxs-lookup"><span data-stu-id="05ef1-128">Get the **riskyUserHistoryItems** from the history navigation property.</span></span>|
|[<span data-ttu-id="05ef1-129">Получение журнала</span><span class="sxs-lookup"><span data-stu-id="05ef1-129">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="05ef1-130">рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="05ef1-130">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="05ef1-131">Чтение свойств и связей объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="05ef1-131">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="05ef1-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="05ef1-132">Properties</span></span>
|<span data-ttu-id="05ef1-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="05ef1-133">Property</span></span>|<span data-ttu-id="05ef1-134">Тип</span><span class="sxs-lookup"><span data-stu-id="05ef1-134">Type</span></span>|<span data-ttu-id="05ef1-135">Описание</span><span class="sxs-lookup"><span data-stu-id="05ef1-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05ef1-136">id</span><span class="sxs-lookup"><span data-stu-id="05ef1-136">id</span></span>|<span data-ttu-id="05ef1-137">String</span><span class="sxs-lookup"><span data-stu-id="05ef1-137">String</span></span>|<span data-ttu-id="05ef1-138">Уникальный идентификатор пользователя под угрозой.</span><span class="sxs-lookup"><span data-stu-id="05ef1-138">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="05ef1-139">isDeleted</span><span class="sxs-lookup"><span data-stu-id="05ef1-139">isDeleted</span></span>|<span data-ttu-id="05ef1-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="05ef1-140">Boolean</span></span>|<span data-ttu-id="05ef1-141">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="05ef1-141">Indicates whether the user is deleted.</span></span> <span data-ttu-id="05ef1-142">Возможные значения: `true` , `false`</span><span class="sxs-lookup"><span data-stu-id="05ef1-142">Possible values are: `true`, `false`</span></span>|
|<span data-ttu-id="05ef1-143">Процесс обработки</span><span class="sxs-lookup"><span data-stu-id="05ef1-143">isProcessing</span></span>|<span data-ttu-id="05ef1-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="05ef1-144">Boolean</span></span>|<span data-ttu-id="05ef1-145">Указывает, вехсер ли опасное состояние пользователя при обработке внутренней</span><span class="sxs-lookup"><span data-stu-id="05ef1-145">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|<span data-ttu-id="05ef1-146">riskDetail</span><span class="sxs-lookup"><span data-stu-id="05ef1-146">riskDetail</span></span>|<span data-ttu-id="05ef1-147">riskDetail</span><span class="sxs-lookup"><span data-stu-id="05ef1-147">riskDetail</span></span>|<span data-ttu-id="05ef1-148">Сведения об обнаруженном риске.</span><span class="sxs-lookup"><span data-stu-id="05ef1-148">Details of the detected risk.</span></span> <span data-ttu-id="05ef1-149">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="05ef1-149">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="05ef1-150">рискластупдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="05ef1-150">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="05ef1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05ef1-151">DateTimeOffset</span></span>|<span data-ttu-id="05ef1-152">Дата и время последнего обновления рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="05ef1-152">The date and time that the risky user was last updated.</span></span>|
|<span data-ttu-id="05ef1-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="05ef1-153">riskLevel</span></span>|<span data-ttu-id="05ef1-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="05ef1-154">riskLevel</span></span>|<span data-ttu-id="05ef1-155">Уровень обнаруженного опасного пользователя.</span><span class="sxs-lookup"><span data-stu-id="05ef1-155">Level of the detected risky user.</span></span> <span data-ttu-id="05ef1-156">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="05ef1-156">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="05ef1-157">riskState</span><span class="sxs-lookup"><span data-stu-id="05ef1-157">riskState</span></span>|<span data-ttu-id="05ef1-158">riskState</span><span class="sxs-lookup"><span data-stu-id="05ef1-158">riskState</span></span>|<span data-ttu-id="05ef1-159">Состояние риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="05ef1-159">State of the user's risk.</span></span> <span data-ttu-id="05ef1-160">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="05ef1-160">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="05ef1-161">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="05ef1-161">userDisplayName</span></span>|<span data-ttu-id="05ef1-162">String</span><span class="sxs-lookup"><span data-stu-id="05ef1-162">String</span></span>|<span data-ttu-id="05ef1-163">Опасное отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="05ef1-163">Risky user display name.</span></span>|
|<span data-ttu-id="05ef1-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05ef1-164">userPrincipalName</span></span>|<span data-ttu-id="05ef1-165">String</span><span class="sxs-lookup"><span data-stu-id="05ef1-165">String</span></span>|<span data-ttu-id="05ef1-166">Опасное имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="05ef1-166">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05ef1-167">Связи</span><span class="sxs-lookup"><span data-stu-id="05ef1-167">Relationships</span></span>
|<span data-ttu-id="05ef1-168">Связь</span><span class="sxs-lookup"><span data-stu-id="05ef1-168">Relationship</span></span>|<span data-ttu-id="05ef1-169">Тип</span><span class="sxs-lookup"><span data-stu-id="05ef1-169">Type</span></span>|<span data-ttu-id="05ef1-170">Описание</span><span class="sxs-lookup"><span data-stu-id="05ef1-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05ef1-171">лист</span><span class="sxs-lookup"><span data-stu-id="05ef1-171">history</span></span>|<span data-ttu-id="05ef1-172">Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="05ef1-172">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|   <span data-ttu-id="05ef1-173">Действие, связанное с изменением уровня риска пользователя</span><span class="sxs-lookup"><span data-stu-id="05ef1-173">The activity related to user risk level change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05ef1-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05ef1-174">JSON representation</span></span>
<span data-ttu-id="05ef1-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05ef1-175">The following is a JSON representation of the resource.</span></span>
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