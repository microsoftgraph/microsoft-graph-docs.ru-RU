---
title: Тип ресурса directRoutingLogRow
description: Представляет строку данных в журнале вызовов прямой маршрутки.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 21104f3d0812edd2af7918d6b55ff9a2f9013037
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159656"
---
# <a name="directroutinglogrow-resource-type"></a><span data-ttu-id="1003b-103">Тип ресурса directRoutingLogRow</span><span class="sxs-lookup"><span data-stu-id="1003b-103">directRoutingLogRow resource type</span></span>

<span data-ttu-id="1003b-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="1003b-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1003b-105">Представляет строку данных в журнале вызовов прямой маршрутки.</span><span class="sxs-lookup"><span data-stu-id="1003b-105">Represents a row of data in the direct routing call log.</span></span> <span data-ttu-id="1003b-106">Каждая строка сопозовна одному вызову.</span><span class="sxs-lookup"><span data-stu-id="1003b-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="1003b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1003b-107">Properties</span></span>

|<span data-ttu-id="1003b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1003b-108">Property</span></span>|<span data-ttu-id="1003b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1003b-109">Type</span></span>|<span data-ttu-id="1003b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1003b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1003b-111">id</span><span class="sxs-lookup"><span data-stu-id="1003b-111">id</span></span>|<span data-ttu-id="1003b-112">String</span><span class="sxs-lookup"><span data-stu-id="1003b-112">String</span></span>|<span data-ttu-id="1003b-113">Уникальный идентификатор вызова.</span><span class="sxs-lookup"><span data-stu-id="1003b-113">Unique call identifier.</span></span> <span data-ttu-id="1003b-114">GUID.</span><span class="sxs-lookup"><span data-stu-id="1003b-114">GUID.</span></span>|
|<span data-ttu-id="1003b-115">correlationId</span><span class="sxs-lookup"><span data-stu-id="1003b-115">correlationId</span></span>|<span data-ttu-id="1003b-116">String</span><span class="sxs-lookup"><span data-stu-id="1003b-116">String</span></span>|<span data-ttu-id="1003b-117">Идентификатор вызова, который можно использовать при вызове службы поддержки Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1003b-117">Identifier for the call that you can use when calling Microsoft Support.</span></span> <span data-ttu-id="1003b-118">GUID.</span><span class="sxs-lookup"><span data-stu-id="1003b-118">GUID.</span></span>|
|<span data-ttu-id="1003b-119">userId</span><span class="sxs-lookup"><span data-stu-id="1003b-119">userId</span></span>|<span data-ttu-id="1003b-120">String</span><span class="sxs-lookup"><span data-stu-id="1003b-120">String</span></span>|<span data-ttu-id="1003b-121">ИД вызываемого пользователя в Graph.</span><span class="sxs-lookup"><span data-stu-id="1003b-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="1003b-122">Эти и другие сведения о пользователе будут пустыми или пустыми для типов вызовов ботов.</span><span class="sxs-lookup"><span data-stu-id="1003b-122">This and other user info will be null/empty for bot call types.</span></span> <span data-ttu-id="1003b-123">GUID.</span><span class="sxs-lookup"><span data-stu-id="1003b-123">GUID.</span></span>|
|<span data-ttu-id="1003b-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1003b-124">userPrincipalName</span></span>|<span data-ttu-id="1003b-125">String</span><span class="sxs-lookup"><span data-stu-id="1003b-125">String</span></span>|<span data-ttu-id="1003b-126">UserPrincipalName (имя для регистрации) в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1003b-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="1003b-127">Обычно он такой же, как SIP-адрес пользователя, и может быть таким же, как и адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="1003b-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="1003b-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1003b-128">userDisplayName</span></span>|<span data-ttu-id="1003b-129">String</span><span class="sxs-lookup"><span data-stu-id="1003b-129">String</span></span>|<span data-ttu-id="1003b-130">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="1003b-130">Display name of the user.</span></span>|
|<span data-ttu-id="1003b-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1003b-131">startDateTime</span></span>|<span data-ttu-id="1003b-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1003b-132">DateTimeOffset</span></span>|<span data-ttu-id="1003b-133">Время начала вызова.</span><span class="sxs-lookup"><span data-stu-id="1003b-133">Call start time.</span></span><br/><span data-ttu-id="1003b-134">Для неудачных и неотвеченных вызовов это может быть равно приглашению или времени сбоя.</span><span class="sxs-lookup"><span data-stu-id="1003b-134">For failed and unanswered calls, this can be equal to invite or failure time.</span></span>|
|<span data-ttu-id="1003b-135">inviteDateTime</span><span class="sxs-lookup"><span data-stu-id="1003b-135">inviteDateTime</span></span>|<span data-ttu-id="1003b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1003b-136">DateTimeOffset</span></span>| <span data-ttu-id="1003b-137">Когда было отправлено начальное приглашение.</span><span class="sxs-lookup"><span data-stu-id="1003b-137">When the initial invite was sent.</span></span>|
|<span data-ttu-id="1003b-138">failureDateTime</span><span class="sxs-lookup"><span data-stu-id="1003b-138">failureDateTime</span></span>|<span data-ttu-id="1003b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1003b-139">DateTimeOffset</span></span>| <span data-ttu-id="1003b-140">Существует только для неудачных (не полностью установленных) вызовов.</span><span class="sxs-lookup"><span data-stu-id="1003b-140">Only exists for failed (not fully established) calls.</span></span>|
|<span data-ttu-id="1003b-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1003b-141">endDateTime</span></span>|<span data-ttu-id="1003b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1003b-142">DateTimeOffset</span></span>| <span data-ttu-id="1003b-143">Существует только для успешных (полностью установленных) вызовов.</span><span class="sxs-lookup"><span data-stu-id="1003b-143">Only exists for successful (fully established) calls.</span></span> <span data-ttu-id="1003b-144">Время окончания вызова.</span><span class="sxs-lookup"><span data-stu-id="1003b-144">Time when call ended.</span></span>|
|<span data-ttu-id="1003b-145">duration</span><span class="sxs-lookup"><span data-stu-id="1003b-145">duration</span></span>|<span data-ttu-id="1003b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1003b-146">Int32</span></span>| <span data-ttu-id="1003b-147">Продолжительность вызова в секундах.</span><span class="sxs-lookup"><span data-stu-id="1003b-147">Duration of the call in seconds.</span></span>|
|<span data-ttu-id="1003b-148">callType</span><span class="sxs-lookup"><span data-stu-id="1003b-148">callType</span></span>|<span data-ttu-id="1003b-149">String</span><span class="sxs-lookup"><span data-stu-id="1003b-149">String</span></span>| <span data-ttu-id="1003b-150">Тип и направление вызова.</span><span class="sxs-lookup"><span data-stu-id="1003b-150">Call type and direction.</span></span>|
|<span data-ttu-id="1003b-151">successfulCall</span><span class="sxs-lookup"><span data-stu-id="1003b-151">successfulCall</span></span>|<span data-ttu-id="1003b-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1003b-152">Boolean</span></span>| <span data-ttu-id="1003b-153">Успех или попытка.</span><span class="sxs-lookup"><span data-stu-id="1003b-153">Success or attempt.</span></span>|
|<span data-ttu-id="1003b-154">callerNumber</span><span class="sxs-lookup"><span data-stu-id="1003b-154">callerNumber</span></span>|<span data-ttu-id="1003b-155">String</span><span class="sxs-lookup"><span data-stu-id="1003b-155">String</span></span>| <span data-ttu-id="1003b-156">Номер пользователя или бота, который сделал вызов.</span><span class="sxs-lookup"><span data-stu-id="1003b-156">Number of the user or bot who made the call.</span></span> <span data-ttu-id="1003b-157">[Формат E.164,](https://en.wikipedia.org/wiki/E.164) но может включать дополнительные данные.</span><span class="sxs-lookup"><span data-stu-id="1003b-157">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="1003b-158">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="1003b-158">calleeNumber</span></span>|<span data-ttu-id="1003b-159">String</span><span class="sxs-lookup"><span data-stu-id="1003b-159">String</span></span>| <span data-ttu-id="1003b-160">Номер пользователя или бота, который принял вызов.</span><span class="sxs-lookup"><span data-stu-id="1003b-160">Number of the user or bot who received the call.</span></span> <span data-ttu-id="1003b-161">[Формат E.164,](https://en.wikipedia.org/wiki/E.164) но может включать дополнительные данные.</span><span class="sxs-lookup"><span data-stu-id="1003b-161">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="1003b-162">mediaPathLocation</span><span class="sxs-lookup"><span data-stu-id="1003b-162">mediaPathLocation</span></span>|<span data-ttu-id="1003b-163">String</span><span class="sxs-lookup"><span data-stu-id="1003b-163">String</span></span>| <span data-ttu-id="1003b-164">Центр обработки данных, используемый для пути мультимедиа при вызове без обхода.</span><span class="sxs-lookup"><span data-stu-id="1003b-164">The datacenter used for media path in non-bypass call.</span></span>|
|<span data-ttu-id="1003b-165">signalingLocation</span><span class="sxs-lookup"><span data-stu-id="1003b-165">signalingLocation</span></span>|<span data-ttu-id="1003b-166">String</span><span class="sxs-lookup"><span data-stu-id="1003b-166">String</span></span>| <span data-ttu-id="1003b-167">Центр обработки данных, используемый для передачи сигналов как для вызовов обхода, так и для вызовов без обхода.</span><span class="sxs-lookup"><span data-stu-id="1003b-167">The datacenter used for signaling for both bypass and non-bypass calls.</span></span>|
|<span data-ttu-id="1003b-168">finalSipCode</span><span class="sxs-lookup"><span data-stu-id="1003b-168">finalSipCode</span></span>|<span data-ttu-id="1003b-169">Int32</span><span class="sxs-lookup"><span data-stu-id="1003b-169">Int32</span></span>| <span data-ttu-id="1003b-170">Код, с помощью которого вызов был завершен, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span><span class="sxs-lookup"><span data-stu-id="1003b-170">The code with which the call ended, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span></span>|
|<span data-ttu-id="1003b-171">callEndSubReason</span><span class="sxs-lookup"><span data-stu-id="1003b-171">callEndSubReason</span></span>|<span data-ttu-id="1003b-172">Int32</span><span class="sxs-lookup"><span data-stu-id="1003b-172">Int32</span></span>| <span data-ttu-id="1003b-173">Помимо кодов SIP, корпорация Майкрософт имеет собственные подкоды, которые указывают на конкретную проблему.</span><span class="sxs-lookup"><span data-stu-id="1003b-173">In addition to the SIP codes, Microsoft has own subcodes that indicate the specific issue.</span></span>|
|<span data-ttu-id="1003b-174">finalSipCodePhrase</span><span class="sxs-lookup"><span data-stu-id="1003b-174">finalSipCodePhrase</span></span>|<span data-ttu-id="1003b-175">String</span><span class="sxs-lookup"><span data-stu-id="1003b-175">String</span></span>| <span data-ttu-id="1003b-176">Описание кода SIP и подкода Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1003b-176">Description of the SIP code and Microsoft subcode.</span></span>|
|<span data-ttu-id="1003b-177">trunkFullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="1003b-177">trunkFullyQualifiedDomainName</span></span>|<span data-ttu-id="1003b-178">String</span><span class="sxs-lookup"><span data-stu-id="1003b-178">String</span></span>| <span data-ttu-id="1003b-179">Полное доменное имя пограничного контроллера сеанса.</span><span class="sxs-lookup"><span data-stu-id="1003b-179">Fully qualified domain name of the session border controller.</span></span>|
|<span data-ttu-id="1003b-180">mediaBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="1003b-180">mediaBypassEnabled</span></span>|<span data-ttu-id="1003b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1003b-181">Boolean</span></span>| <span data-ttu-id="1003b-182">Указывает, включена ли для магистрали обход мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="1003b-182">Indicates if the trunk was enabled for media bypass or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1003b-183">Связи</span><span class="sxs-lookup"><span data-stu-id="1003b-183">Relationships</span></span>

<span data-ttu-id="1003b-184">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1003b-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1003b-185">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1003b-185">JSON representation</span></span>

<span data-ttu-id="1003b-186">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1003b-186">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
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


