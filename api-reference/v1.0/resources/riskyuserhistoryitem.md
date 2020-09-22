---
title: Тип ресурса Рискюсерхисторитем
description: элемент истории опасного пользователя
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 551f008696b3c9507f1cae414c34de5a8779ab24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984161"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="30fa5-103">Тип ресурса Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="30fa5-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="30fa5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30fa5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="30fa5-105">Представляет историю риска пользователя Azure AD, определенная службой защиты удостоверений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="30fa5-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span>


<span data-ttu-id="30fa5-106">Наследуется от [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="30fa5-106">Inherits from [riskyUser](../resources/riskyuser.md).</span></span>

## <a name="methods"></a><span data-ttu-id="30fa5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="30fa5-107">Methods</span></span>
|<span data-ttu-id="30fa5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="30fa5-108">Method</span></span>|<span data-ttu-id="30fa5-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="30fa5-109">Return type</span></span>|<span data-ttu-id="30fa5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="30fa5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30fa5-111">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="30fa5-111">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="30fa5-112">Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="30fa5-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="30fa5-113">Получение Рискюсерхисторитемс из свойства навигации по журналу.</span><span class="sxs-lookup"><span data-stu-id="30fa5-113">Get the riskyUserHistoryItems from the history navigation property.</span></span>|
|[<span data-ttu-id="30fa5-114">Получение журнала</span><span class="sxs-lookup"><span data-stu-id="30fa5-114">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="30fa5-115">рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="30fa5-115">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="30fa5-116">Чтение свойств и связей объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="30fa5-116">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30fa5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="30fa5-117">Properties</span></span>
|<span data-ttu-id="30fa5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="30fa5-118">Property</span></span>|<span data-ttu-id="30fa5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="30fa5-119">Type</span></span>|<span data-ttu-id="30fa5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="30fa5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30fa5-121">activity</span><span class="sxs-lookup"><span data-stu-id="30fa5-121">activity</span></span>|[<span data-ttu-id="30fa5-122">рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="30fa5-122">riskUserActivity</span></span>](../resources/riskuseractivity.md)|<span data-ttu-id="30fa5-123">Действие, связанное с изменением уровня риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="30fa5-123">The activity related to user risk level change.</span></span>|
|<span data-ttu-id="30fa5-124">id</span><span class="sxs-lookup"><span data-stu-id="30fa5-124">id</span></span>|<span data-ttu-id="30fa5-125">String</span><span class="sxs-lookup"><span data-stu-id="30fa5-125">String</span></span>|<span data-ttu-id="30fa5-126">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="30fa5-126">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="30fa5-127">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="30fa5-127">initiatedBy</span></span>|<span data-ttu-id="30fa5-128">String</span><span class="sxs-lookup"><span data-stu-id="30fa5-128">String</span></span>|<span data-ttu-id="30fa5-129">Идентификатор субъекта, который выполняет операцию.</span><span class="sxs-lookup"><span data-stu-id="30fa5-129">The id of actor that does the operation.</span></span>|
|<span data-ttu-id="30fa5-130">isDeleted</span><span class="sxs-lookup"><span data-stu-id="30fa5-130">isDeleted</span></span>|<span data-ttu-id="30fa5-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="30fa5-131">Boolean</span></span>| <span data-ttu-id="30fa5-132">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="30fa5-132">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="30fa5-133">Процесс обработки</span><span class="sxs-lookup"><span data-stu-id="30fa5-133">isProcessing</span></span>|<span data-ttu-id="30fa5-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="30fa5-134">Boolean</span></span>| <span data-ttu-id="30fa5-135">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="30fa5-135">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="30fa5-136">riskDetail</span><span class="sxs-lookup"><span data-stu-id="30fa5-136">riskDetail</span></span>|<span data-ttu-id="30fa5-137">riskDetail</span><span class="sxs-lookup"><span data-stu-id="30fa5-137">riskDetail</span></span>|<span data-ttu-id="30fa5-138">Наследуется от [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="30fa5-138">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="30fa5-139">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="30fa5-139">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="30fa5-140">рискластупдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="30fa5-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="30fa5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30fa5-141">DateTimeOffset</span></span>|<span data-ttu-id="30fa5-142">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="30fa5-142">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="30fa5-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="30fa5-143">riskLevel</span></span>|<span data-ttu-id="30fa5-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="30fa5-144">riskLevel</span></span>|<span data-ttu-id="30fa5-145">Наследуется от [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="30fa5-145">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="30fa5-146">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="30fa5-146">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="30fa5-147">riskState</span><span class="sxs-lookup"><span data-stu-id="30fa5-147">riskState</span></span>|<span data-ttu-id="30fa5-148">riskState</span><span class="sxs-lookup"><span data-stu-id="30fa5-148">riskState</span></span>|<span data-ttu-id="30fa5-149">Наследуется от [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="30fa5-149">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="30fa5-150">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="30fa5-150">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="30fa5-151">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="30fa5-151">userDisplayName</span></span>|<span data-ttu-id="30fa5-152">String</span><span class="sxs-lookup"><span data-stu-id="30fa5-152">String</span></span>|<span data-ttu-id="30fa5-153">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="30fa5-153">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="30fa5-154">userId</span><span class="sxs-lookup"><span data-stu-id="30fa5-154">userId</span></span>|<span data-ttu-id="30fa5-155">String</span><span class="sxs-lookup"><span data-stu-id="30fa5-155">String</span></span>|<span data-ttu-id="30fa5-156">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="30fa5-156">The id of the user.</span></span>|
|<span data-ttu-id="30fa5-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="30fa5-157">userPrincipalName</span></span>|<span data-ttu-id="30fa5-158">String</span><span class="sxs-lookup"><span data-stu-id="30fa5-158">String</span></span>|<span data-ttu-id="30fa5-159">Опасное имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="30fa5-159">Risky user principal name.</span></span> <span data-ttu-id="30fa5-160">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="30fa5-160">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="30fa5-161">Связи</span><span class="sxs-lookup"><span data-stu-id="30fa5-161">Relationships</span></span>
|<span data-ttu-id="30fa5-162">Связь</span><span class="sxs-lookup"><span data-stu-id="30fa5-162">Relationship</span></span>|<span data-ttu-id="30fa5-163">Тип</span><span class="sxs-lookup"><span data-stu-id="30fa5-163">Type</span></span>|<span data-ttu-id="30fa5-164">Описание</span><span class="sxs-lookup"><span data-stu-id="30fa5-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30fa5-165">лист</span><span class="sxs-lookup"><span data-stu-id="30fa5-165">history</span></span>|<span data-ttu-id="30fa5-166">Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="30fa5-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>| <span data-ttu-id="30fa5-167">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="30fa5-167">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30fa5-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30fa5-168">JSON representation</span></span>
<span data-ttu-id="30fa5-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30fa5-169">The following is a JSON representation of the resource.</span></span>
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


