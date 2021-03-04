---
title: тип ресурса phoneAuthenticationMethod
description: Представление телефона, зарегистрированного на пользователя.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2d0ec89e21ff6ab7aa39b05acabd81c2b22bd54f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442903"
---
# <a name="phoneauthenticationmethod-resource-type"></a><span data-ttu-id="97091-103">тип ресурса phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="97091-103">phoneAuthenticationMethod resource type</span></span>

<span data-ttu-id="97091-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97091-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97091-105">Представление телефона, зарегистрированного на пользователя.</span><span class="sxs-lookup"><span data-stu-id="97091-105">A representation of a phone registered to a user.</span></span> <span data-ttu-id="97091-106">Этот ресурс включает номер телефона, тип телефона и настроен ли телефон, чтобы пользователь вошел с помощью SMS.</span><span class="sxs-lookup"><span data-stu-id="97091-106">This resource includes the phone number, the phone type, and whether the phone is configured for the user to sign in via SMS.</span></span>

<span data-ttu-id="97091-107">Телефон имеет один из трех типов: мобильный, альтернативный мобильный или офисный.</span><span class="sxs-lookup"><span data-stu-id="97091-107">A phone has one of three types: mobile, alternate mobile, or office.</span></span> <span data-ttu-id="97091-108">Пользователь может иметь один номер, зарегистрированный для каждого типа, и должен иметь мобильный телефон перед добавлением альтернативного мобильного телефона.</span><span class="sxs-lookup"><span data-stu-id="97091-108">A user can have one number registered for each type, and must have a mobile phone before an alternate mobile phone is added.</span></span> <span data-ttu-id="97091-109">При использовании телефона для многофакторной проверки подлинности (MFA) или сброса пароля самообслуживления (SSPR) мобильный телефон является по умолчанию, а альтернативный мобильный телефон — резервное копирование.</span><span class="sxs-lookup"><span data-stu-id="97091-109">When using a phone for multi-factor authentication (MFA) or self-service password reset (SSPR), the mobile phone is the default and the alternate mobile phone is the backup.</span></span> 

<span data-ttu-id="97091-110">Мобильные телефоны можно использовать как для SMS, так и для голосовых вызовов в зависимости от параметров клиента.</span><span class="sxs-lookup"><span data-stu-id="97091-110">Mobile phones can be used for both SMS and voice calls, depending on the tenant settings.</span></span>

<span data-ttu-id="97091-111">Телефон в офисе может принимать только голосовые звонки, а не SMS-сообщения.</span><span class="sxs-lookup"><span data-stu-id="97091-111">An office phone can only receive voice calls, not SMS messages.</span></span>

<span data-ttu-id="97091-112">Свойство государственного регистрации SMS дает сведения о том, готов ли номер телефона войти с помощью SMS.</span><span class="sxs-lookup"><span data-stu-id="97091-112">The SMS sign-in state property gives information about whether or not a phone number is ready to sign in via SMS.</span></span> <span data-ttu-id="97091-113">Ниже возможен вариант значений.</span><span class="sxs-lookup"><span data-stu-id="97091-113">The following are the possible values.</span></span>

|<span data-ttu-id="97091-114">Значение</span><span class="sxs-lookup"><span data-stu-id="97091-114">Value</span></span>|<span data-ttu-id="97091-115">Описание</span><span class="sxs-lookup"><span data-stu-id="97091-115">Description</span></span>|
|--------|-----------|
|`notSupported`|<span data-ttu-id="97091-116">Основной вход не поддерживается в этом методе проверки подлинности , например, вход можно включить только на основной мобильный номер пользователя, а не на альтернативном номере.</span><span class="sxs-lookup"><span data-stu-id="97091-116">Primary sign-in not supported on this authentication method - for example, sign-in can be enabled only on a user's primary mobile number, not the alternate number.</span></span>|
|`notAllowedByPolicy`|<span data-ttu-id="97091-117">Политика не позволяет этому пользователю использовать этот метод в качестве основного входа.</span><span class="sxs-lookup"><span data-stu-id="97091-117">This user isn't enabled by policy to use this method as a primary sign-in.</span></span>|
|`notConfigured`|<span data-ttu-id="97091-118">Политика позволяет этому пользователю использовать этот метод в качестве основного входа, но для его настройки необходимо принять дополнительные меры.</span><span class="sxs-lookup"><span data-stu-id="97091-118">This user is enabled by policy to use this method as primary sign-in but needs to take additional action to configure it.</span></span>|
|`phoneNumberNotUnique`|<span data-ttu-id="97091-119">Этот пользователь попытался настроить номер телефона в качестве основного входного номера, но он не был уникальным и не может использоваться в качестве имени для регистрации.</span><span class="sxs-lookup"><span data-stu-id="97091-119">This user attempted to set up a phone number as primary sign-in but the number was not unique and can't be used as a sign-in name.</span></span>|
|`ready`|<span data-ttu-id="97091-120">Этот метод проверки подлинности готов к использованию при первичном входе.</span><span class="sxs-lookup"><span data-stu-id="97091-120">This authentication method is ready for use in primary sign-in.</span></span>|

## <a name="methods"></a><span data-ttu-id="97091-121">Методы</span><span class="sxs-lookup"><span data-stu-id="97091-121">Methods</span></span>

| <span data-ttu-id="97091-122">Метод</span><span class="sxs-lookup"><span data-stu-id="97091-122">Method</span></span>       | <span data-ttu-id="97091-123">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="97091-123">Return Type</span></span> | <span data-ttu-id="97091-124">Описание</span><span class="sxs-lookup"><span data-stu-id="97091-124">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="97091-125">Список</span><span class="sxs-lookup"><span data-stu-id="97091-125">List</span></span>](../api/Authentication-list-phonemethods.md) | [<span data-ttu-id="97091-126">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="97091-126">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="97091-127">Чтение свойств и связей всех объектов phoneAuthenticationMethod этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="97091-127">Read properties and relationships of all of this user's phoneAuthenticationMethod objects.</span></span> |
| <span data-ttu-id="97091-128">[получение](../api/phoneauthenticationmethod-get.md);</span><span class="sxs-lookup"><span data-stu-id="97091-128">[Get](../api/phoneauthenticationmethod-get.md)</span></span> | [<span data-ttu-id="97091-129">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="97091-129">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="97091-130">Чтение свойств и связей объекта phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="97091-130">Read properties and relationships of phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="97091-131">Обновление</span><span class="sxs-lookup"><span data-stu-id="97091-131">Update</span></span>](../api/phoneauthenticationmethod-update.md) | [<span data-ttu-id="97091-132">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="97091-132">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="97091-133">Обновление объекта phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="97091-133">Update phoneAuthenticationMethod object.</span></span> |
| <span data-ttu-id="97091-134">[удаление](../api/phoneauthenticationmethod-delete.md);</span><span class="sxs-lookup"><span data-stu-id="97091-134">[Delete](../api/phoneauthenticationmethod-delete.md)</span></span> | <span data-ttu-id="97091-135">Нет</span><span class="sxs-lookup"><span data-stu-id="97091-135">None</span></span> | <span data-ttu-id="97091-136">Удаление объекта phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="97091-136">Delete phoneAuthenticationMethod object.</span></span> |
|[<span data-ttu-id="97091-137">Отключение подписи SMS</span><span class="sxs-lookup"><span data-stu-id="97091-137">Disable SMS signin</span></span>](../api/phoneauthenticationmethod-disablesmssignin.md)|<span data-ttu-id="97091-138">Нет</span><span class="sxs-lookup"><span data-stu-id="97091-138">None</span></span>|<span data-ttu-id="97091-139">Отключите вход в SMS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="97091-139">Turn off SMS sign-in for a user.</span></span>|
|[<span data-ttu-id="97091-140">Включить подписывку SMS</span><span class="sxs-lookup"><span data-stu-id="97091-140">Enable SMS signin</span></span>](../api/phoneauthenticationmethod-enablesmssignin.md)|<span data-ttu-id="97091-141">Нет</span><span class="sxs-lookup"><span data-stu-id="97091-141">None</span></span>|<span data-ttu-id="97091-142">Включив вход в SMS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="97091-142">Turn on SMS sign-in for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="97091-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="97091-143">Properties</span></span>

| <span data-ttu-id="97091-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="97091-144">Property</span></span>     | <span data-ttu-id="97091-145">Тип</span><span class="sxs-lookup"><span data-stu-id="97091-145">Type</span></span>        | <span data-ttu-id="97091-146">Описание</span><span class="sxs-lookup"><span data-stu-id="97091-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97091-147">id</span><span class="sxs-lookup"><span data-stu-id="97091-147">id</span></span>|<span data-ttu-id="97091-148">String</span><span class="sxs-lookup"><span data-stu-id="97091-148">String</span></span>| <span data-ttu-id="97091-149">Идентификатор этого телефона, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="97091-149">The identifier of this phone registered to this user.</span></span> <span data-ttu-id="97091-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="97091-150">Read-only.</span></span>|
|<span data-ttu-id="97091-151">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="97091-151">phoneNumber</span></span>|<span data-ttu-id="97091-152">String</span><span class="sxs-lookup"><span data-stu-id="97091-152">String</span></span>|<span data-ttu-id="97091-153">Номер телефона для текста или вызова для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="97091-153">The phone number to text or call for authentication.</span></span> <span data-ttu-id="97091-154">Номера телефонов используют формат "+ \<country code\> \<number\> \<extension\> x", при этом расширение необязательно.</span><span class="sxs-lookup"><span data-stu-id="97091-154">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="97091-155">Например, допустимы +1 5555551234 или +1 5555551234x1233.</span><span class="sxs-lookup"><span data-stu-id="97091-155">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="97091-156">При создании и обновлении номера отклоняется, если они не соответствуют требуемой форме.</span><span class="sxs-lookup"><span data-stu-id="97091-156">Numbers are rejected when creating/updating if they do not match the required format.</span></span> |
|<span data-ttu-id="97091-157">phoneType</span><span class="sxs-lookup"><span data-stu-id="97091-157">phoneType</span></span>|<span data-ttu-id="97091-158">string</span><span class="sxs-lookup"><span data-stu-id="97091-158">string</span></span>|<span data-ttu-id="97091-159">Тип этого телефона.</span><span class="sxs-lookup"><span data-stu-id="97091-159">The type of this phone.</span></span> <span data-ttu-id="97091-160">Возможные значения: `mobile`, `alternateMobile` или `office`.</span><span class="sxs-lookup"><span data-stu-id="97091-160">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|
|<span data-ttu-id="97091-161">smsSignInState</span><span class="sxs-lookup"><span data-stu-id="97091-161">smsSignInState</span></span>|<span data-ttu-id="97091-162">string</span><span class="sxs-lookup"><span data-stu-id="97091-162">string</span></span>|<span data-ttu-id="97091-163">Готов ли телефон к входу в SMS или нет.</span><span class="sxs-lookup"><span data-stu-id="97091-163">Whether a phone is ready to be used for SMS sign-in or not.</span></span> <span data-ttu-id="97091-164">Возможные значения: `notSupported` `notAllowedByPolicy` , , , , , `notEnabled` `phoneNumberNotUnique` или `ready` `notConfigured` .</span><span class="sxs-lookup"><span data-stu-id="97091-164">Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, or `notConfigured`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97091-165">Связи</span><span class="sxs-lookup"><span data-stu-id="97091-165">Relationships</span></span>

<span data-ttu-id="97091-166">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97091-166">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="97091-167">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="97091-167">JSON representation</span></span>

<span data-ttu-id="97091-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="97091-168">The following is a JSON representation of the resource.</span></span>

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


