---
title: Тип ресурса Рискюсерхисторитем
description: элемент истории опасного пользователя
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bcf9e1834e8fff48a148095ffe7ddbd459ee23e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896002"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="88822-103">Тип ресурса Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="88822-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="88822-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88822-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88822-105">Представляет историю риска пользователя Azure AD, определенная службой защиты удостоверений Azure AD.</span><span class="sxs-lookup"><span data-stu-id="88822-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span>


<span data-ttu-id="88822-106">Наследуется от [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="88822-106">Inherits from [riskyUser](../resources/riskyuser.md).</span></span>

## <a name="methods"></a><span data-ttu-id="88822-107">Методы</span><span class="sxs-lookup"><span data-stu-id="88822-107">Methods</span></span>
|<span data-ttu-id="88822-108">Метод</span><span class="sxs-lookup"><span data-stu-id="88822-108">Method</span></span>|<span data-ttu-id="88822-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="88822-109">Return type</span></span>|<span data-ttu-id="88822-110">Описание</span><span class="sxs-lookup"><span data-stu-id="88822-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88822-111">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="88822-111">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="88822-112">Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="88822-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="88822-113">Получение Рискюсерхисторитемс из свойства навигации по журналу.</span><span class="sxs-lookup"><span data-stu-id="88822-113">Get the riskyUserHistoryItems from the history navigation property.</span></span>|
|[<span data-ttu-id="88822-114">Получение журнала</span><span class="sxs-lookup"><span data-stu-id="88822-114">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="88822-115">рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="88822-115">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="88822-116">Чтение свойств и связей объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="88822-116">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="88822-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="88822-117">Properties</span></span>
|<span data-ttu-id="88822-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="88822-118">Property</span></span>|<span data-ttu-id="88822-119">Тип</span><span class="sxs-lookup"><span data-stu-id="88822-119">Type</span></span>|<span data-ttu-id="88822-120">Описание</span><span class="sxs-lookup"><span data-stu-id="88822-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88822-121">activity</span><span class="sxs-lookup"><span data-stu-id="88822-121">activity</span></span>|[<span data-ttu-id="88822-122">рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="88822-122">riskUserActivity</span></span>](../resources/riskuseractivity.md)|<span data-ttu-id="88822-123">Действие, связанное с изменением уровня риска пользователя.</span><span class="sxs-lookup"><span data-stu-id="88822-123">The activity related to user risk level change.</span></span>|
|<span data-ttu-id="88822-124">id</span><span class="sxs-lookup"><span data-stu-id="88822-124">id</span></span>|<span data-ttu-id="88822-125">Строка</span><span class="sxs-lookup"><span data-stu-id="88822-125">String</span></span>|<span data-ttu-id="88822-126">Наследуется от [объекта](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="88822-126">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="88822-127">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="88822-127">initiatedBy</span></span>|<span data-ttu-id="88822-128">String</span><span class="sxs-lookup"><span data-stu-id="88822-128">String</span></span>|<span data-ttu-id="88822-129">Идентификатор субъекта, который выполняет операцию.</span><span class="sxs-lookup"><span data-stu-id="88822-129">The id of actor that does the operation.</span></span>|
|<span data-ttu-id="88822-130">isDeleted</span><span class="sxs-lookup"><span data-stu-id="88822-130">isDeleted</span></span>|<span data-ttu-id="88822-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="88822-131">Boolean</span></span>| <span data-ttu-id="88822-132">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="88822-132">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="88822-133">Процесс обработки</span><span class="sxs-lookup"><span data-stu-id="88822-133">isProcessing</span></span>|<span data-ttu-id="88822-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="88822-134">Boolean</span></span>| <span data-ttu-id="88822-135">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="88822-135">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="88822-136">riskDetail</span><span class="sxs-lookup"><span data-stu-id="88822-136">riskDetail</span></span>|<span data-ttu-id="88822-137">riskDetail</span><span class="sxs-lookup"><span data-stu-id="88822-137">riskDetail</span></span>|<span data-ttu-id="88822-138">Наследуется от [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="88822-138">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="88822-139">Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="88822-139">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="88822-140">рискластупдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="88822-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="88822-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88822-141">DateTimeOffset</span></span>|<span data-ttu-id="88822-142">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="88822-142">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="88822-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="88822-143">riskLevel</span></span>|<span data-ttu-id="88822-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="88822-144">riskLevel</span></span>|<span data-ttu-id="88822-145">Наследуется от [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="88822-145">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="88822-146">Возможные значения: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="88822-146">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="88822-147">riskState</span><span class="sxs-lookup"><span data-stu-id="88822-147">riskState</span></span>|<span data-ttu-id="88822-148">riskState</span><span class="sxs-lookup"><span data-stu-id="88822-148">riskState</span></span>|<span data-ttu-id="88822-149">Наследуется от [рискюсер](../resources/riskyuser.md).</span><span class="sxs-lookup"><span data-stu-id="88822-149">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="88822-150">Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="88822-150">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="88822-151">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="88822-151">userDisplayName</span></span>|<span data-ttu-id="88822-152">String</span><span class="sxs-lookup"><span data-stu-id="88822-152">String</span></span>|<span data-ttu-id="88822-153">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="88822-153">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="88822-154">userId</span><span class="sxs-lookup"><span data-stu-id="88822-154">userId</span></span>|<span data-ttu-id="88822-155">String</span><span class="sxs-lookup"><span data-stu-id="88822-155">String</span></span>|<span data-ttu-id="88822-156">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="88822-156">The id of the user.</span></span>|
|<span data-ttu-id="88822-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="88822-157">userPrincipalName</span></span>|<span data-ttu-id="88822-158">Строка</span><span class="sxs-lookup"><span data-stu-id="88822-158">String</span></span>|<span data-ttu-id="88822-159">Опасное имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="88822-159">Risky user principal name.</span></span> <span data-ttu-id="88822-160">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="88822-160">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="88822-161">Связи</span><span class="sxs-lookup"><span data-stu-id="88822-161">Relationships</span></span>
|<span data-ttu-id="88822-162">Связь</span><span class="sxs-lookup"><span data-stu-id="88822-162">Relationship</span></span>|<span data-ttu-id="88822-163">Тип</span><span class="sxs-lookup"><span data-stu-id="88822-163">Type</span></span>|<span data-ttu-id="88822-164">Описание</span><span class="sxs-lookup"><span data-stu-id="88822-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88822-165">лист</span><span class="sxs-lookup"><span data-stu-id="88822-165">history</span></span>|<span data-ttu-id="88822-166">Коллекция [рискюсерхисторитем](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="88822-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>| <span data-ttu-id="88822-167">Наследуется от [рискюсер](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="88822-167">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88822-168">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="88822-168">JSON representation</span></span>
<span data-ttu-id="88822-169">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88822-169">The following is a JSON representation of the resource.</span></span>
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

