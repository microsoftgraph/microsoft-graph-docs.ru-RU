---
title: тип ресурса riskyUserHistoryItem
description: рискованный элемент истории пользователей
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2188a3a13d36a6d224b3c8ca2a7ac297c22712ce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443890"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="5937f-103">тип ресурса riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="5937f-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="5937f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5937f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5937f-105">Представляет историю рисков пользователя Azure AD, определяемую службой Azure AD Identity Protection.</span><span class="sxs-lookup"><span data-stu-id="5937f-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span>


<span data-ttu-id="5937f-106">Наследует от [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="5937f-106">Inherits from [riskyUser](../resources/riskyuser.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5937f-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5937f-107">Methods</span></span>
|<span data-ttu-id="5937f-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5937f-108">Method</span></span>|<span data-ttu-id="5937f-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="5937f-109">Return type</span></span>|<span data-ttu-id="5937f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5937f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5937f-111">История списка</span><span class="sxs-lookup"><span data-stu-id="5937f-111">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="5937f-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="5937f-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="5937f-113">Получите свойство riskyUserHistoryItems из свойства навигации по истории.</span><span class="sxs-lookup"><span data-stu-id="5937f-113">Get the riskyUserHistoryItems from the history navigation property.</span></span>|
|[<span data-ttu-id="5937f-114">Получить историю</span><span class="sxs-lookup"><span data-stu-id="5937f-114">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="5937f-115">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="5937f-115">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="5937f-116">Ознакомьтесь с свойствами и отношениями объекта [riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5937f-116">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5937f-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="5937f-117">Properties</span></span>
|<span data-ttu-id="5937f-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5937f-118">Property</span></span>|<span data-ttu-id="5937f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5937f-119">Type</span></span>|<span data-ttu-id="5937f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5937f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5937f-121">действие</span><span class="sxs-lookup"><span data-stu-id="5937f-121">activity</span></span>|[<span data-ttu-id="5937f-122">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="5937f-122">riskUserActivity</span></span>](../resources/riskuseractivity.md)|<span data-ttu-id="5937f-123">Действие, связанное с изменением уровня риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="5937f-123">The activity related to user risk level change.</span></span>|
|<span data-ttu-id="5937f-124">id</span><span class="sxs-lookup"><span data-stu-id="5937f-124">id</span></span>|<span data-ttu-id="5937f-125">String</span><span class="sxs-lookup"><span data-stu-id="5937f-125">String</span></span>|<span data-ttu-id="5937f-126">Унаследованный от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="5937f-126">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="5937f-127">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="5937f-127">initiatedBy</span></span>|<span data-ttu-id="5937f-128">String</span><span class="sxs-lookup"><span data-stu-id="5937f-128">String</span></span>|<span data-ttu-id="5937f-129">ID субъекта, который делает операцию.</span><span class="sxs-lookup"><span data-stu-id="5937f-129">The id of actor that does the operation.</span></span>|
|<span data-ttu-id="5937f-130">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5937f-130">isDeleted</span></span>|<span data-ttu-id="5937f-131">Логический</span><span class="sxs-lookup"><span data-stu-id="5937f-131">Boolean</span></span>| <span data-ttu-id="5937f-132">Унаследованный от [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5937f-132">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="5937f-133">isProcessing</span><span class="sxs-lookup"><span data-stu-id="5937f-133">isProcessing</span></span>|<span data-ttu-id="5937f-134">Логический</span><span class="sxs-lookup"><span data-stu-id="5937f-134">Boolean</span></span>| <span data-ttu-id="5937f-135">Унаследованный от [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5937f-135">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="5937f-136">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5937f-136">riskDetail</span></span>|<span data-ttu-id="5937f-137">riskDetail</span><span class="sxs-lookup"><span data-stu-id="5937f-137">riskDetail</span></span>|<span data-ttu-id="5937f-138">Унаследованный от [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="5937f-138">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="5937f-139">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5937f-139">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5937f-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5937f-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="5937f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5937f-141">DateTimeOffset</span></span>|<span data-ttu-id="5937f-142">Унаследованный от [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5937f-142">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="5937f-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5937f-143">riskLevel</span></span>|<span data-ttu-id="5937f-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="5937f-144">riskLevel</span></span>|<span data-ttu-id="5937f-145">Унаследованный от [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="5937f-145">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="5937f-146">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5937f-146">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5937f-147">riskState</span><span class="sxs-lookup"><span data-stu-id="5937f-147">riskState</span></span>|<span data-ttu-id="5937f-148">riskState</span><span class="sxs-lookup"><span data-stu-id="5937f-148">riskState</span></span>|<span data-ttu-id="5937f-149">Унаследованный от [riskyUser](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="5937f-149">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="5937f-150">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5937f-150">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="5937f-151">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5937f-151">userDisplayName</span></span>|<span data-ttu-id="5937f-152">String</span><span class="sxs-lookup"><span data-stu-id="5937f-152">String</span></span>|<span data-ttu-id="5937f-153">Унаследованный от [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5937f-153">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="5937f-154">userId</span><span class="sxs-lookup"><span data-stu-id="5937f-154">userId</span></span>|<span data-ttu-id="5937f-155">String</span><span class="sxs-lookup"><span data-stu-id="5937f-155">String</span></span>|<span data-ttu-id="5937f-156">ID пользователя.</span><span class="sxs-lookup"><span data-stu-id="5937f-156">The id of the user.</span></span>|
|<span data-ttu-id="5937f-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5937f-157">userPrincipalName</span></span>|<span data-ttu-id="5937f-158">String</span><span class="sxs-lookup"><span data-stu-id="5937f-158">String</span></span>|<span data-ttu-id="5937f-159">Рискованное основное имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="5937f-159">Risky user principal name.</span></span> <span data-ttu-id="5937f-160">Унаследованный от [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5937f-160">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="5937f-161">Связи</span><span class="sxs-lookup"><span data-stu-id="5937f-161">Relationships</span></span>
|<span data-ttu-id="5937f-162">Связь</span><span class="sxs-lookup"><span data-stu-id="5937f-162">Relationship</span></span>|<span data-ttu-id="5937f-163">Тип</span><span class="sxs-lookup"><span data-stu-id="5937f-163">Type</span></span>|<span data-ttu-id="5937f-164">Описание</span><span class="sxs-lookup"><span data-stu-id="5937f-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5937f-165">история</span><span class="sxs-lookup"><span data-stu-id="5937f-165">history</span></span>|<span data-ttu-id="5937f-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span><span class="sxs-lookup"><span data-stu-id="5937f-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>| <span data-ttu-id="5937f-167">Унаследованный от [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="5937f-167">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5937f-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5937f-168">JSON representation</span></span>
<span data-ttu-id="5937f-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5937f-169">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "initiatedBy": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  }
}
```


