---
title: Тип ресурса pstnCallLogRow
description: Представляет строку данных в журнале вызовов телефонной сети общего коммутатора (PSTN).
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5103404bdaa6ac4eafbfcffd45deef41c217600a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155582"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="4415e-103">Тип ресурса pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="4415e-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="4415e-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="4415e-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4415e-105">Представляет строку данных в журнале вызовов телефонной сети общего коммутатора (PSTN).</span><span class="sxs-lookup"><span data-stu-id="4415e-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="4415e-106">Каждая строка сопозовна одному вызову.</span><span class="sxs-lookup"><span data-stu-id="4415e-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="4415e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4415e-107">Properties</span></span>

|<span data-ttu-id="4415e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4415e-108">Property</span></span>|<span data-ttu-id="4415e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4415e-109">Type</span></span>|<span data-ttu-id="4415e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4415e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4415e-111">id</span><span class="sxs-lookup"><span data-stu-id="4415e-111">id</span></span>|<span data-ttu-id="4415e-112">String</span><span class="sxs-lookup"><span data-stu-id="4415e-112">String</span></span>|<span data-ttu-id="4415e-113">Уникальный идентификатор вызова.</span><span class="sxs-lookup"><span data-stu-id="4415e-113">Unique call identifier.</span></span> <span data-ttu-id="4415e-114">GUID.</span><span class="sxs-lookup"><span data-stu-id="4415e-114">GUID.</span></span>|
|<span data-ttu-id="4415e-115">callId</span><span class="sxs-lookup"><span data-stu-id="4415e-115">callId</span></span>|<span data-ttu-id="4415e-116">String</span><span class="sxs-lookup"><span data-stu-id="4415e-116">String</span></span>|<span data-ttu-id="4415e-117">Идентификатор вызова.</span><span class="sxs-lookup"><span data-stu-id="4415e-117">Call identifier.</span></span> <span data-ttu-id="4415e-118">Не гарантируется уникальность.</span><span class="sxs-lookup"><span data-stu-id="4415e-118">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="4415e-119">userId</span><span class="sxs-lookup"><span data-stu-id="4415e-119">userId</span></span>|<span data-ttu-id="4415e-120">String</span><span class="sxs-lookup"><span data-stu-id="4415e-120">String</span></span>|<span data-ttu-id="4415e-121">ИД вызываемого пользователя в Graph.</span><span class="sxs-lookup"><span data-stu-id="4415e-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="4415e-122">GUID.</span><span class="sxs-lookup"><span data-stu-id="4415e-122">GUID.</span></span> <span data-ttu-id="4415e-123">Эти и другие сведения о пользователе будут пустыми или пустыми для типов вызовов ботов (ucap_in, ucap_out).</span><span class="sxs-lookup"><span data-stu-id="4415e-123">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="4415e-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4415e-124">userPrincipalName</span></span>|<span data-ttu-id="4415e-125">String</span><span class="sxs-lookup"><span data-stu-id="4415e-125">String</span></span>|<span data-ttu-id="4415e-126">UserPrincipalName (имя для регистрации) в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4415e-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="4415e-127">Обычно он такой же, как SIP-адрес пользователя, и может быть таким же, как и адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="4415e-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="4415e-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4415e-128">userDisplayName</span></span>|<span data-ttu-id="4415e-129">String</span><span class="sxs-lookup"><span data-stu-id="4415e-129">String</span></span>|<span data-ttu-id="4415e-130">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="4415e-130">Display name of the user.</span></span>|
|<span data-ttu-id="4415e-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4415e-131">startDateTime</span></span>|<span data-ttu-id="4415e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4415e-132">DateTimeOffset</span></span>|<span data-ttu-id="4415e-133">Время начала вызова.</span><span class="sxs-lookup"><span data-stu-id="4415e-133">Call start time.</span></span>|
|<span data-ttu-id="4415e-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4415e-134">endDateTime</span></span>|<span data-ttu-id="4415e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4415e-135">DateTimeOffset</span></span>|<span data-ttu-id="4415e-136">Время окончания вызова.</span><span class="sxs-lookup"><span data-stu-id="4415e-136">Call end time.</span></span>|
|<span data-ttu-id="4415e-137">duration</span><span class="sxs-lookup"><span data-stu-id="4415e-137">duration</span></span>|<span data-ttu-id="4415e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="4415e-138">Int32</span></span>|<span data-ttu-id="4415e-139">Время подключения вызова в секундах.</span><span class="sxs-lookup"><span data-stu-id="4415e-139">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="4415e-140">charge</span><span class="sxs-lookup"><span data-stu-id="4415e-140">charge</span></span>|<span data-ttu-id="4415e-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4415e-141">Double</span></span>|<span data-ttu-id="4415e-142">Сумма денег или стоимость вызова, который взимается с вашей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="4415e-142">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="4415e-143">callType</span><span class="sxs-lookup"><span data-stu-id="4415e-143">callType</span></span>|<span data-ttu-id="4415e-144">String</span><span class="sxs-lookup"><span data-stu-id="4415e-144">String</span></span>|<span data-ttu-id="4415e-145">Был ли вызов исходящие или входящие вызовы STN, а также тип вызова, например звонок, который был сделан пользователем или аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="4415e-145">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="4415e-146">currency</span><span class="sxs-lookup"><span data-stu-id="4415e-146">currency</span></span>|<span data-ttu-id="4415e-147">String</span><span class="sxs-lookup"><span data-stu-id="4415e-147">String</span></span>|<span data-ttu-id="4415e-148">Тип валюты, используемой для расчета стоимости вызова[(ISO 4217).](https://en.wikipedia.org/wiki/ISO_4217)</span><span class="sxs-lookup"><span data-stu-id="4415e-148">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="4415e-149">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="4415e-149">calleeNumber</span></span>|<span data-ttu-id="4415e-150">String</span><span class="sxs-lookup"><span data-stu-id="4415e-150">String</span></span>|<span data-ttu-id="4415e-151">Номер, набираемый [в формате E.164.](https://en.wikipedia.org/wiki/E.164)</span><span class="sxs-lookup"><span data-stu-id="4415e-151">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="4415e-152">usageCountryCode</span><span class="sxs-lookup"><span data-stu-id="4415e-152">usageCountryCode</span></span>|<span data-ttu-id="4415e-153">String</span><span class="sxs-lookup"><span data-stu-id="4415e-153">String</span></span>|<span data-ttu-id="4415e-154">Код страны пользователя, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="4415e-154">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="4415e-155">tenantCountryCode</span><span class="sxs-lookup"><span data-stu-id="4415e-155">tenantCountryCode</span></span>|<span data-ttu-id="4415e-156">String</span><span class="sxs-lookup"><span data-stu-id="4415e-156">String</span></span>|<span data-ttu-id="4415e-157">Код страны клиента, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="4415e-157">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="4415e-158">connectionCharge</span><span class="sxs-lookup"><span data-stu-id="4415e-158">connectionCharge</span></span>|<span data-ttu-id="4415e-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4415e-159">Double</span></span>|<span data-ttu-id="4415e-160">Цена платы за подключение.</span><span class="sxs-lookup"><span data-stu-id="4415e-160">Connection fee price.</span></span>|
|<span data-ttu-id="4415e-161">callerNumber</span><span class="sxs-lookup"><span data-stu-id="4415e-161">callerNumber</span></span>|<span data-ttu-id="4415e-162">String</span><span class="sxs-lookup"><span data-stu-id="4415e-162">String</span></span>|<span data-ttu-id="4415e-163">Номер, который принял вызов для входящие вызовы, или номер, набираемый для исходящие вызовы.</span><span class="sxs-lookup"><span data-stu-id="4415e-163">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="4415e-164">Формат E.164.</span><span class="sxs-lookup"><span data-stu-id="4415e-164">E.164 format.</span></span>|
|<span data-ttu-id="4415e-165">destinationContext</span><span class="sxs-lookup"><span data-stu-id="4415e-165">destinationContext</span></span>|<span data-ttu-id="4415e-166">String</span><span class="sxs-lookup"><span data-stu-id="4415e-166">String</span></span>|<span data-ttu-id="4415e-167">Был ли звонок внутренним (внутри страны или региона) или международным (за пределами страны или региона) в зависимости от расположения пользователя.</span><span class="sxs-lookup"><span data-stu-id="4415e-167">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="4415e-168">destinationName</span><span class="sxs-lookup"><span data-stu-id="4415e-168">destinationName</span></span>|<span data-ttu-id="4415e-169">String</span><span class="sxs-lookup"><span data-stu-id="4415e-169">String</span></span>|<span data-ttu-id="4415e-170">Страна или регион набрана.</span><span class="sxs-lookup"><span data-stu-id="4415e-170">Country or region dialed.</span></span>|
|<span data-ttu-id="4415e-171">conferenceId</span><span class="sxs-lookup"><span data-stu-id="4415e-171">conferenceId</span></span>|<span data-ttu-id="4415e-172">String</span><span class="sxs-lookup"><span data-stu-id="4415e-172">String</span></span>|<span data-ttu-id="4415e-173">ИД аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="4415e-173">ID of the audio conference.</span></span>|
|<span data-ttu-id="4415e-174">licenseCapability</span><span class="sxs-lookup"><span data-stu-id="4415e-174">licenseCapability</span></span>|<span data-ttu-id="4415e-175">String</span><span class="sxs-lookup"><span data-stu-id="4415e-175">String</span></span>|<span data-ttu-id="4415e-176">Лицензия, используемая для вызова.</span><span class="sxs-lookup"><span data-stu-id="4415e-176">The license used for the call.</span></span>|
|<span data-ttu-id="4415e-177">inventoryType</span><span class="sxs-lookup"><span data-stu-id="4415e-177">inventoryType</span></span>|<span data-ttu-id="4415e-178">String</span><span class="sxs-lookup"><span data-stu-id="4415e-178">String</span></span>|<span data-ttu-id="4415e-179">Тип номера телефона пользователя, например служба бесплатных номеров.</span><span class="sxs-lookup"><span data-stu-id="4415e-179">User's phone number type, such as a service of toll-free number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4415e-180">Связи</span><span class="sxs-lookup"><span data-stu-id="4415e-180">Relationships</span></span>

<span data-ttu-id="4415e-181">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4415e-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4415e-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4415e-182">JSON representation</span></span>

<span data-ttu-id="4415e-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4415e-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.pstnCallLogRow",
  "id": "String (identifier)",
  "callId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "duration": "Integer",
  "charge": "Double",
  "callType": "String",
  "currency": "String",
  "calleeNumber": "String",
  "usageCountryCode": "String",
  "tenantCountryCode": "String",
  "connectionCharge": "Double",
  "callerNumber": "String",
  "destinationContext": "String",
  "destinationName": "String",
  "conferenceId": "String",
  "licenseCapability": "String",
  "inventoryType": "String"
}
```


