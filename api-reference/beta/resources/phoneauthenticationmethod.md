---
title: тип ресурса phoneAuthenticationMethod
description: Представление телефона, зарегистрированного на пользователя.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0cab7a96923f49c77e6d160d68e8746530f8dcf2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964550"
---
# <a name="phoneauthenticationmethod-resource-type"></a><span data-ttu-id="decb3-103">тип ресурса phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="decb3-103">phoneAuthenticationMethod resource type</span></span>

<span data-ttu-id="decb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="decb3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="decb3-105">Представление телефона, зарегистрированного на пользователя.</span><span class="sxs-lookup"><span data-stu-id="decb3-105">A representation of a phone registered to a user.</span></span> <span data-ttu-id="decb3-106">Этот ресурс включает номер телефона, тип телефона и настроен ли телефон, чтобы пользователь вошел с помощью SMS.</span><span class="sxs-lookup"><span data-stu-id="decb3-106">This resource includes the phone number, the phone type, and whether the phone is configured for the user to sign in via SMS.</span></span>

<span data-ttu-id="decb3-107">Телефон имеет один из трех типов: мобильный, альтернативный мобильный или офисный.</span><span class="sxs-lookup"><span data-stu-id="decb3-107">A phone has one of three types: mobile, alternate mobile, or office.</span></span> <span data-ttu-id="decb3-108">Пользователь может иметь один номер, зарегистрированный для каждого типа, и должен иметь мобильный телефон перед добавлением альтернативного мобильного телефона.</span><span class="sxs-lookup"><span data-stu-id="decb3-108">A user can have one number registered for each type, and must have a mobile phone before an alternate mobile phone is added.</span></span> <span data-ttu-id="decb3-109">При использовании телефона для многофакторной проверки подлинности (MFA) или сброса пароля самообслуживления (SSPR) мобильный телефон является по умолчанию, а альтернативный мобильный телефон — резервное копирование.</span><span class="sxs-lookup"><span data-stu-id="decb3-109">When using a phone for multi-factor authentication (MFA) or self-service password reset (SSPR), the mobile phone is the default and the alternate mobile phone is the backup.</span></span> 

<span data-ttu-id="decb3-110">Мобильные телефоны можно использовать как для SMS, так и для голосовых вызовов в зависимости от параметров клиента.</span><span class="sxs-lookup"><span data-stu-id="decb3-110">Mobile phones can be used for both SMS and voice calls, depending on the tenant settings.</span></span>

<span data-ttu-id="decb3-111">Телефон в офисе может принимать только голосовые звонки, а не SMS-сообщения.</span><span class="sxs-lookup"><span data-stu-id="decb3-111">An office phone can only receive voice calls, not SMS messages.</span></span>

## <a name="methods"></a><span data-ttu-id="decb3-112">Методы</span><span class="sxs-lookup"><span data-stu-id="decb3-112">Methods</span></span>

| <span data-ttu-id="decb3-113">Метод</span><span class="sxs-lookup"><span data-stu-id="decb3-113">Method</span></span>       | <span data-ttu-id="decb3-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="decb3-114">Return Type</span></span> | <span data-ttu-id="decb3-115">Описание</span><span class="sxs-lookup"><span data-stu-id="decb3-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="decb3-116">Список</span><span class="sxs-lookup"><span data-stu-id="decb3-116">List</span></span>](../api/Authentication-list-phonemethods.md) | [<span data-ttu-id="decb3-117">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="decb3-117">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="decb3-118">Чтение свойств и связей всех объектов phoneAuthenticationMethod этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="decb3-118">Read properties and relationships of all of this user's phoneAuthenticationMethod objects.</span></span> |
| <span data-ttu-id="decb3-119">[получение](../api/phoneauthenticationmethod-get.md);</span><span class="sxs-lookup"><span data-stu-id="decb3-119">[Get](../api/phoneauthenticationmethod-get.md)</span></span> | [<span data-ttu-id="decb3-120">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="decb3-120">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="decb3-121">Чтение свойств и связей объекта phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="decb3-121">Read properties and relationships of phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="decb3-122">Обновление</span><span class="sxs-lookup"><span data-stu-id="decb3-122">Update</span></span>](../api/phoneauthenticationmethod-update.md) | [<span data-ttu-id="decb3-123">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="decb3-123">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="decb3-124">Обновление объекта phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="decb3-124">Update phoneAuthenticationMethod object.</span></span> |
| <span data-ttu-id="decb3-125">[удаление](../api/phoneauthenticationmethod-delete.md);</span><span class="sxs-lookup"><span data-stu-id="decb3-125">[Delete](../api/phoneauthenticationmethod-delete.md)</span></span> | <span data-ttu-id="decb3-126">Нет</span><span class="sxs-lookup"><span data-stu-id="decb3-126">None</span></span> | <span data-ttu-id="decb3-127">Удаление объекта phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="decb3-127">Delete phoneAuthenticationMethod object.</span></span> |
|[<span data-ttu-id="decb3-128">Отключение подписи SMS</span><span class="sxs-lookup"><span data-stu-id="decb3-128">Disable SMS signin</span></span>](../api/phoneauthenticationmethod-disablesmssignin.md)|<span data-ttu-id="decb3-129">Нет</span><span class="sxs-lookup"><span data-stu-id="decb3-129">None</span></span>|<span data-ttu-id="decb3-130">Отключите вход в SMS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="decb3-130">Turn off SMS sign-in for a user.</span></span>|
|[<span data-ttu-id="decb3-131">Включить подписывку SMS</span><span class="sxs-lookup"><span data-stu-id="decb3-131">Enable SMS signin</span></span>](../api/phoneauthenticationmethod-enablesmssignin.md)|<span data-ttu-id="decb3-132">Нет</span><span class="sxs-lookup"><span data-stu-id="decb3-132">None</span></span>|<span data-ttu-id="decb3-133">Включив вход в SMS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="decb3-133">Turn on SMS sign-in for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="decb3-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="decb3-134">Properties</span></span>

| <span data-ttu-id="decb3-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="decb3-135">Property</span></span>     | <span data-ttu-id="decb3-136">Тип</span><span class="sxs-lookup"><span data-stu-id="decb3-136">Type</span></span>        | <span data-ttu-id="decb3-137">Описание</span><span class="sxs-lookup"><span data-stu-id="decb3-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="decb3-138">id</span><span class="sxs-lookup"><span data-stu-id="decb3-138">id</span></span>|<span data-ttu-id="decb3-139">Строка</span><span class="sxs-lookup"><span data-stu-id="decb3-139">String</span></span>| <span data-ttu-id="decb3-140">Идентификатор этого телефона, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="decb3-140">The identifier of this phone registered to this user.</span></span> <span data-ttu-id="decb3-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="decb3-141">Read-only.</span></span> <br/><br/><span data-ttu-id="decb3-142">Значение id является одним из следующих:</span><span class="sxs-lookup"><span data-stu-id="decb3-142">The value of id is one of the following:</span></span><ul><li><span data-ttu-id="decb3-143">`b6332ec1-7057-4abe-9331-3d72feddfe41` - где **phoneType** `alternateMobile` .</span><span class="sxs-lookup"><span data-stu-id="decb3-143">`b6332ec1-7057-4abe-9331-3d72feddfe41` - where **phoneType** is `alternateMobile`.</span></span></li><li><span data-ttu-id="decb3-144">`e37fc753-ff3b-4958-9484-eaa9425c82bc` - где **phoneType** `office` .</span><span class="sxs-lookup"><span data-stu-id="decb3-144">`e37fc753-ff3b-4958-9484-eaa9425c82bc` - where **phoneType** is `office`.</span></span></li><li><span data-ttu-id="decb3-145">`3179e48a-750b-4051-897c-87b9720928f7` - где **phoneType** `mobile` .</span><span class="sxs-lookup"><span data-stu-id="decb3-145">`3179e48a-750b-4051-897c-87b9720928f7` - where **phoneType** is `mobile`.</span></span></li>|
|<span data-ttu-id="decb3-146">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="decb3-146">phoneNumber</span></span>|<span data-ttu-id="decb3-147">String</span><span class="sxs-lookup"><span data-stu-id="decb3-147">String</span></span>|<span data-ttu-id="decb3-148">Номер телефона для текста или вызова для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="decb3-148">The phone number to text or call for authentication.</span></span> <span data-ttu-id="decb3-149">Номера телефонов используют формат "+ \<country code\> \<number\> \<extension\> x", при этом расширение необязательно.</span><span class="sxs-lookup"><span data-stu-id="decb3-149">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="decb3-150">Например, допустимы +1 5555551234 или +1 5555551234x1233.</span><span class="sxs-lookup"><span data-stu-id="decb3-150">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="decb3-151">При создании и обновлении номера отклоняется, если они не соответствуют требуемой форме.</span><span class="sxs-lookup"><span data-stu-id="decb3-151">Numbers are rejected when creating/updating if they do not match the required format.</span></span> |
|<span data-ttu-id="decb3-152">phoneType</span><span class="sxs-lookup"><span data-stu-id="decb3-152">phoneType</span></span>|<span data-ttu-id="decb3-153">проверка подлинностиPhoneType</span><span class="sxs-lookup"><span data-stu-id="decb3-153">authenticationPhoneType</span></span>|<span data-ttu-id="decb3-154">Тип этого телефона.</span><span class="sxs-lookup"><span data-stu-id="decb3-154">The type of this phone.</span></span> <span data-ttu-id="decb3-155">Возможные значения: `mobile`, `alternateMobile` или `office`.</span><span class="sxs-lookup"><span data-stu-id="decb3-155">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|
|<span data-ttu-id="decb3-156">smsSignInState</span><span class="sxs-lookup"><span data-stu-id="decb3-156">smsSignInState</span></span>|<span data-ttu-id="decb3-157">authenticationMethodSignInState</span><span class="sxs-lookup"><span data-stu-id="decb3-157">authenticationMethodSignInState</span></span>|<span data-ttu-id="decb3-158">Готов ли телефон к входу в SMS или нет.</span><span class="sxs-lookup"><span data-stu-id="decb3-158">Whether a phone is ready to be used for SMS sign-in or not.</span></span> <span data-ttu-id="decb3-159">Возможные значения: `notSupported` `notAllowedByPolicy` , , , , , `notEnabled` или `phoneNumberNotUnique` , `ready` `notConfigured` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="decb3-159">Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, or `notConfigured`, `unknownFutureValue`.</span></span>|

### <a name="smssigninstate-values"></a><span data-ttu-id="decb3-160">значения smsSignInState</span><span class="sxs-lookup"><span data-stu-id="decb3-160">smsSignInState values</span></span>

<span data-ttu-id="decb3-161">Свойство государственного регистрации SMS дает сведения о том, готов ли номер телефона войти с помощью SMS.</span><span class="sxs-lookup"><span data-stu-id="decb3-161">The SMS sign-in state property gives information about whether or not a phone number is ready to sign in via SMS.</span></span> <span data-ttu-id="decb3-162">Ниже возможен вариант значений.</span><span class="sxs-lookup"><span data-stu-id="decb3-162">The following are the possible values.</span></span>

|<span data-ttu-id="decb3-163">Значение</span><span class="sxs-lookup"><span data-stu-id="decb3-163">Value</span></span>|<span data-ttu-id="decb3-164">Описание</span><span class="sxs-lookup"><span data-stu-id="decb3-164">Description</span></span>|
|--------|-----------|
|<span data-ttu-id="decb3-165">notSupported</span><span class="sxs-lookup"><span data-stu-id="decb3-165">notSupported</span></span>|<span data-ttu-id="decb3-166">Основной вход не поддерживается в этом методе проверки подлинности , например, вход можно включить только на основной мобильный номер пользователя, а не на альтернативном номере.</span><span class="sxs-lookup"><span data-stu-id="decb3-166">Primary sign-in not supported on this authentication method - for example, sign-in can be enabled only on a user's primary mobile number, not the alternate number.</span></span>|
|<span data-ttu-id="decb3-167">notAllowedByPolicy</span><span class="sxs-lookup"><span data-stu-id="decb3-167">notAllowedByPolicy</span></span>|<span data-ttu-id="decb3-168">Политика не позволяет этому пользователю использовать этот метод в качестве основного входа.</span><span class="sxs-lookup"><span data-stu-id="decb3-168">This user isn't enabled by policy to use this method as a primary sign-in.</span></span>|
|<span data-ttu-id="decb3-169">notConfigured</span><span class="sxs-lookup"><span data-stu-id="decb3-169">notConfigured</span></span>|<span data-ttu-id="decb3-170">Политика позволяет этому пользователю использовать этот метод в качестве основного входа, но для его настройки необходимо принять дополнительные меры.</span><span class="sxs-lookup"><span data-stu-id="decb3-170">This user is enabled by policy to use this method as primary sign-in but needs to take additional action to configure it.</span></span>|
|<span data-ttu-id="decb3-171">phoneNumberNotUnique</span><span class="sxs-lookup"><span data-stu-id="decb3-171">phoneNumberNotUnique</span></span>|<span data-ttu-id="decb3-172">Этот пользователь попытался настроить номер телефона в качестве основного входного номера, но он не был уникальным и не может использоваться в качестве имени для регистрации.</span><span class="sxs-lookup"><span data-stu-id="decb3-172">This user attempted to set up a phone number as primary sign-in but the number was not unique and can't be used as a sign-in name.</span></span>|
|<span data-ttu-id="decb3-173">готово</span><span class="sxs-lookup"><span data-stu-id="decb3-173">ready</span></span>|<span data-ttu-id="decb3-174">Этот метод проверки подлинности готов к использованию при первичном входе.</span><span class="sxs-lookup"><span data-stu-id="decb3-174">This authentication method is ready for use in primary sign-in.</span></span>|
|<span data-ttu-id="decb3-175">notEnabled</span><span class="sxs-lookup"><span data-stu-id="decb3-175">notEnabled</span></span>|<span data-ttu-id="decb3-176">Этот метод входа не включен</span><span class="sxs-lookup"><span data-stu-id="decb3-176">This sign-in method is not enabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="decb3-177">Связи</span><span class="sxs-lookup"><span data-stu-id="decb3-177">Relationships</span></span>

<span data-ttu-id="decb3-178">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="decb3-178">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="decb3-179">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="decb3-179">JSON representation</span></span>

<span data-ttu-id="decb3-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="decb3-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "string",
  "smsSignInState": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


