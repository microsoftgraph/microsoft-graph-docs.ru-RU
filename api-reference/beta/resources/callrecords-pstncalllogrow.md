---
title: Тип ресурса Пстнкалллогров
description: Представляет строку данных в журнале звонков телефонной сети общего пользования (PSTN).
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa25211831db42f70fef18375e718554029df4de
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071376"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="26bc2-103">Тип ресурса Пстнкалллогров</span><span class="sxs-lookup"><span data-stu-id="26bc2-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="26bc2-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="26bc2-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26bc2-105">Представляет строку данных в журнале звонков телефонной сети общего пользования (PSTN).</span><span class="sxs-lookup"><span data-stu-id="26bc2-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="26bc2-106">Каждая строка соответствует одному вызову.</span><span class="sxs-lookup"><span data-stu-id="26bc2-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="26bc2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="26bc2-107">Properties</span></span>

|<span data-ttu-id="26bc2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="26bc2-108">Property</span></span>|<span data-ttu-id="26bc2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="26bc2-109">Type</span></span>|<span data-ttu-id="26bc2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="26bc2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26bc2-111">id</span><span class="sxs-lookup"><span data-stu-id="26bc2-111">id</span></span>|<span data-ttu-id="26bc2-112">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-112">String</span></span>|<span data-ttu-id="26bc2-113">Уникальный идентификатор звонка.</span><span class="sxs-lookup"><span data-stu-id="26bc2-113">Unique call identifier.</span></span> <span data-ttu-id="26bc2-114">Кодом.</span><span class="sxs-lookup"><span data-stu-id="26bc2-114">GUID.</span></span>|
|<span data-ttu-id="26bc2-115">callId</span><span class="sxs-lookup"><span data-stu-id="26bc2-115">callId</span></span>|<span data-ttu-id="26bc2-116">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-116">String</span></span>|<span data-ttu-id="26bc2-117">Идентификатор вызова.</span><span class="sxs-lookup"><span data-stu-id="26bc2-117">Call identifier.</span></span> <span data-ttu-id="26bc2-118">Не гарантируется уникальным.</span><span class="sxs-lookup"><span data-stu-id="26bc2-118">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="26bc2-119">userId</span><span class="sxs-lookup"><span data-stu-id="26bc2-119">userId</span></span>|<span data-ttu-id="26bc2-120">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-120">String</span></span>|<span data-ttu-id="26bc2-121">Идентификатор вызывающего пользователя в Graph.</span><span class="sxs-lookup"><span data-stu-id="26bc2-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="26bc2-122">Кодом.</span><span class="sxs-lookup"><span data-stu-id="26bc2-122">GUID.</span></span> <span data-ttu-id="26bc2-123">Эта и другие сведения о пользователе будут иметь значение null или Empty для типов вызовов Bot (ucap_in, ucap_out).</span><span class="sxs-lookup"><span data-stu-id="26bc2-123">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="26bc2-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="26bc2-124">userPrincipalName</span></span>|<span data-ttu-id="26bc2-125">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-125">String</span></span>|<span data-ttu-id="26bc2-126">UserPrincipalName (имя входа) в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="26bc2-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="26bc2-127">Обычно это тот же адрес SIP, что и адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="26bc2-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="26bc2-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="26bc2-128">userDisplayName</span></span>|<span data-ttu-id="26bc2-129">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-129">String</span></span>|<span data-ttu-id="26bc2-130">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="26bc2-130">Display name of the user.</span></span>|
|<span data-ttu-id="26bc2-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="26bc2-131">startDateTime</span></span>|<span data-ttu-id="26bc2-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26bc2-132">DateTimeOffset</span></span>|<span data-ttu-id="26bc2-133">Время начала вызова.</span><span class="sxs-lookup"><span data-stu-id="26bc2-133">Call start time.</span></span>|
|<span data-ttu-id="26bc2-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="26bc2-134">endDateTime</span></span>|<span data-ttu-id="26bc2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26bc2-135">DateTimeOffset</span></span>|<span data-ttu-id="26bc2-136">Время окончания вызова.</span><span class="sxs-lookup"><span data-stu-id="26bc2-136">Call end time.</span></span>|
|<span data-ttu-id="26bc2-137">duration</span><span class="sxs-lookup"><span data-stu-id="26bc2-137">duration</span></span>|<span data-ttu-id="26bc2-138">Int32</span><span class="sxs-lookup"><span data-stu-id="26bc2-138">Int32</span></span>|<span data-ttu-id="26bc2-139">Время подключения вызова в секундах.</span><span class="sxs-lookup"><span data-stu-id="26bc2-139">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="26bc2-140">товар</span><span class="sxs-lookup"><span data-stu-id="26bc2-140">charge</span></span>|<span data-ttu-id="26bc2-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="26bc2-141">Double</span></span>|<span data-ttu-id="26bc2-142">Количество денег или затрат на звонок, которые оплачиваются по вашей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="26bc2-142">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="26bc2-143">callType</span><span class="sxs-lookup"><span data-stu-id="26bc2-143">callType</span></span>|<span data-ttu-id="26bc2-144">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-144">String</span></span>|<span data-ttu-id="26bc2-145">Указывает, был ли вызов исходящий или входящий вызов PSTN, и тип вызова, например, поступающий от пользователя или конференции с аудио-и видеосвязи.</span><span class="sxs-lookup"><span data-stu-id="26bc2-145">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="26bc2-146">евро</span><span class="sxs-lookup"><span data-stu-id="26bc2-146">currency</span></span>|<span data-ttu-id="26bc2-147">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-147">String</span></span>|<span data-ttu-id="26bc2-148">Тип валюты, используемой для вычисления стоимости звонка ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span><span class="sxs-lookup"><span data-stu-id="26bc2-148">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="26bc2-149">каллинумбер</span><span class="sxs-lookup"><span data-stu-id="26bc2-149">calleeNumber</span></span>|<span data-ttu-id="26bc2-150">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-150">String</span></span>|<span data-ttu-id="26bc2-151">Номер, набранный в формате [E. 164](https://en.wikipedia.org/wiki/E.164) .</span><span class="sxs-lookup"><span data-stu-id="26bc2-151">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="26bc2-152">усажекаунтрикоде</span><span class="sxs-lookup"><span data-stu-id="26bc2-152">usageCountryCode</span></span>|<span data-ttu-id="26bc2-153">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-153">String</span></span>|<span data-ttu-id="26bc2-154">Код страны пользователя, [ISO 3166-1 Alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="26bc2-154">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="26bc2-155">тенанткаунтрикоде</span><span class="sxs-lookup"><span data-stu-id="26bc2-155">tenantCountryCode</span></span>|<span data-ttu-id="26bc2-156">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-156">String</span></span>|<span data-ttu-id="26bc2-157">Код страны клиента, [ISO 3166-1 Alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="26bc2-157">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="26bc2-158">коннектиончарже</span><span class="sxs-lookup"><span data-stu-id="26bc2-158">connectionCharge</span></span>|<span data-ttu-id="26bc2-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="26bc2-159">Double</span></span>|<span data-ttu-id="26bc2-160">Цена оплаты по подключению.</span><span class="sxs-lookup"><span data-stu-id="26bc2-160">Connection fee price.</span></span>|
|<span data-ttu-id="26bc2-161">каллернумбер</span><span class="sxs-lookup"><span data-stu-id="26bc2-161">callerNumber</span></span>|<span data-ttu-id="26bc2-162">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-162">String</span></span>|<span data-ttu-id="26bc2-163">Номер, который получил вызов для входящих звонков или номер, набранный для исходящих звонков.</span><span class="sxs-lookup"><span data-stu-id="26bc2-163">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="26bc2-164">Формат E. 164.</span><span class="sxs-lookup"><span data-stu-id="26bc2-164">E.164 format.</span></span>|
|<span data-ttu-id="26bc2-165">дестинатионконтекст</span><span class="sxs-lookup"><span data-stu-id="26bc2-165">destinationContext</span></span>|<span data-ttu-id="26bc2-166">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-166">String</span></span>|<span data-ttu-id="26bc2-167">Указывает, является ли вызов внутренним (в стране или регионе) или международным (за пределами страны или региона) на основе расположения пользователя.</span><span class="sxs-lookup"><span data-stu-id="26bc2-167">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="26bc2-168">дестинатионнаме</span><span class="sxs-lookup"><span data-stu-id="26bc2-168">destinationName</span></span>|<span data-ttu-id="26bc2-169">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-169">String</span></span>|<span data-ttu-id="26bc2-170">Страна или регион набора.</span><span class="sxs-lookup"><span data-stu-id="26bc2-170">Country or region dialed.</span></span>|
|<span data-ttu-id="26bc2-171">конференцеид</span><span class="sxs-lookup"><span data-stu-id="26bc2-171">conferenceId</span></span>|<span data-ttu-id="26bc2-172">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-172">String</span></span>|<span data-ttu-id="26bc2-173">Идентификатор конференции с аудио-и видеосвязи.</span><span class="sxs-lookup"><span data-stu-id="26bc2-173">ID of the audio conference.</span></span>|
|<span data-ttu-id="26bc2-174">лиценсекапабилити</span><span class="sxs-lookup"><span data-stu-id="26bc2-174">licenseCapability</span></span>|<span data-ttu-id="26bc2-175">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-175">String</span></span>|<span data-ttu-id="26bc2-176">Лицензия, используемая для вызова.</span><span class="sxs-lookup"><span data-stu-id="26bc2-176">The license used for the call.</span></span>|
|<span data-ttu-id="26bc2-177">инвенторитипе</span><span class="sxs-lookup"><span data-stu-id="26bc2-177">inventoryType</span></span>|<span data-ttu-id="26bc2-178">String</span><span class="sxs-lookup"><span data-stu-id="26bc2-178">String</span></span>|<span data-ttu-id="26bc2-179">Тип номера телефона пользователя, например услуга бесплатных номеров.</span><span class="sxs-lookup"><span data-stu-id="26bc2-179">User's phone number type, such as a service of toll-free number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26bc2-180">Отношения</span><span class="sxs-lookup"><span data-stu-id="26bc2-180">Relationships</span></span>

<span data-ttu-id="26bc2-181">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="26bc2-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26bc2-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="26bc2-182">JSON representation</span></span>

<span data-ttu-id="26bc2-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26bc2-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "baseType": "",
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


