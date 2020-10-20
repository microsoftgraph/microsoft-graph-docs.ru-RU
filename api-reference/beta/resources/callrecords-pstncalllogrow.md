---
title: Тип ресурса Пстнкалллогров
description: Представляет строку данных в журнале звонков телефонной сети общего пользования (PSTN).
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bc83f3304eeb918d665b2651fda9809fd8a05880
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601673"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="0f9ee-103">Тип ресурса Пстнкалллогров</span><span class="sxs-lookup"><span data-stu-id="0f9ee-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="0f9ee-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="0f9ee-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f9ee-105">Представляет строку данных в журнале звонков телефонной сети общего пользования (PSTN).</span><span class="sxs-lookup"><span data-stu-id="0f9ee-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="0f9ee-106">Каждая строка соответствует одному вызову.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="0f9ee-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f9ee-107">Properties</span></span>

|<span data-ttu-id="0f9ee-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f9ee-108">Property</span></span>|<span data-ttu-id="0f9ee-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0f9ee-109">Type</span></span>|<span data-ttu-id="0f9ee-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0f9ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f9ee-111">id</span><span class="sxs-lookup"><span data-stu-id="0f9ee-111">id</span></span>|<span data-ttu-id="0f9ee-112">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-112">String</span></span>|<span data-ttu-id="0f9ee-113">Уникальный идентификатор звонка.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-113">Unique call identifier.</span></span> <span data-ttu-id="0f9ee-114">Кодом.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-114">GUID.</span></span>|
|<span data-ttu-id="0f9ee-115">callId</span><span class="sxs-lookup"><span data-stu-id="0f9ee-115">callId</span></span>|<span data-ttu-id="0f9ee-116">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-116">String</span></span>|<span data-ttu-id="0f9ee-117">Идентификатор вызова.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-117">Call identifier.</span></span> <span data-ttu-id="0f9ee-118">Не гарантируется уникальным.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-118">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="0f9ee-119">userId</span><span class="sxs-lookup"><span data-stu-id="0f9ee-119">userId</span></span>|<span data-ttu-id="0f9ee-120">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-120">String</span></span>|<span data-ttu-id="0f9ee-121">Идентификатор вызывающего пользователя в Graph.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="0f9ee-122">Кодом.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-122">GUID.</span></span> <span data-ttu-id="0f9ee-123">Эта и другие сведения о пользователе будут иметь значение null или Empty для типов вызовов Bot (ucap_in, ucap_out).</span><span class="sxs-lookup"><span data-stu-id="0f9ee-123">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="0f9ee-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0f9ee-124">userPrincipalName</span></span>|<span data-ttu-id="0f9ee-125">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-125">String</span></span>|<span data-ttu-id="0f9ee-126">UserPrincipalName (имя входа) в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="0f9ee-127">Обычно это тот же адрес SIP, что и адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="0f9ee-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="0f9ee-128">userDisplayName</span></span>|<span data-ttu-id="0f9ee-129">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-129">String</span></span>|<span data-ttu-id="0f9ee-130">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-130">Display name of the user.</span></span>|
|<span data-ttu-id="0f9ee-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0f9ee-131">startDateTime</span></span>|<span data-ttu-id="0f9ee-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f9ee-132">DateTimeOffset</span></span>|<span data-ttu-id="0f9ee-133">Время начала вызова.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-133">Call start time.</span></span>|
|<span data-ttu-id="0f9ee-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0f9ee-134">endDateTime</span></span>|<span data-ttu-id="0f9ee-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f9ee-135">DateTimeOffset</span></span>|<span data-ttu-id="0f9ee-136">Время окончания вызова.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-136">Call end time.</span></span>|
|<span data-ttu-id="0f9ee-137">duration</span><span class="sxs-lookup"><span data-stu-id="0f9ee-137">duration</span></span>|<span data-ttu-id="0f9ee-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0f9ee-138">Int32</span></span>|<span data-ttu-id="0f9ee-139">Время подключения вызова в секундах.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-139">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="0f9ee-140">товар</span><span class="sxs-lookup"><span data-stu-id="0f9ee-140">charge</span></span>|<span data-ttu-id="0f9ee-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0f9ee-141">Double</span></span>|<span data-ttu-id="0f9ee-142">Количество денег или затрат на звонок, которые оплачиваются по вашей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-142">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="0f9ee-143">callType</span><span class="sxs-lookup"><span data-stu-id="0f9ee-143">callType</span></span>|<span data-ttu-id="0f9ee-144">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-144">String</span></span>|<span data-ttu-id="0f9ee-145">Указывает, был ли вызов исходящий или входящий вызов PSTN, и тип вызова, например, поступающий от пользователя или конференции с аудио-и видеосвязи.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-145">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="0f9ee-146">евро</span><span class="sxs-lookup"><span data-stu-id="0f9ee-146">currency</span></span>|<span data-ttu-id="0f9ee-147">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-147">String</span></span>|<span data-ttu-id="0f9ee-148">Тип валюты, используемой для вычисления стоимости звонка ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span><span class="sxs-lookup"><span data-stu-id="0f9ee-148">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="0f9ee-149">каллинумбер</span><span class="sxs-lookup"><span data-stu-id="0f9ee-149">calleeNumber</span></span>|<span data-ttu-id="0f9ee-150">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-150">String</span></span>|<span data-ttu-id="0f9ee-151">Номер, набранный в формате [E. 164](https://en.wikipedia.org/wiki/E.164) .</span><span class="sxs-lookup"><span data-stu-id="0f9ee-151">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="0f9ee-152">усажекаунтрикоде</span><span class="sxs-lookup"><span data-stu-id="0f9ee-152">usageCountryCode</span></span>|<span data-ttu-id="0f9ee-153">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-153">String</span></span>|<span data-ttu-id="0f9ee-154">Код страны пользователя, [ISO 3166-1 Alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="0f9ee-154">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="0f9ee-155">тенанткаунтрикоде</span><span class="sxs-lookup"><span data-stu-id="0f9ee-155">tenantCountryCode</span></span>|<span data-ttu-id="0f9ee-156">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-156">String</span></span>|<span data-ttu-id="0f9ee-157">Код страны клиента, [ISO 3166-1 Alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="0f9ee-157">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="0f9ee-158">коннектиончарже</span><span class="sxs-lookup"><span data-stu-id="0f9ee-158">connectionCharge</span></span>|<span data-ttu-id="0f9ee-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0f9ee-159">Double</span></span>|<span data-ttu-id="0f9ee-160">Цена оплаты по подключению.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-160">Connection fee price.</span></span>|
|<span data-ttu-id="0f9ee-161">каллернумбер</span><span class="sxs-lookup"><span data-stu-id="0f9ee-161">callerNumber</span></span>|<span data-ttu-id="0f9ee-162">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-162">String</span></span>|<span data-ttu-id="0f9ee-163">Номер, который получил вызов для входящих звонков или номер, набранный для исходящих звонков.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-163">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="0f9ee-164">Формат E. 164.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-164">E.164 format.</span></span>|
|<span data-ttu-id="0f9ee-165">дестинатионконтекст</span><span class="sxs-lookup"><span data-stu-id="0f9ee-165">destinationContext</span></span>|<span data-ttu-id="0f9ee-166">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-166">String</span></span>|<span data-ttu-id="0f9ee-167">Указывает, является ли вызов внутренним (в стране или регионе) или международным (за пределами страны или региона) на основе расположения пользователя.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-167">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="0f9ee-168">дестинатионнаме</span><span class="sxs-lookup"><span data-stu-id="0f9ee-168">destinationName</span></span>|<span data-ttu-id="0f9ee-169">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-169">String</span></span>|<span data-ttu-id="0f9ee-170">Страна или регион набора.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-170">Country or region dialed.</span></span>|
|<span data-ttu-id="0f9ee-171">конференцеид</span><span class="sxs-lookup"><span data-stu-id="0f9ee-171">conferenceId</span></span>|<span data-ttu-id="0f9ee-172">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-172">String</span></span>|<span data-ttu-id="0f9ee-173">Идентификатор конференции с аудио-и видеосвязи.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-173">ID of the audio conference.</span></span>|
|<span data-ttu-id="0f9ee-174">лиценсекапабилити</span><span class="sxs-lookup"><span data-stu-id="0f9ee-174">licenseCapability</span></span>|<span data-ttu-id="0f9ee-175">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-175">String</span></span>|<span data-ttu-id="0f9ee-176">Лицензия, используемая для вызова.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-176">The license used for the call.</span></span>|
|<span data-ttu-id="0f9ee-177">инвенторитипе</span><span class="sxs-lookup"><span data-stu-id="0f9ee-177">inventoryType</span></span>|<span data-ttu-id="0f9ee-178">String</span><span class="sxs-lookup"><span data-stu-id="0f9ee-178">String</span></span>|<span data-ttu-id="0f9ee-179">Тип номера телефона пользователя, например услуга бесплатных номеров.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-179">User's phone number type, such as a service of toll-free number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f9ee-180">Связи</span><span class="sxs-lookup"><span data-stu-id="0f9ee-180">Relationships</span></span>

<span data-ttu-id="0f9ee-181">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f9ee-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0f9ee-182">JSON representation</span></span>

<span data-ttu-id="0f9ee-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f9ee-183">The following is a JSON representation of the resource.</span></span>

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


