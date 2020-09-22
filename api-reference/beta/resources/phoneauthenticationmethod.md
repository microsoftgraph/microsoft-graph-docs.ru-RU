---
title: Тип ресурса Фонеаусентикатионмесод
description: Представление телефона, зарегистрированное для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 93bf64756d0da1e4199fdede55990e695f434480
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997839"
---
# <a name="phoneauthenticationmethod-resource-type"></a><span data-ttu-id="b9be1-103">Тип ресурса Фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="b9be1-103">phoneAuthenticationMethod resource type</span></span>

<span data-ttu-id="b9be1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9be1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9be1-105">Представление телефона, зарегистрированное для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9be1-105">A representation of a phone registered to a user.</span></span> <span data-ttu-id="b9be1-106">Этот ресурс включает номер телефона, тип телефона, а также сведения о том, настроен ли телефон для входа пользователя с помощью SMS.</span><span class="sxs-lookup"><span data-stu-id="b9be1-106">This resource includes the phone number, the phone type, and whether the phone is configured for the user to sign in via SMS.</span></span>

<span data-ttu-id="b9be1-107">Телефон имеет один из трех типов: мобильный, альтернативный мобильный или Office.</span><span class="sxs-lookup"><span data-stu-id="b9be1-107">A phone has one of three types: mobile, alternate mobile, or office.</span></span> <span data-ttu-id="b9be1-108">Пользователь может иметь один номер, зарегистрированный для каждого типа, и для него должен быть установлен мобильный телефон, прежде чем будет добавлен другой мобильный телефон.</span><span class="sxs-lookup"><span data-stu-id="b9be1-108">A user can have one number registered for each type, and must have a mobile phone before an alternate mobile phone is added.</span></span> <span data-ttu-id="b9be1-109">При использовании телефона для многофакторной проверки подлинности (MFA) или самостоятельного сброса пароля (SSPR) мобильный телефон является значением по умолчанию, а альтернативным мобильным телефоном является резервная копия.</span><span class="sxs-lookup"><span data-stu-id="b9be1-109">When using a phone for multi-factor authentication (MFA) or self-service password reset (SSPR), the mobile phone is the default and the alternate mobile phone is the backup.</span></span> 

<span data-ttu-id="b9be1-110">Мобильные телефоны можно использовать как для SMS, так и для голосовых вызовов в зависимости от параметров клиента.</span><span class="sxs-lookup"><span data-stu-id="b9be1-110">Mobile phones can be used for both SMS and voice calls, depending on the tenant settings.</span></span>

<span data-ttu-id="b9be1-111">Телефон Office может принимать только голосовые вызовы, а не сообщения SMS.</span><span class="sxs-lookup"><span data-stu-id="b9be1-111">An office phone can only receive voice calls, not SMS messages.</span></span>

<span data-ttu-id="b9be1-112">Свойство состояния входа SMS-сообщений содержит сведения о том, готов ли телефонный номер к входу через SMS.</span><span class="sxs-lookup"><span data-stu-id="b9be1-112">The SMS sign-in state property gives information about whether or not a phone number is ready to sign in via SMS.</span></span> <span data-ttu-id="b9be1-113">Ниже приведены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="b9be1-113">The following are the possible values.</span></span>

|<span data-ttu-id="b9be1-114">Значение</span><span class="sxs-lookup"><span data-stu-id="b9be1-114">Value</span></span>|<span data-ttu-id="b9be1-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b9be1-115">Description</span></span>|
|--------|-----------|
|`notSupported`|<span data-ttu-id="b9be1-116">Основной вход не поддерживается в этом методе проверки подлинности — например, вход можно включить только для основного номера мобильного телефона пользователя, а не для дополнительного номера.</span><span class="sxs-lookup"><span data-stu-id="b9be1-116">Primary sign-in not supported on this authentication method - for example, sign-in can be enabled only on a user's primary mobile number, not the alternate number.</span></span>|
|`notAllowedByPolicy`|<span data-ttu-id="b9be1-117">Этот пользователь не включен политикой для использования этого метода в качестве основного входа.</span><span class="sxs-lookup"><span data-stu-id="b9be1-117">This user isn't enabled by policy to use this method as a primary sign-in.</span></span>|
|`notConfigured`|<span data-ttu-id="b9be1-118">Этот пользователь включен с помощью политики, чтобы использовать этот метод в качестве основного входа, но необходимо выполнить дополнительные действия по его настройке.</span><span class="sxs-lookup"><span data-stu-id="b9be1-118">This user is enabled by policy to use this method as primary sign-in but needs to take additional action to configure it.</span></span>|
|`phoneNumberNotUnique`|<span data-ttu-id="b9be1-119">Этот пользователь попытался настроить телефонный номер в качестве основного, но это значение не является уникальным и не может использоваться в качестве имени для входа.</span><span class="sxs-lookup"><span data-stu-id="b9be1-119">This user attempted to set up a phone number as primary sign-in but the number was not unique and can't be used as a sign-in name.</span></span>|
|`ready`|<span data-ttu-id="b9be1-120">Этот метод проверки подлинности готов к использованию в основном входе.</span><span class="sxs-lookup"><span data-stu-id="b9be1-120">This authentication method is ready for use in primary sign-in.</span></span>|

## <a name="methods"></a><span data-ttu-id="b9be1-121">Методы</span><span class="sxs-lookup"><span data-stu-id="b9be1-121">Methods</span></span>

| <span data-ttu-id="b9be1-122">Метод</span><span class="sxs-lookup"><span data-stu-id="b9be1-122">Method</span></span>       | <span data-ttu-id="b9be1-123">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b9be1-123">Return Type</span></span> | <span data-ttu-id="b9be1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b9be1-124">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b9be1-125">Список</span><span class="sxs-lookup"><span data-stu-id="b9be1-125">List</span></span>](../api/Authentication-list-phonemethods.md) | [<span data-ttu-id="b9be1-126">фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="b9be1-126">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="b9be1-127">Чтение свойств и связей всех объектов Фонеаусентикатионмесод этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9be1-127">Read properties and relationships of all of this user's phoneAuthenticationMethod objects.</span></span> |
| <span data-ttu-id="b9be1-128">[получение](../api/phoneauthenticationmethod-get.md);</span><span class="sxs-lookup"><span data-stu-id="b9be1-128">[Get](../api/phoneauthenticationmethod-get.md)</span></span> | [<span data-ttu-id="b9be1-129">фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="b9be1-129">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="b9be1-130">Чтение свойств и связей объекта Фонеаусентикатионмесод.</span><span class="sxs-lookup"><span data-stu-id="b9be1-130">Read properties and relationships of phoneAuthenticationMethod object.</span></span> |
| <span data-ttu-id="b9be1-131">[обновление](../api/phoneauthenticationmethod-update.md).</span><span class="sxs-lookup"><span data-stu-id="b9be1-131">[Update](../api/phoneauthenticationmethod-update.md)</span></span> | [<span data-ttu-id="b9be1-132">фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="b9be1-132">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="b9be1-133">Обновление объекта Фонеаусентикатионмесод.</span><span class="sxs-lookup"><span data-stu-id="b9be1-133">Update phoneAuthenticationMethod object.</span></span> |
| <span data-ttu-id="b9be1-134">[удаление](../api/phoneauthenticationmethod-delete.md);</span><span class="sxs-lookup"><span data-stu-id="b9be1-134">[Delete](../api/phoneauthenticationmethod-delete.md)</span></span> | <span data-ttu-id="b9be1-135">Нет</span><span class="sxs-lookup"><span data-stu-id="b9be1-135">None</span></span> | <span data-ttu-id="b9be1-136">Удаление объекта Фонеаусентикатионмесод.</span><span class="sxs-lookup"><span data-stu-id="b9be1-136">Delete phoneAuthenticationMethod object.</span></span> |
|[<span data-ttu-id="b9be1-137">Отключение входа в SMS</span><span class="sxs-lookup"><span data-stu-id="b9be1-137">Disable SMS signin</span></span>](../api/phoneauthenticationmethod-disablesmssignin.md)|<span data-ttu-id="b9be1-138">Нет</span><span class="sxs-lookup"><span data-stu-id="b9be1-138">None</span></span>|<span data-ttu-id="b9be1-139">Отключение входа в SMS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9be1-139">Turn off SMS sign-in for a user.</span></span>|
|[<span data-ttu-id="b9be1-140">Включение входа в SMS</span><span class="sxs-lookup"><span data-stu-id="b9be1-140">Enable SMS signin</span></span>](../api/phoneauthenticationmethod-enablesmssignin.md)|<span data-ttu-id="b9be1-141">Нет</span><span class="sxs-lookup"><span data-stu-id="b9be1-141">None</span></span>|<span data-ttu-id="b9be1-142">Включите вход в SMS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9be1-142">Turn on SMS sign-in for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="b9be1-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9be1-143">Properties</span></span>

| <span data-ttu-id="b9be1-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9be1-144">Property</span></span>     | <span data-ttu-id="b9be1-145">Тип</span><span class="sxs-lookup"><span data-stu-id="b9be1-145">Type</span></span>        | <span data-ttu-id="b9be1-146">Описание</span><span class="sxs-lookup"><span data-stu-id="b9be1-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9be1-147">id</span><span class="sxs-lookup"><span data-stu-id="b9be1-147">id</span></span>|<span data-ttu-id="b9be1-148">String</span><span class="sxs-lookup"><span data-stu-id="b9be1-148">String</span></span>| <span data-ttu-id="b9be1-149">Идентификатор телефона, зарегистрированный для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9be1-149">The identifier of this phone registered to this user.</span></span> <span data-ttu-id="b9be1-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b9be1-150">Read-only.</span></span>|
|<span data-ttu-id="b9be1-151">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b9be1-151">phoneNumber</span></span>|<span data-ttu-id="b9be1-152">String</span><span class="sxs-lookup"><span data-stu-id="b9be1-152">String</span></span>|<span data-ttu-id="b9be1-153">Номер телефона для текста или вызов для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b9be1-153">The phone number to text or call for authentication.</span></span> <span data-ttu-id="b9be1-154">Номера телефонов используют формат "+ \<country code\> \<number\> x \<extension\> " с необязательным расширением.</span><span class="sxs-lookup"><span data-stu-id="b9be1-154">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="b9be1-155">Например, допустимые + 1 5555551234 или + 1 5555551234x123.</span><span class="sxs-lookup"><span data-stu-id="b9be1-155">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="b9be1-156">При создании или обновлении числа отклоняются, если они не совпадают с требуемым форматом.</span><span class="sxs-lookup"><span data-stu-id="b9be1-156">Numbers are rejected when creating/updating if they do not match the required format.</span></span> |
|<span data-ttu-id="b9be1-157">фонетипе</span><span class="sxs-lookup"><span data-stu-id="b9be1-157">phoneType</span></span>|<span data-ttu-id="b9be1-158">string</span><span class="sxs-lookup"><span data-stu-id="b9be1-158">string</span></span>|<span data-ttu-id="b9be1-159">Тип телефона.</span><span class="sxs-lookup"><span data-stu-id="b9be1-159">The type of this phone.</span></span> <span data-ttu-id="b9be1-160">Возможные значения: `mobile` , `alternateMobile` , или `office` .</span><span class="sxs-lookup"><span data-stu-id="b9be1-160">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|
|<span data-ttu-id="b9be1-161">смссигнинстате</span><span class="sxs-lookup"><span data-stu-id="b9be1-161">smsSignInState</span></span>|<span data-ttu-id="b9be1-162">string</span><span class="sxs-lookup"><span data-stu-id="b9be1-162">string</span></span>|<span data-ttu-id="b9be1-163">Указывает, готов ли телефон к использованию для входа в SMS.</span><span class="sxs-lookup"><span data-stu-id="b9be1-163">Whether a phone is ready to be used for SMS sign-in or not.</span></span> <span data-ttu-id="b9be1-164">Возможные значения: `notSupported` , `notAllowedByPolicy` ,, `notEnabled` , `phoneNumberNotUnique` `ready` , или `notConfigured` .</span><span class="sxs-lookup"><span data-stu-id="b9be1-164">Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, or `notConfigured`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9be1-165">Связи</span><span class="sxs-lookup"><span data-stu-id="b9be1-165">Relationships</span></span>

<span data-ttu-id="b9be1-166">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9be1-166">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9be1-167">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b9be1-167">JSON representation</span></span>

<span data-ttu-id="b9be1-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9be1-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "baseType": "",
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


