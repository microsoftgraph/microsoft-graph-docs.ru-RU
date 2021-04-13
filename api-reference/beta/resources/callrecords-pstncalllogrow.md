---
title: тип ресурсов pstnCallLogRow
description: Представляет строку данных в журнале вызовов для общедоступных телефонных сетей коммутатора (PSTN).
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 584efcd6e320a95dc6e62f59b112d1041535f054
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697174"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="72ac4-103">тип ресурсов pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="72ac4-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="72ac4-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="72ac4-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72ac4-105">Представляет строку данных в журнале вызовов для общедоступных телефонных сетей коммутатора (PSTN).</span><span class="sxs-lookup"><span data-stu-id="72ac4-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="72ac4-106">Каждая строка сопомна одному вызову.</span><span class="sxs-lookup"><span data-stu-id="72ac4-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="72ac4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="72ac4-107">Properties</span></span>

|<span data-ttu-id="72ac4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="72ac4-108">Property</span></span>|<span data-ttu-id="72ac4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="72ac4-109">Type</span></span>|<span data-ttu-id="72ac4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="72ac4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72ac4-111">callDurationSource</span><span class="sxs-lookup"><span data-stu-id="72ac4-111">callDurationSource</span></span>|<span data-ttu-id="72ac4-112">pstnCallDurationSource</span><span class="sxs-lookup"><span data-stu-id="72ac4-112">pstnCallDurationSource</span></span>|<span data-ttu-id="72ac4-113">Источник данных о продолжительности вызова.</span><span class="sxs-lookup"><span data-stu-id="72ac4-113">The source of the call duration data.</span></span> <span data-ttu-id="72ac4-114">Если при вызове используется сторонний оператор связи через программу "Подключение оператора", оператор может предоставить собственные данные о продолжительности вызова.</span><span class="sxs-lookup"><span data-stu-id="72ac4-114">If the call uses a third-party telecommunications operator via the Operator Connect Program, the operator may provide their own call duration data.</span></span> <span data-ttu-id="72ac4-115">В этом случае значение свойства `operator` .</span><span class="sxs-lookup"><span data-stu-id="72ac4-115">In this case, the property value is `operator`.</span></span> <span data-ttu-id="72ac4-116">В противном случае значение `microsoft` .</span><span class="sxs-lookup"><span data-stu-id="72ac4-116">Otherwise, the value is `microsoft`.</span></span>|
|<span data-ttu-id="72ac4-117">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="72ac4-117">calleeNumber</span></span>|<span data-ttu-id="72ac4-118">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-118">String</span></span>|<span data-ttu-id="72ac4-119">Номер, набраный [в формате E.164.](https://en.wikipedia.org/wiki/E.164)</span><span class="sxs-lookup"><span data-stu-id="72ac4-119">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="72ac4-120">callerNumber</span><span class="sxs-lookup"><span data-stu-id="72ac4-120">callerNumber</span></span>|<span data-ttu-id="72ac4-121">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-121">String</span></span>|<span data-ttu-id="72ac4-122">Номер, который получил вызов для входящие вызовы или номер, набраный для исходящие вызовы.</span><span class="sxs-lookup"><span data-stu-id="72ac4-122">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="72ac4-123">Формат E.164.</span><span class="sxs-lookup"><span data-stu-id="72ac4-123">E.164 format.</span></span>|
|<span data-ttu-id="72ac4-124">callId</span><span class="sxs-lookup"><span data-stu-id="72ac4-124">callId</span></span>|<span data-ttu-id="72ac4-125">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-125">String</span></span>|<span data-ttu-id="72ac4-126">Идентификатор вызова.</span><span class="sxs-lookup"><span data-stu-id="72ac4-126">Call identifier.</span></span> <span data-ttu-id="72ac4-127">Не гарантируется уникальность.</span><span class="sxs-lookup"><span data-stu-id="72ac4-127">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="72ac4-128">callType</span><span class="sxs-lookup"><span data-stu-id="72ac4-128">callType</span></span>|<span data-ttu-id="72ac4-129">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-129">String</span></span>|<span data-ttu-id="72ac4-130">Был ли вызов исходящие или входящие вызовы PSTN и тип вызова, например вызов, размещенный пользователем или аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="72ac4-130">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="72ac4-131">заряд</span><span class="sxs-lookup"><span data-stu-id="72ac4-131">charge</span></span>|<span data-ttu-id="72ac4-132">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="72ac4-132">Double</span></span>|<span data-ttu-id="72ac4-133">Сумма денег или стоимость звонка, который взимается с вашей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="72ac4-133">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="72ac4-134">conferenceId</span><span class="sxs-lookup"><span data-stu-id="72ac4-134">conferenceId</span></span>|<span data-ttu-id="72ac4-135">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-135">String</span></span>|<span data-ttu-id="72ac4-136">ID аудиоконференции.</span><span class="sxs-lookup"><span data-stu-id="72ac4-136">ID of the audio conference.</span></span>|
|<span data-ttu-id="72ac4-137">connectionCharge</span><span class="sxs-lookup"><span data-stu-id="72ac4-137">connectionCharge</span></span>|<span data-ttu-id="72ac4-138">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="72ac4-138">Double</span></span>|<span data-ttu-id="72ac4-139">Цена платы за подключение.</span><span class="sxs-lookup"><span data-stu-id="72ac4-139">Connection fee price.</span></span>|
|<span data-ttu-id="72ac4-140">валюта</span><span class="sxs-lookup"><span data-stu-id="72ac4-140">currency</span></span>|<span data-ttu-id="72ac4-141">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-141">String</span></span>|<span data-ttu-id="72ac4-142">Тип валюты, используемой для расчета стоимости вызова[(ISO 4217).](https://en.wikipedia.org/wiki/ISO_4217)</span><span class="sxs-lookup"><span data-stu-id="72ac4-142">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="72ac4-143">destinationContext</span><span class="sxs-lookup"><span data-stu-id="72ac4-143">destinationContext</span></span>|<span data-ttu-id="72ac4-144">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-144">String</span></span>|<span data-ttu-id="72ac4-145">Был ли вызов внутренним (в пределах страны или региона) или международным (за пределами страны или региона) в зависимости от расположения пользователя.</span><span class="sxs-lookup"><span data-stu-id="72ac4-145">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="72ac4-146">destinationName</span><span class="sxs-lookup"><span data-stu-id="72ac4-146">destinationName</span></span>|<span data-ttu-id="72ac4-147">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-147">String</span></span>|<span data-ttu-id="72ac4-148">Страна или регион, набрана.</span><span class="sxs-lookup"><span data-stu-id="72ac4-148">Country or region dialed.</span></span>|
|<span data-ttu-id="72ac4-149">duration</span><span class="sxs-lookup"><span data-stu-id="72ac4-149">duration</span></span>|<span data-ttu-id="72ac4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="72ac4-150">Int32</span></span>|<span data-ttu-id="72ac4-151">Сколько времени вызов был подключен, в секундах.</span><span class="sxs-lookup"><span data-stu-id="72ac4-151">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="72ac4-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="72ac4-152">endDateTime</span></span>|<span data-ttu-id="72ac4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72ac4-153">DateTimeOffset</span></span>|<span data-ttu-id="72ac4-154">Время окончания вызова.</span><span class="sxs-lookup"><span data-stu-id="72ac4-154">Call end time.</span></span>|
|<span data-ttu-id="72ac4-155">id</span><span class="sxs-lookup"><span data-stu-id="72ac4-155">id</span></span>|<span data-ttu-id="72ac4-156">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-156">String</span></span>|<span data-ttu-id="72ac4-157">Уникальный идентификатор вызовов.</span><span class="sxs-lookup"><span data-stu-id="72ac4-157">Unique call identifier.</span></span> <span data-ttu-id="72ac4-158">GUID.</span><span class="sxs-lookup"><span data-stu-id="72ac4-158">GUID.</span></span>|
|<span data-ttu-id="72ac4-159">inventoryType</span><span class="sxs-lookup"><span data-stu-id="72ac4-159">inventoryType</span></span>|<span data-ttu-id="72ac4-160">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-160">String</span></span>|<span data-ttu-id="72ac4-161">Тип номера телефона пользователя, например служба бесплатного номера.</span><span class="sxs-lookup"><span data-stu-id="72ac4-161">User's phone number type, such as a service of toll-free number.</span></span>|
|<span data-ttu-id="72ac4-162">licenseCapability</span><span class="sxs-lookup"><span data-stu-id="72ac4-162">licenseCapability</span></span>|<span data-ttu-id="72ac4-163">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-163">String</span></span>|<span data-ttu-id="72ac4-164">Лицензия, используемая для вызова.</span><span class="sxs-lookup"><span data-stu-id="72ac4-164">The license used for the call.</span></span>|
|<span data-ttu-id="72ac4-165">operator</span><span class="sxs-lookup"><span data-stu-id="72ac4-165">operator</span></span>|<span data-ttu-id="72ac4-166">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-166">String</span></span>|<span data-ttu-id="72ac4-167">Оператор связи, предоставлял службы PSTN для этого вызова.</span><span class="sxs-lookup"><span data-stu-id="72ac4-167">The telecommunications operator which provided PSTN services for this call.</span></span> <span data-ttu-id="72ac4-168">Это может быть Корпорация Майкрософт или сторонний оператор через [программу подключения оператора.](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398)</span><span class="sxs-lookup"><span data-stu-id="72ac4-168">This may be Microsoft, or it may be a third-party operator via the [Operator Connect Program](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398).</span></span>|
|<span data-ttu-id="72ac4-169">startDateTime</span><span class="sxs-lookup"><span data-stu-id="72ac4-169">startDateTime</span></span>|<span data-ttu-id="72ac4-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72ac4-170">DateTimeOffset</span></span>|<span data-ttu-id="72ac4-171">Время начала вызова.</span><span class="sxs-lookup"><span data-stu-id="72ac4-171">Call start time.</span></span>|
|<span data-ttu-id="72ac4-172">tenantCountryCode</span><span class="sxs-lookup"><span data-stu-id="72ac4-172">tenantCountryCode</span></span>|<span data-ttu-id="72ac4-173">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-173">String</span></span>|<span data-ttu-id="72ac4-174">Код страны клиента [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="72ac4-174">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="72ac4-175">useCountryCode</span><span class="sxs-lookup"><span data-stu-id="72ac4-175">usageCountryCode</span></span>|<span data-ttu-id="72ac4-176">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-176">String</span></span>|<span data-ttu-id="72ac4-177">Код страны пользователя [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="72ac4-177">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="72ac4-178">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="72ac4-178">userDisplayName</span></span>|<span data-ttu-id="72ac4-179">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-179">String</span></span>|<span data-ttu-id="72ac4-180">Отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="72ac4-180">Display name of the user.</span></span>|
|<span data-ttu-id="72ac4-181">userId</span><span class="sxs-lookup"><span data-stu-id="72ac4-181">userId</span></span>|<span data-ttu-id="72ac4-182">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-182">String</span></span>|<span data-ttu-id="72ac4-183">Вызов ID пользователя в Графе.</span><span class="sxs-lookup"><span data-stu-id="72ac4-183">Calling user's ID in Graph.</span></span> <span data-ttu-id="72ac4-184">GUID.</span><span class="sxs-lookup"><span data-stu-id="72ac4-184">GUID.</span></span> <span data-ttu-id="72ac4-185">Эта и другие сведения о пользователях будут null/empty для типов вызовов ботов (ucap_in, ucap_out).</span><span class="sxs-lookup"><span data-stu-id="72ac4-185">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="72ac4-186">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="72ac4-186">userPrincipalName</span></span>|<span data-ttu-id="72ac4-187">String</span><span class="sxs-lookup"><span data-stu-id="72ac4-187">String</span></span>|<span data-ttu-id="72ac4-188">UserPrincipalName (имя регистрации) в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="72ac4-188">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="72ac4-189">Это обычно то же самое, что и SIP-адрес пользователя, и может быть таким же, как и адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="72ac4-189">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72ac4-190">Связи</span><span class="sxs-lookup"><span data-stu-id="72ac4-190">Relationships</span></span>

<span data-ttu-id="72ac4-191">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72ac4-191">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72ac4-192">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="72ac4-192">JSON representation</span></span>

<span data-ttu-id="72ac4-193">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72ac4-193">The following is a JSON representation of the resource.</span></span>

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
  "inventoryType": "String",
  "operator": "String",
  "callDurationSource": "String"
}
```


