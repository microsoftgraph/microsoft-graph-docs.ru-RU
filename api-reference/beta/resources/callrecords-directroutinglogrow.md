---
title: Тип ресурса Директраутинглогров
description: Представляет строку данных в журнале вызовов прямой маршрутизации.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b3636882236d24e3da1435e89904de1f2845756
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966774"
---
# <a name="directroutinglogrow-resource-type"></a><span data-ttu-id="54c98-103">Тип ресурса Директраутинглогров</span><span class="sxs-lookup"><span data-stu-id="54c98-103">directRoutingLogRow resource type</span></span>

<span data-ttu-id="54c98-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="54c98-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54c98-105">Представляет строку данных в журнале вызовов прямой маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="54c98-105">Represents a row of data in the direct routing call log.</span></span> <span data-ttu-id="54c98-106">Каждая строка соответствует одному вызову.</span><span class="sxs-lookup"><span data-stu-id="54c98-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="54c98-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="54c98-107">Properties</span></span>

|<span data-ttu-id="54c98-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="54c98-108">Property</span></span>|<span data-ttu-id="54c98-109">Тип</span><span class="sxs-lookup"><span data-stu-id="54c98-109">Type</span></span>|<span data-ttu-id="54c98-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54c98-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54c98-111">id</span><span class="sxs-lookup"><span data-stu-id="54c98-111">id</span></span>|<span data-ttu-id="54c98-112">String</span><span class="sxs-lookup"><span data-stu-id="54c98-112">String</span></span>|<span data-ttu-id="54c98-113">Уникальный идентификатор звонка.</span><span class="sxs-lookup"><span data-stu-id="54c98-113">Unique call identifier.</span></span> <span data-ttu-id="54c98-114">Кодом.</span><span class="sxs-lookup"><span data-stu-id="54c98-114">GUID.</span></span>|
|<span data-ttu-id="54c98-115">correlationId</span><span class="sxs-lookup"><span data-stu-id="54c98-115">correlationId</span></span>|<span data-ttu-id="54c98-116">String</span><span class="sxs-lookup"><span data-stu-id="54c98-116">String</span></span>|<span data-ttu-id="54c98-117">Идентификатор вызова, который можно использовать при вызове службы поддержки Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="54c98-117">Identifier for the call that you can use when calling Microsoft Support.</span></span> <span data-ttu-id="54c98-118">Кодом.</span><span class="sxs-lookup"><span data-stu-id="54c98-118">GUID.</span></span>|
|<span data-ttu-id="54c98-119">userId</span><span class="sxs-lookup"><span data-stu-id="54c98-119">userId</span></span>|<span data-ttu-id="54c98-120">String</span><span class="sxs-lookup"><span data-stu-id="54c98-120">String</span></span>|<span data-ttu-id="54c98-121">Идентификатор вызывающего пользователя в Graph.</span><span class="sxs-lookup"><span data-stu-id="54c98-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="54c98-122">Эта и другие сведения о пользователе будут иметь значение null или Empty для типов вызовов Bot.</span><span class="sxs-lookup"><span data-stu-id="54c98-122">This and other user info will be null/empty for bot call types.</span></span> <span data-ttu-id="54c98-123">Кодом.</span><span class="sxs-lookup"><span data-stu-id="54c98-123">GUID.</span></span>|
|<span data-ttu-id="54c98-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="54c98-124">userPrincipalName</span></span>|<span data-ttu-id="54c98-125">String</span><span class="sxs-lookup"><span data-stu-id="54c98-125">String</span></span>|<span data-ttu-id="54c98-126">UserPrincipalName (имя входа) в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="54c98-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="54c98-127">Обычно это тот же адрес SIP, что и адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="54c98-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="54c98-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="54c98-128">userDisplayName</span></span>|<span data-ttu-id="54c98-129">String</span><span class="sxs-lookup"><span data-stu-id="54c98-129">String</span></span>|<span data-ttu-id="54c98-130">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="54c98-130">Display name of the user.</span></span>|
|<span data-ttu-id="54c98-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="54c98-131">startDateTime</span></span>|<span data-ttu-id="54c98-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54c98-132">DateTimeOffset</span></span>|<span data-ttu-id="54c98-133">Время начала вызова.</span><span class="sxs-lookup"><span data-stu-id="54c98-133">Call start time.</span></span><br/><span data-ttu-id="54c98-134">Для неудачных и неотвеченных вызовов это значение может быть равно приглашению или времени сбоя.</span><span class="sxs-lookup"><span data-stu-id="54c98-134">For failed and unanswered calls, this can be equal to invite or failure time.</span></span>|
|<span data-ttu-id="54c98-135">инвитедатетиме</span><span class="sxs-lookup"><span data-stu-id="54c98-135">inviteDateTime</span></span>|<span data-ttu-id="54c98-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54c98-136">DateTimeOffset</span></span>| <span data-ttu-id="54c98-137">При отправке первого приглашения.</span><span class="sxs-lookup"><span data-stu-id="54c98-137">When the initial invite was sent.</span></span>|
|<span data-ttu-id="54c98-138">фаилуредатетиме</span><span class="sxs-lookup"><span data-stu-id="54c98-138">failureDateTime</span></span>|<span data-ttu-id="54c98-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54c98-139">DateTimeOffset</span></span>| <span data-ttu-id="54c98-140">Существует только для вызовов с ошибками (не полностью установленными).</span><span class="sxs-lookup"><span data-stu-id="54c98-140">Only exists for failed (not fully established) calls.</span></span>|
|<span data-ttu-id="54c98-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="54c98-141">endDateTime</span></span>|<span data-ttu-id="54c98-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54c98-142">DateTimeOffset</span></span>| <span data-ttu-id="54c98-143">Существует только для успешных (полностью установленных) вызовов.</span><span class="sxs-lookup"><span data-stu-id="54c98-143">Only exists for successful (fully established) calls.</span></span> <span data-ttu-id="54c98-144">Время окончания звонка.</span><span class="sxs-lookup"><span data-stu-id="54c98-144">Time when call ended.</span></span>|
|<span data-ttu-id="54c98-145">duration</span><span class="sxs-lookup"><span data-stu-id="54c98-145">duration</span></span>|<span data-ttu-id="54c98-146">Int32</span><span class="sxs-lookup"><span data-stu-id="54c98-146">Int32</span></span>| <span data-ttu-id="54c98-147">Продолжительность звонка в секундах.</span><span class="sxs-lookup"><span data-stu-id="54c98-147">Duration of the call in seconds.</span></span>|
|<span data-ttu-id="54c98-148">callType</span><span class="sxs-lookup"><span data-stu-id="54c98-148">callType</span></span>|<span data-ttu-id="54c98-149">String</span><span class="sxs-lookup"><span data-stu-id="54c98-149">String</span></span>| <span data-ttu-id="54c98-150">Тип и направление звонка.</span><span class="sxs-lookup"><span data-stu-id="54c98-150">Call type and direction.</span></span>|
|<span data-ttu-id="54c98-151">сукцессфулкалл</span><span class="sxs-lookup"><span data-stu-id="54c98-151">successfulCall</span></span>|<span data-ttu-id="54c98-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="54c98-152">Boolean</span></span>| <span data-ttu-id="54c98-153">Успех или попытка.</span><span class="sxs-lookup"><span data-stu-id="54c98-153">Success or attempt.</span></span>|
|<span data-ttu-id="54c98-154">каллернумбер</span><span class="sxs-lookup"><span data-stu-id="54c98-154">callerNumber</span></span>|<span data-ttu-id="54c98-155">String</span><span class="sxs-lookup"><span data-stu-id="54c98-155">String</span></span>| <span data-ttu-id="54c98-156">Номер пользователя или ленты, выполнившего звонок.</span><span class="sxs-lookup"><span data-stu-id="54c98-156">Number of the user or bot who made the call.</span></span> <span data-ttu-id="54c98-157">Формат [E. 164](https://en.wikipedia.org/wiki/E.164) , но может содержать дополнительные данные.</span><span class="sxs-lookup"><span data-stu-id="54c98-157">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="54c98-158">каллинумбер</span><span class="sxs-lookup"><span data-stu-id="54c98-158">calleeNumber</span></span>|<span data-ttu-id="54c98-159">String</span><span class="sxs-lookup"><span data-stu-id="54c98-159">String</span></span>| <span data-ttu-id="54c98-160">Номер пользователя или робота, который получил звонок.</span><span class="sxs-lookup"><span data-stu-id="54c98-160">Number of the user or bot who received the call.</span></span> <span data-ttu-id="54c98-161">Формат [E. 164](https://en.wikipedia.org/wiki/E.164) , но может содержать дополнительные данные.</span><span class="sxs-lookup"><span data-stu-id="54c98-161">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="54c98-162">медиапаслокатион</span><span class="sxs-lookup"><span data-stu-id="54c98-162">mediaPathLocation</span></span>|<span data-ttu-id="54c98-163">String</span><span class="sxs-lookup"><span data-stu-id="54c98-163">String</span></span>| <span data-ttu-id="54c98-164">Центр обработки данных, используемый для пути к носителю при вызове без обхода.</span><span class="sxs-lookup"><span data-stu-id="54c98-164">The datacenter used for media path in non-bypass call.</span></span>|
|<span data-ttu-id="54c98-165">сигналинглокатион</span><span class="sxs-lookup"><span data-stu-id="54c98-165">signalingLocation</span></span>|<span data-ttu-id="54c98-166">String</span><span class="sxs-lookup"><span data-stu-id="54c98-166">String</span></span>| <span data-ttu-id="54c98-167">Центр обработки данных, используемый для передачи сигналов как для обхода, так и для вызовов без обхода.</span><span class="sxs-lookup"><span data-stu-id="54c98-167">The datacenter used for signaling for both bypass and non-bypass calls.</span></span>|
|<span data-ttu-id="54c98-168">финалсипкоде</span><span class="sxs-lookup"><span data-stu-id="54c98-168">finalSipCode</span></span>|<span data-ttu-id="54c98-169">Int32</span><span class="sxs-lookup"><span data-stu-id="54c98-169">Int32</span></span>| <span data-ttu-id="54c98-170">Код, с которым закончился вызов, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span><span class="sxs-lookup"><span data-stu-id="54c98-170">The code with which the call ended, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span></span>|
|<span data-ttu-id="54c98-171">каллендсубреасон</span><span class="sxs-lookup"><span data-stu-id="54c98-171">callEndSubReason</span></span>|<span data-ttu-id="54c98-172">Int32</span><span class="sxs-lookup"><span data-stu-id="54c98-172">Int32</span></span>| <span data-ttu-id="54c98-173">Помимо SIP кодов, у корпорации Майкрософт есть подкода, указывающие на конкретную ошибку.</span><span class="sxs-lookup"><span data-stu-id="54c98-173">In addition to the SIP codes, Microsoft has own subcodes that indicate the specific issue.</span></span>|
|<span data-ttu-id="54c98-174">финалсипкодефрасе</span><span class="sxs-lookup"><span data-stu-id="54c98-174">finalSipCodePhrase</span></span>|<span data-ttu-id="54c98-175">String</span><span class="sxs-lookup"><span data-stu-id="54c98-175">String</span></span>| <span data-ttu-id="54c98-176">Описание кода SIP и подкода корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="54c98-176">Description of the SIP code and Microsoft subcode.</span></span>|
|<span data-ttu-id="54c98-177">трункфулликуалифиеддомаиннаме</span><span class="sxs-lookup"><span data-stu-id="54c98-177">trunkFullyQualifiedDomainName</span></span>|<span data-ttu-id="54c98-178">String</span><span class="sxs-lookup"><span data-stu-id="54c98-178">String</span></span>| <span data-ttu-id="54c98-179">Полное доменное имя пограничного контроллера сеансов.</span><span class="sxs-lookup"><span data-stu-id="54c98-179">Fully qualified domain name of the session border controller.</span></span>|
|<span data-ttu-id="54c98-180">медиабипассенаблед</span><span class="sxs-lookup"><span data-stu-id="54c98-180">mediaBypassEnabled</span></span>|<span data-ttu-id="54c98-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="54c98-181">Boolean</span></span>| <span data-ttu-id="54c98-182">Указывает, включена ли магистраль для обхода сервера мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="54c98-182">Indicates if the trunk was enabled for media bypass or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54c98-183">Связи</span><span class="sxs-lookup"><span data-stu-id="54c98-183">Relationships</span></span>

<span data-ttu-id="54c98-184">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="54c98-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="54c98-185">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="54c98-185">JSON representation</span></span>

<span data-ttu-id="54c98-186">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54c98-186">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "baseType": "",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.directRoutingLogRow",
  "id": "String (identifier)",
  "correlationId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "inviteDateTime": "String (timestamp)",
  "failureDateTime": "String (timestamp)",
  "duration": "Integer",
  "callType": "String",
  "successfulCall": "Boolean",
  "callerNumber": "String",
  "calleeNumber": "String",
  "mediaPathLocation": "String",
  "signalingLocation": "String",
  "finalSipCode": "Integer",
  "callEndSubReason": "Integer",
  "finalSipCodePhrase": "String",
  "trunkFullyQualifiedDomainName": "String",
  "mediaBypassEnabled": "Boolean"
}
```


