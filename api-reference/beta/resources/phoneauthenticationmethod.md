---
title: Тип ресурса phoneAuthenticationMethod
description: Представление телефона, зарегистрированного для пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 397d55050cbe0e985075a83527efff45572afe0b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156688"
---
# <a name="phoneauthenticationmethod-resource-type"></a><span data-ttu-id="b0571-103">Тип ресурса phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b0571-103">phoneAuthenticationMethod resource type</span></span>

<span data-ttu-id="b0571-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0571-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0571-105">Представление телефона, зарегистрированного для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0571-105">A representation of a phone registered to a user.</span></span> <span data-ttu-id="b0571-106">Этот ресурс включает номер телефона, тип телефона и то, настроен ли для пользователя вход с помощью SMS.</span><span class="sxs-lookup"><span data-stu-id="b0571-106">This resource includes the phone number, the phone type, and whether the phone is configured for the user to sign in via SMS.</span></span>

<span data-ttu-id="b0571-107">Телефон имеет один из трех типов: мобильный, альтернативный мобильный телефон или офис.</span><span class="sxs-lookup"><span data-stu-id="b0571-107">A phone has one of three types: mobile, alternate mobile, or office.</span></span> <span data-ttu-id="b0571-108">Пользователь может зарегистрировать один номер для каждого типа и должен иметь мобильный телефон до того, как будет добавлен альтернативный мобильный телефон.</span><span class="sxs-lookup"><span data-stu-id="b0571-108">A user can have one number registered for each type, and must have a mobile phone before an alternate mobile phone is added.</span></span> <span data-ttu-id="b0571-109">При использовании телефона для многофакторной проверки подлинности (MFA) или самостоятельного сброса пароля (SSPR) мобильный телефон используется по умолчанию, а альтернативный мобильный телефон является резервным.</span><span class="sxs-lookup"><span data-stu-id="b0571-109">When using a phone for multi-factor authentication (MFA) or self-service password reset (SSPR), the mobile phone is the default and the alternate mobile phone is the backup.</span></span> 

<span data-ttu-id="b0571-110">Мобильные телефоны можно использовать как для SMS-вызовов, так и для голосовых вызовов в зависимости от параметров клиента.</span><span class="sxs-lookup"><span data-stu-id="b0571-110">Mobile phones can be used for both SMS and voice calls, depending on the tenant settings.</span></span>

<span data-ttu-id="b0571-111">Офисный телефон может принимать только голосовые вызовы, а не SMS-сообщения.</span><span class="sxs-lookup"><span data-stu-id="b0571-111">An office phone can only receive voice calls, not SMS messages.</span></span>

<span data-ttu-id="b0571-112">Свойство состояния для входов в систему с помощью SMS-сообщения предоставляет сведения о готовности номера телефона к входу через SMS.</span><span class="sxs-lookup"><span data-stu-id="b0571-112">The SMS sign-in state property gives information about whether or not a phone number is ready to sign in via SMS.</span></span> <span data-ttu-id="b0571-113">Ниже возможен вариант значений.</span><span class="sxs-lookup"><span data-stu-id="b0571-113">The following are the possible values.</span></span>

|<span data-ttu-id="b0571-114">Значение</span><span class="sxs-lookup"><span data-stu-id="b0571-114">Value</span></span>|<span data-ttu-id="b0571-115">Описание</span><span class="sxs-lookup"><span data-stu-id="b0571-115">Description</span></span>|
|--------|-----------|
|`notSupported`|<span data-ttu-id="b0571-116">Основной вход не поддерживается для этого метода проверки подлинности. Например, вход можно включить только на основном мобильном номере пользователя, а не на альтернативном номере.</span><span class="sxs-lookup"><span data-stu-id="b0571-116">Primary sign-in not supported on this authentication method - for example, sign-in can be enabled only on a user's primary mobile number, not the alternate number.</span></span>|
|`notAllowedByPolicy`|<span data-ttu-id="b0571-117">Политика не позволяет этому пользователю использовать этот метод в качестве основного входа.</span><span class="sxs-lookup"><span data-stu-id="b0571-117">This user isn't enabled by policy to use this method as a primary sign-in.</span></span>|
|`notConfigured`|<span data-ttu-id="b0571-118">Политика позволяет этому пользователю использовать этот метод в качестве основного входа, но для его настройки необходимо принять дополнительные меры.</span><span class="sxs-lookup"><span data-stu-id="b0571-118">This user is enabled by policy to use this method as primary sign-in but needs to take additional action to configure it.</span></span>|
|`phoneNumberNotUnique`|<span data-ttu-id="b0571-119">Этот пользователь попытался настроить номер телефона в качестве основного, но он не был уникальным и не может использоваться в качестве имени для регистрации.</span><span class="sxs-lookup"><span data-stu-id="b0571-119">This user attempted to set up a phone number as primary sign-in but the number was not unique and can't be used as a sign-in name.</span></span>|
|`ready`|<span data-ttu-id="b0571-120">Этот метод проверки подлинности готов к использованию при основном входе.</span><span class="sxs-lookup"><span data-stu-id="b0571-120">This authentication method is ready for use in primary sign-in.</span></span>|

## <a name="methods"></a><span data-ttu-id="b0571-121">Методы</span><span class="sxs-lookup"><span data-stu-id="b0571-121">Methods</span></span>

| <span data-ttu-id="b0571-122">Метод</span><span class="sxs-lookup"><span data-stu-id="b0571-122">Method</span></span>       | <span data-ttu-id="b0571-123">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b0571-123">Return Type</span></span> | <span data-ttu-id="b0571-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b0571-124">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b0571-125">Список</span><span class="sxs-lookup"><span data-stu-id="b0571-125">List</span></span>](../api/Authentication-list-phonemethods.md) | [<span data-ttu-id="b0571-126">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b0571-126">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="b0571-127">Чтение свойств и связей всех объектов phoneAuthenticationMethod этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0571-127">Read properties and relationships of all of this user's phoneAuthenticationMethod objects.</span></span> |
| [<span data-ttu-id="b0571-128">Получение</span><span class="sxs-lookup"><span data-stu-id="b0571-128">Get</span></span>](../api/phoneauthenticationmethod-get.md) | [<span data-ttu-id="b0571-129">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b0571-129">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="b0571-130">Чтение свойств и связей объекта phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="b0571-130">Read properties and relationships of phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="b0571-131">Обновление</span><span class="sxs-lookup"><span data-stu-id="b0571-131">Update</span></span>](../api/phoneauthenticationmethod-update.md) | [<span data-ttu-id="b0571-132">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b0571-132">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="b0571-133">Обновление объекта phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="b0571-133">Update phoneAuthenticationMethod object.</span></span> |
| <span data-ttu-id="b0571-134">[удаление](../api/phoneauthenticationmethod-delete.md);</span><span class="sxs-lookup"><span data-stu-id="b0571-134">[Delete](../api/phoneauthenticationmethod-delete.md)</span></span> | <span data-ttu-id="b0571-135">Нет</span><span class="sxs-lookup"><span data-stu-id="b0571-135">None</span></span> | <span data-ttu-id="b0571-136">Удаление объекта phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="b0571-136">Delete phoneAuthenticationMethod object.</span></span> |
|[<span data-ttu-id="b0571-137">Отключение sms-подписи</span><span class="sxs-lookup"><span data-stu-id="b0571-137">Disable SMS signin</span></span>](../api/phoneauthenticationmethod-disablesmssignin.md)|<span data-ttu-id="b0571-138">Нет</span><span class="sxs-lookup"><span data-stu-id="b0571-138">None</span></span>|<span data-ttu-id="b0571-139">Отключите вход с помощью SMS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0571-139">Turn off SMS sign-in for a user.</span></span>|
|[<span data-ttu-id="b0571-140">Включить вход с помощью SMS</span><span class="sxs-lookup"><span data-stu-id="b0571-140">Enable SMS signin</span></span>](../api/phoneauthenticationmethod-enablesmssignin.md)|<span data-ttu-id="b0571-141">Нет</span><span class="sxs-lookup"><span data-stu-id="b0571-141">None</span></span>|<span data-ttu-id="b0571-142">Включит вход с помощью SMS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0571-142">Turn on SMS sign-in for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0571-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0571-143">Properties</span></span>

| <span data-ttu-id="b0571-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0571-144">Property</span></span>     | <span data-ttu-id="b0571-145">Тип</span><span class="sxs-lookup"><span data-stu-id="b0571-145">Type</span></span>        | <span data-ttu-id="b0571-146">Описание</span><span class="sxs-lookup"><span data-stu-id="b0571-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0571-147">id</span><span class="sxs-lookup"><span data-stu-id="b0571-147">id</span></span>|<span data-ttu-id="b0571-148">String</span><span class="sxs-lookup"><span data-stu-id="b0571-148">String</span></span>| <span data-ttu-id="b0571-149">Идентификатор этого телефона, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b0571-149">The identifier of this phone registered to this user.</span></span> <span data-ttu-id="b0571-150">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0571-150">Read-only.</span></span>|
|<span data-ttu-id="b0571-151">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b0571-151">phoneNumber</span></span>|<span data-ttu-id="b0571-152">String</span><span class="sxs-lookup"><span data-stu-id="b0571-152">String</span></span>|<span data-ttu-id="b0571-153">Номер телефона для текста или вызов для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b0571-153">The phone number to text or call for authentication.</span></span> <span data-ttu-id="b0571-154">Номера телефонов используют формат "+ \<country code\> \<number\> \<extension\> x", с необязательным расширением.</span><span class="sxs-lookup"><span data-stu-id="b0571-154">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="b0571-155">Например, допустимы +1 5555551234 или +1 5555551234x123.</span><span class="sxs-lookup"><span data-stu-id="b0571-155">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="b0571-156">Числа отклоняется при создании или обновлении, если они не соответствуют требуемму формату.</span><span class="sxs-lookup"><span data-stu-id="b0571-156">Numbers are rejected when creating/updating if they do not match the required format.</span></span> |
|<span data-ttu-id="b0571-157">phoneType</span><span class="sxs-lookup"><span data-stu-id="b0571-157">phoneType</span></span>|<span data-ttu-id="b0571-158">string</span><span class="sxs-lookup"><span data-stu-id="b0571-158">string</span></span>|<span data-ttu-id="b0571-159">Тип этого телефона.</span><span class="sxs-lookup"><span data-stu-id="b0571-159">The type of this phone.</span></span> <span data-ttu-id="b0571-160">Возможные значения: `mobile` , , или `alternateMobile` `office` .</span><span class="sxs-lookup"><span data-stu-id="b0571-160">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|
|<span data-ttu-id="b0571-161">smsSignInState</span><span class="sxs-lookup"><span data-stu-id="b0571-161">smsSignInState</span></span>|<span data-ttu-id="b0571-162">string</span><span class="sxs-lookup"><span data-stu-id="b0571-162">string</span></span>|<span data-ttu-id="b0571-163">Можно ли использовать телефон для sms-входов.</span><span class="sxs-lookup"><span data-stu-id="b0571-163">Whether a phone is ready to be used for SMS sign-in or not.</span></span> <span data-ttu-id="b0571-164">Возможные значения: `notSupported` , , , , , или `notAllowedByPolicy` `notEnabled` `phoneNumberNotUnique` `ready` `notConfigured` .</span><span class="sxs-lookup"><span data-stu-id="b0571-164">Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, or `notConfigured`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0571-165">Связи</span><span class="sxs-lookup"><span data-stu-id="b0571-165">Relationships</span></span>

<span data-ttu-id="b0571-166">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b0571-166">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0571-167">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b0571-167">JSON representation</span></span>

<span data-ttu-id="b0571-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0571-168">The following is a JSON representation of the resource.</span></span>

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


