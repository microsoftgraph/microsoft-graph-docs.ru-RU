---
title: Тип ресурса Рискюсер
description: элемент рискованных пользователей
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2810ffc35b1550ae75a21b5f8baebb91c444799f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984189"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="a854a-103">Тип ресурса Рискюсер</span><span class="sxs-lookup"><span data-stu-id="a854a-103">riskyUser resource type</span></span>

<span data-ttu-id="a854a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a854a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a854a-105">Представляет пользователей Azure AD, которые находятся под угрозой.</span><span class="sxs-lookup"><span data-stu-id="a854a-105">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="a854a-106">Azure AD постоянно оценивает риск пользователя на основе различных сигналов и машинного обучения.</span><span class="sxs-lookup"><span data-stu-id="a854a-106">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="a854a-107">Этот API предоставляет программный доступ ко всем пользователям с рисками в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a854a-107">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="a854a-108">Для получения дополнительных сведений о событиях риска обратитесь к разделу [Защита удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span><span class="sxs-lookup"><span data-stu-id="a854a-108">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="a854a-109">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="a854a-109">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="a854a-110">Методы</span><span class="sxs-lookup"><span data-stu-id="a854a-110">Methods</span></span>
|<span data-ttu-id="a854a-111">Метод</span><span class="sxs-lookup"><span data-stu-id="a854a-111">Method</span></span>|<span data-ttu-id="a854a-112">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="a854a-112">Return type</span></span>|<span data-ttu-id="a854a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="a854a-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a854a-114">Список riskyUsers</span><span class="sxs-lookup"><span data-stu-id="a854a-114">List riskyUsers</span></span>](../api/riskyuser-list.md)|<span data-ttu-id="a854a-115">Коллекция [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="a854a-115">[riskyUser](../resources/riskyuser.md) collection</span></span>|<span data-ttu-id="a854a-116">Получение списка объектов **рискюсер** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="a854a-116">Get a list of the **riskyUser** objects and their properties.</span></span>|
|[<span data-ttu-id="a854a-117">Получение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="a854a-117">Get riskyUser</span></span>](../api/riskyuser-get.md)|[<span data-ttu-id="a854a-118">рискюсер</span><span class="sxs-lookup"><span data-stu-id="a854a-118">riskyUser</span></span>](../resources/riskyuser.md)|<span data-ttu-id="a854a-119">Чтение свойств и связей объекта **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="a854a-119">Read the properties and relationships of a **riskyUser** object.</span></span>|
|[<span data-ttu-id="a854a-120">Отклонение Рискюсер</span><span class="sxs-lookup"><span data-stu-id="a854a-120">Dismiss a riskyUser</span></span>](../api/riskyuser-dismiss.md)|<span data-ttu-id="a854a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="a854a-121">None</span></span>|<span data-ttu-id="a854a-122">Отклонить риск одного или нескольких объектов **рискюсер** .</span><span class="sxs-lookup"><span data-stu-id="a854a-122">Dismiss the risk of one or more **riskyUser** objects.</span></span> |
|[<span data-ttu-id="a854a-123">Подтверждение Рискюсер в качестве скомпрометированного</span><span class="sxs-lookup"><span data-stu-id="a854a-123">Confirm a riskyUser as compromised</span></span>](../api/riskyuser-confirmcompromised.md)|<span data-ttu-id="a854a-124">Нет</span><span class="sxs-lookup"><span data-stu-id="a854a-124">None</span></span>|<span data-ttu-id="a854a-125">Подтвердите, что один или несколько объектов **рискюсер** считаются скомпрометированными.</span><span class="sxs-lookup"><span data-stu-id="a854a-125">Confirm one or more **riskyUser** objects as compromised.</span></span>|
|[<span data-ttu-id="a854a-126">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="a854a-126">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="a854a-127">Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="a854a-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="a854a-128">Получение **рискюсерхисторитемс** из свойства навигации по журналу.</span><span class="sxs-lookup"><span data-stu-id="a854a-128">Get the **riskyUserHistoryItems** from the history navigation property.</span></span>|
|[<span data-ttu-id="a854a-129">Получение журнала</span><span class="sxs-lookup"><span data-stu-id="a854a-129">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="a854a-130">рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="a854a-130">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="a854a-131">Чтение свойств и связей объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="a854a-131">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="a854a-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="a854a-132">Properties</span></span>
|<span data-ttu-id="a854a-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a854a-133">Property</span></span>|<span data-ttu-id="a854a-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a854a-134">Type</span></span>|<span data-ttu-id="a854a-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a854a-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a854a-136">id</span><span class="sxs-lookup"><span data-stu-id="a854a-136">id</span></span>|<span data-ttu-id="a854a-137">String</span><span class="sxs-lookup"><span data-stu-id="a854a-137">String</span></span>|<span data-ttu-id="a854a-138">Уникальный идентификатор пользователя под угрозой.</span><span class="sxs-lookup"><span data-stu-id="a854a-138">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="a854a-139">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a854a-139">isDeleted</span></span>|<span data-ttu-id="a854a-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="a854a-140">Boolean</span></span>|<span data-ttu-id="a854a-141">Указывает, удален ли пользователь.</span><span class="sxs-lookup"><span data-stu-id="a854a-141">Indicates whether the user is deleted.</span></span> <span data-ttu-id="a854a-142">Возможные значения: `true` , `false`</span><span class="sxs-lookup"><span data-stu-id="a854a-142">Possible values are: `true`, `false`</span></span>|
|<span data-ttu-id="a854a-143">Процесс обработки</span><span class="sxs-lookup"><span data-stu-id="a854a-143">isProcessing</span></span>|<span data-ttu-id="a854a-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="a854a-144">Boolean</span></span>|<span data-ttu-id="a854a-145">Указывает, вехсер ли опасное состояние пользователя при обработке внутренней</span><span class="sxs-lookup"><span data-stu-id="a854a-145">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|<span data-ttu-id="a854a-146">riskDetail</span><span class="sxs-lookup"><span data-stu-id="a854a-146">riskDetail</span></span>|<span data-ttu-id="a854a-147">riskDetail</span><span class="sxs-lookup"><span data-stu-id="a854a-147">riskDetail</span></span>|<span data-ttu-id="a854a-148">Сведения об обнаруженном риске.</span><span class="sxs-lookup"><span data-stu-id="a854a-148">Details of the detected risk.</span></span> <span data-ttu-id="a854a-149">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a854a-149">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a854a-150">рискластупдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="a854a-150">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="a854a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a854a-151">DateTimeOffset</span></span>|<span data-ttu-id="a854a-152">Дата и время последнего обновления рискованного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a854a-152">The date and time that the risky user was last updated.</span></span>|
|<span data-ttu-id="a854a-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="a854a-153">riskLevel</span></span>|<span data-ttu-id="a854a-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="a854a-154">riskLevel</span></span>|<span data-ttu-id="a854a-155">Уровень обнаруженного опасного пользователя.</span><span class="sxs-lookup"><span data-stu-id="a854a-155">Level of the detected risky user.</span></span> <span data-ttu-id="a854a-156">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a854a-156">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a854a-157">riskState</span><span class="sxs-lookup"><span data-stu-id="a854a-157">riskState</span></span>|<span data-ttu-id="a854a-158">riskState</span><span class="sxs-lookup"><span data-stu-id="a854a-158">riskState</span></span>|<span data-ttu-id="a854a-159">Состояние риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="a854a-159">State of the user's risk.</span></span> <span data-ttu-id="a854a-160">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a854a-160">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a854a-161">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a854a-161">userDisplayName</span></span>|<span data-ttu-id="a854a-162">String</span><span class="sxs-lookup"><span data-stu-id="a854a-162">String</span></span>|<span data-ttu-id="a854a-163">Опасное отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="a854a-163">Risky user display name.</span></span>|
|<span data-ttu-id="a854a-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a854a-164">userPrincipalName</span></span>|<span data-ttu-id="a854a-165">String</span><span class="sxs-lookup"><span data-stu-id="a854a-165">String</span></span>|<span data-ttu-id="a854a-166">Опасное имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="a854a-166">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a854a-167">Связи</span><span class="sxs-lookup"><span data-stu-id="a854a-167">Relationships</span></span>
|<span data-ttu-id="a854a-168">Связь</span><span class="sxs-lookup"><span data-stu-id="a854a-168">Relationship</span></span>|<span data-ttu-id="a854a-169">Тип</span><span class="sxs-lookup"><span data-stu-id="a854a-169">Type</span></span>|<span data-ttu-id="a854a-170">Описание</span><span class="sxs-lookup"><span data-stu-id="a854a-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a854a-171">лист</span><span class="sxs-lookup"><span data-stu-id="a854a-171">history</span></span>|<span data-ttu-id="a854a-172">Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="a854a-172">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|   <span data-ttu-id="a854a-173">Действие, связанное с изменением уровня риска пользователя</span><span class="sxs-lookup"><span data-stu-id="a854a-173">The activity related to user risk level change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a854a-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a854a-174">JSON representation</span></span>
<span data-ttu-id="a854a-175">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a854a-175">The following is a JSON representation of the resource.</span></span>
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


