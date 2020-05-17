---
title: Начало работы с API методов проверки подлинности Microsoft Graph
description: API методов проверки подлинности в Microsoft Graph дает организациям возможность программно управлять методами проверки подлинности пользователей, получая пользователей, зарегистрированных для многофакторной проверки подлинности (MFA) и самостоятельного сброса пароля (SSPR).
author: mmcla
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8f08ae59f7a2ad0e16c4fc0c3af5637bcbfaaca
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272813"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a><span data-ttu-id="b5ce0-103">Начало работы с API методов проверки подлинности Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b5ce0-103">Get started with the Microsoft Graph authentication methods API</span></span>

<span data-ttu-id="b5ce0-104">[Методы проверки подлинности](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) — это способы проверки подлинности пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b5ce0-104">[Authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="b5ce0-105">Методы проверки подлинности в Azure AD включают пароль и телефон (например, SMS и голосовые вызовы), которые могут управляться сегодня в Microsoft Graph, среди многих других, таких как ключи безопасности FIDO2 и приложение Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-105">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="b5ce0-106">Методы проверки подлинности используются в основной, второй фактор и пошаговой проверке подлинности, а также в процессе самообслуживания пароля (SSPR).</span><span class="sxs-lookup"><span data-stu-id="b5ce0-106">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="b5ce0-107">Для управления методами проверки подлинности пользователя можно использовать API метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-107">You can use the authentication method APIs to manage a user's authentication methods.</span></span> <span data-ttu-id="b5ce0-108">Например, вы можете:</span><span class="sxs-lookup"><span data-stu-id="b5ce0-108">For example, you can:</span></span>

* <span data-ttu-id="b5ce0-109">Добавление номера телефона для пользователя, который может использовать этот номер для проверки подлинности SMS и голосовых вызовов, если они включены для использования политикой</span><span class="sxs-lookup"><span data-stu-id="b5ce0-109">Add a phone number for a user, who can then use that number for SMS and voice call authentication if they're enabled to use it by policy</span></span>
* <span data-ttu-id="b5ce0-110">Обновление или удаление номера телефона, назначенного пользователю</span><span class="sxs-lookup"><span data-stu-id="b5ce0-110">Update or delete the phone number assigned to a user</span></span>
* <span data-ttu-id="b5ce0-111">Включение и выключение номера для входа в SMS</span><span class="sxs-lookup"><span data-stu-id="b5ce0-111">Enable or disable the number for SMS sign-in</span></span>
* <span data-ttu-id="b5ce0-112">Сброс пароля пользователя</span><span class="sxs-lookup"><span data-stu-id="b5ce0-112">Reset a user's password</span></span>

<span data-ttu-id="b5ce0-113">API — это ключевой инструмент для управления методами проверки подлинности пользователей.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-113">The APIs are a key tool to manage your users' authentication methods.</span></span>

<span data-ttu-id="b5ce0-114">В этом руководстве вы узнаете, как:</span><span class="sxs-lookup"><span data-stu-id="b5ce0-114">In this tutorial, you'll learn how to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="b5ce0-115">Проверка подлинности в Azure AD с правильными ролями и разрешениями</span><span class="sxs-lookup"><span data-stu-id="b5ce0-115">Authenticate to Azure AD with the right roles and permissions</span></span>
> * <span data-ttu-id="b5ce0-116">Проверка методов проверки подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="b5ce0-116">Check the user's authentication methods</span></span>
> * <span data-ttu-id="b5ce0-117">Добавление новых номеров телефонов для пользователя</span><span class="sxs-lookup"><span data-stu-id="b5ce0-117">Add new phone numbers for the user</span></span>
> * <span data-ttu-id="b5ce0-118">Удаление номера телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="b5ce0-118">Remove a phone number from the user</span></span>
> * <span data-ttu-id="b5ce0-119">Сброс пароля пользователя</span><span class="sxs-lookup"><span data-stu-id="b5ce0-119">Reset the user's password</span></span>

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a><span data-ttu-id="b5ce0-120">Шаг 1: проверка подлинности в Azure AD с правильными ролями и разрешениями</span><span class="sxs-lookup"><span data-stu-id="b5ce0-120">Step 1: Authenticate to Azure AD with the right roles and permissions</span></span>

<span data-ttu-id="b5ce0-121">С помощью избранного [средства для взаимодействия с Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph)выполните вход с помощью учетной записи с одной из этих ролей:</span><span class="sxs-lookup"><span data-stu-id="b5ce0-121">Using your favorite [tool for interacting with Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), sign in using an account with one of these roles:</span></span>

* <span data-ttu-id="b5ce0-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b5ce0-122">Global administrator</span></span>
* <span data-ttu-id="b5ce0-123">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b5ce0-123">Privileged authentication administrator</span></span>
* <span data-ttu-id="b5ce0-124">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b5ce0-124">Authentication administrator</span></span>

<span data-ttu-id="b5ce0-125">Затем измените свои разрешения.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-125">Next, modify your permissions.</span></span> <span data-ttu-id="b5ce0-126">Мы будем использовать [усераусентикатионмесод. ReadWrite. ALL](permissions-reference.md#user-authentication-method-permissions-preview) для этого руководства, поэтому убедитесь, что он включен в проводнике Graph или приложении.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-126">We'll use [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview) for this tutorial, so make sure it's enabled in Graph Explorer or your app.</span></span>

<span data-ttu-id="b5ce0-127">Когда область будет назначена и отправлена, вы можете начать использовать API.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-127">Once the scope is assigned and consented, you can start using the API.</span></span> <span data-ttu-id="b5ce0-128">В приведенных ниже примерах используется стандартный пользователь с именем Avery Говард.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-128">The examples here use a standard user named Avery Howard.</span></span> <span data-ttu-id="b5ce0-129">Следует использовать уже существующую тестовую учетную запись или создать новую с помощью приведенных ниже [инструкций](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span><span class="sxs-lookup"><span data-stu-id="b5ce0-129">You should use a preexisting test account or create a new one following [these instructions](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span></span> <span data-ttu-id="b5ce0-130">Эти API являются реальными, поэтому их не следует тестировать на реальных пользователях.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-130">These APIs are live so don't test them on real users.</span></span>

## <a name="step-2-check-the-users-authentication-methods"></a><span data-ttu-id="b5ce0-131">Шаг 2: проверка методов проверки подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="b5ce0-131">Step 2: Check the user's authentication methods</span></span>

<span data-ttu-id="b5ce0-132">Выполните вызов, чтобы увидеть методы проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-132">Make a call to see the user's authentication methods.</span></span> <span data-ttu-id="b5ce0-133">Сделайте URL-адрес, чтобы просмотреть профиль пользователя, и добавьте `/authentication/methods` :</span><span class="sxs-lookup"><span data-stu-id="b5ce0-133">Take the URL to see a user's profile and add `/authentication/methods`:</span></span>

### <a name="request"></a><span data-ttu-id="b5ce0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ce0-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="b5ce0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ce0-135">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

## <a name="step-3-add-new-phone-numbers-for-the-user"></a><span data-ttu-id="b5ce0-136">Шаг 3: Добавление новых номеров телефонов для пользователя</span><span class="sxs-lookup"><span data-stu-id="b5ce0-136">Step 3: Add new phone numbers for the user</span></span>

<span data-ttu-id="b5ce0-137">На предыдущем шаге для нового пользователя (Avery) записывается только пароль.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-137">From the previous step, a new user (Avery) only has a password registered.</span></span> <span data-ttu-id="b5ce0-138">Чтобы назначить новый номер телефона для использования с помощью параметра Avery, сделайте `POST` запрос с типом телефона и номером в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-138">To assign a new phone number for Avery to use, make a `POST` request with the phone type and number in the body.</span></span> <span data-ttu-id="b5ce0-139">Чтобы сообщить системе, что номер телефона добавлен, также необходимо изменить конец URL-адреса с `methods` на `phoneMethods` .</span><span class="sxs-lookup"><span data-stu-id="b5ce0-139">To tell the system that a phone number is being added, you'll also need to change the end of the URL from `methods` to `phoneMethods`.</span></span>

### <a name="request"></a><span data-ttu-id="b5ce0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ce0-140">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "mobile",
    "phoneNumber": "+1 2065550123"
}
```

### <a name="response"></a><span data-ttu-id="b5ce0-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ce0-141">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "3179e48a-750b-4051-897c-87b9720928f7",
    "phoneNumber": "+1 2065550123",
    "phoneType": "mobile",
    "smsSignInState": "ready"
}
```

<span data-ttu-id="b5ce0-142">Чтобы добавить номер Office для Office, `POST` повторите попытку с тем же URL-адресом, но измените тип и номер телефона:</span><span class="sxs-lookup"><span data-stu-id="b5ce0-142">To add Avery's office number, you'll `POST` again to the same URL but update the phone type and number:</span></span>

### <a name="request"></a><span data-ttu-id="b5ce0-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ce0-143">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
Content-Type: application/json
```

```json
{
    "phoneType": "office",
    "phoneNumber": "+1 4255550199"
}
```

### <a name="response"></a><span data-ttu-id="b5ce0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ce0-144">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
    "phoneNumber": "+1 4255550199",
    "phoneType": "office",
    "smsSignInState": "notSupported"
}
```

<span data-ttu-id="b5ce0-145">Сделайте еще один дополнительный `GET` URL-адрес методов телефона, чтобы просмотреть все номера телефонов Avery:</span><span class="sxs-lookup"><span data-stu-id="b5ce0-145">Do one more `GET` to the phone methods URL to see all of Avery's phone numbers:</span></span>

### <a name="request"></a><span data-ttu-id="b5ce0-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ce0-146">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
```

### <a name="response"></a><span data-ttu-id="b5ce0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ce0-147">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods",
    "value": [
        {
            "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
            "phoneNumber": "+1 4255550199",
            "phoneType": "office",
            "smsSignInState": "notSupported"
        },
        {
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        }
    ]
}
```

<span data-ttu-id="b5ce0-148">Убедитесь, что вы видите оба числа, как ожидалось.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-148">Confirm that you can see both numbers as expected.</span></span>

## <a name="step-4-remove-a-phone-number-from-the-user"></a><span data-ttu-id="b5ce0-149">Шаг 4: Удаление номера телефона пользователя</span><span class="sxs-lookup"><span data-stu-id="b5ce0-149">Step 4: Remove a phone number from the user</span></span>

<span data-ttu-id="b5ce0-150">В этом сценарии Avery теперь работает с домашней страницы, поэтому вам нужно удалить номер Office из своей учетной записи.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-150">In this scenario, Avery is now working from home you need to remove their office number from their account.</span></span> <span data-ttu-id="b5ce0-151">Вам нужно позвонить по `DELETE` URL-адресу Office Phone, который можно создать, добавив идентификатор Office Phone в URL-адрес методов телефона.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-151">You need to call `DELETE` on the office phone URL, which you can create by appending the office phone's ID to the phone methods URL.</span></span> <span data-ttu-id="b5ce0-152">Просмотрите список номеров телефонов, приведенный в разделе Avery: номер офиса начинается с "e37f".</span><span class="sxs-lookup"><span data-stu-id="b5ce0-152">Look at Avery's list of phones above: the office phone ID starts with "e37f".</span></span>

### <a name="request"></a><span data-ttu-id="b5ce0-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ce0-153">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

<span data-ttu-id="b5ce0-154">В ответе нет данных, так как для него больше не предусмотрено Office Phone.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-154">There's no data in the response because there's no more office phone as intended.</span></span> <span data-ttu-id="b5ce0-155">Вы можете убедиться, что он просматривает все методы Avery, которые были `GET` сделаны ранее:</span><span class="sxs-lookup"><span data-stu-id="b5ce0-155">You can confirm it's gone by looking at all of Avery's methods, which is the same `GET` that was made previously:</span></span>

### <a name="request"></a><span data-ttu-id="b5ce0-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ce0-156">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="b5ce0-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ce0-157">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/methods",
    "value": [
        {
            "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
            "id": "3179e48a-750b-4051-897c-87b9720928f7",
            "phoneNumber": "+1 2065550123",
            "phoneType": "mobile",
            "smsSignInState": "ready"
        },
        {
            "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
            "id": "28c10230-6103-485e-b985-444c60001490",
            "password": null,
            "creationDateTime": null
        }
    ]
}
```

<span data-ttu-id="b5ce0-158">Как и ожидалось, теперь у пользователя есть только один мобильный телефон и пароль.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-158">As expected, the user is now back to only having one mobile phone and a password.</span></span>

## <a name="step-5-reset-the-users-password"></a><span data-ttu-id="b5ce0-159">Шаг 5: Сброс пароля пользователя</span><span class="sxs-lookup"><span data-stu-id="b5ce0-159">Step 5: Reset the user's password</span></span>

<span data-ttu-id="b5ce0-160">В этом сценарии Avery забыл пароль и его необходимо сбросить.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-160">In this scenario, Avery has forgotten their password and you need to reset it for them.</span></span> <span data-ttu-id="b5ce0-161">Для сброса необходимо указать `POST` URL-адрес своего пароля (в списке методы проверки подлинности, начинающийся с "28c1"), с указанием действия "ресетпассворд".</span><span class="sxs-lookup"><span data-stu-id="b5ce0-161">To reset, you'll make a `POST` to their password's URL (see the ID starting with "28c1" above in Avery's list of authentication methods), specifying the "resetPassword" action.</span></span> <span data-ttu-id="b5ce0-162">Введите новый пароль в теле запроса.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-162">Provide the new password in the request body.</span></span>

### <a name="request"></a><span data-ttu-id="b5ce0-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ce0-163">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-Type: application/json
```

```json
{
    "newPassword": "29sdjfw#fajsdA_a_3an3223"
}
```

### <a name="response"></a><span data-ttu-id="b5ce0-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ce0-164">Response</span></span>

```
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

<span data-ttu-id="b5ce0-165">Так как это приведет к синхронизации пароля в Active Directory в локальной инфраструктуре клиента, может потребоваться несколько минут, поэтому у вас есть адрес, по которому можно проверить, завершена ли работа.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-165">Because this is syncing the password down to Active Directory in the tenant's on-prem infrastructure, it might take a few minutes, so you have an address where you can check to see if it's complete.</span></span> <span data-ttu-id="b5ce0-166">Этот адрес находится в заголовке местоположения ответа, и для просмотра состояния выполните `GET` по этому URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-166">This address is in the location header of the response, and to see the status do a `GET` on that URL.</span></span>

### <a name="request"></a><span data-ttu-id="b5ce0-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5ce0-167">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

### <a name="response"></a><span data-ttu-id="b5ce0-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5ce0-168">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('ed178e23-7447-4892-baf8-fc46f8af26ce')/authentication/operations/$entity",
    "id": "74bfa1a6-c0e0-4957-8c37-f91048f4959e",
    "createdDateTime": "2020-05-14T00:23:40Z",
    "lastActionDateTime": "2020-05-14T00:23:41Z",
    "status": "succeeded",
    "statusDetail": "ResetSuccess",
    "resourceLocation": "https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/methods/28c10230-6103-485e-b985-444c60001490"
}
```

<span data-ttu-id="b5ce0-169">И успешное выполнение!</span><span class="sxs-lookup"><span data-stu-id="b5ce0-169">And success!</span></span> <span data-ttu-id="b5ce0-170">Вы проверили Просмотр профиля пользователя, методов проверки подлинности, добавления и удаления номеров телефонов, а также сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-170">You've walked through seeing a user's profile, their auth methods, adding and removing phone numbers, and resetting their password.</span></span> <span data-ttu-id="b5ce0-171">Теперь вы готовы к управлению методами своих пользователей.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-171">Now you're ready to go manage your own users' methods.</span></span>

## <a name="api-reference"></a><span data-ttu-id="b5ce0-172">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="b5ce0-172">API reference</span></span>

<span data-ttu-id="b5ce0-173">Ищете справочные материалы по API для методов проверки подлинности?</span><span class="sxs-lookup"><span data-stu-id="b5ce0-173">Looking for the API reference for authentication methods?</span></span>

* <span data-ttu-id="b5ce0-174">[Общие сведения об API методов проверки подлинности Azure AD](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="b5ce0-174">See [Azure AD authentication methods API overview](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span></span>

## <a name="next-steps"></a><span data-ttu-id="b5ce0-175">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b5ce0-175">Next steps</span></span>

* <span data-ttu-id="b5ce0-176">Узнайте [, как использовать REST API метода проверки подлинности](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="b5ce0-176">Find out how to [use the authentication method REST APIs](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span></span>
* <span data-ttu-id="b5ce0-177">Используйте Azure AD для [аутентификации](/graph/auth) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-177">Use Azure AD to [authenticate](/graph/auth) to Microsoft Graph.</span></span>
* <span data-ttu-id="b5ce0-178">Интегрируйте [вход в Azure AD](https://azure.microsoft.com/develop/identity/signin/) в свое приложение или в свой веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-178">Integrate [Azure AD sign-in](https://azure.microsoft.com/develop/identity/signin/) into your app or website.</span></span>
* <span data-ttu-id="b5ce0-179">Сведения о новых возможностях API Azure AD см. в [журнале изменений](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="b5ce0-179">See the [Changelog](changelog.md) for information about what's new in the Azure AD APIs.</span></span>
* <span data-ttu-id="b5ce0-180">Изучите [примеры](https://developer.microsoft.com/graph/graph/examples), чтобы получить более четкое представление об использовании Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b5ce0-180">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
