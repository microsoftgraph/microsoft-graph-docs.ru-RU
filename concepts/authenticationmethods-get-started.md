---
title: Начало работы с API способов проверки подлинности в Microsoft Graph
description: AP способов проверки подлинности в Microsoft Graph с помощью программных средств позволяет организациям управлять способами проверки подлинности пользователей, регистрировать пользователей для выполнения многофакторной проверки подлинности (MFA) и выполнять самостоятельный сброс пароля (SSPR).
author: mmcla
localization_priority: Priority
ms.prod: identity-and-sign-in
ms.openlocfilehash: 36385345141daa8dc782b64fa154ef97c46b3091
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761453"
---
# <a name="get-started-with-the-microsoft-graph-authentication-methods-api"></a><span data-ttu-id="4f6c6-103">Начало работы с API способов проверки подлинности в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4f6c6-103">Get started with the Microsoft Graph authentication methods API</span></span>

<span data-ttu-id="4f6c6-104">[Способы проверки подлинности](/azure/active-directory/authentication/concept-authentication-methods) — это способы, с помощью которых происходит проверка подлинности пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="4f6c6-104">[Authentication methods](/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="4f6c6-105">Способы проверки подлинности в Azure AD включают пароль и телефон (например, SMS и голосовые вызовы), которыми можно управлять в Microsoft Graph уже сегодня, и множество других, таких как ключи безопасности FIDO2 и приложение Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-105">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="4f6c6-106">Способы проверки подлинности используются в ходе основной, двухфакторной проверки подлинности, проверки подлинности повышенного уровня, а также в процессе самостоятельного сброса пароля (SSPR).</span><span class="sxs-lookup"><span data-stu-id="4f6c6-106">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="4f6c6-107">Вы можете использовать API способа проверки подлинности для управления способами проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-107">You can use the authentication method APIs to manage a user's authentication methods.</span></span> <span data-ttu-id="4f6c6-108">Например, вы можете:</span><span class="sxs-lookup"><span data-stu-id="4f6c6-108">For example, you can:</span></span>

* <span data-ttu-id="4f6c6-109">добавить номер телефона пользователя, который затем он может использовать для проверки подлинности с помощью SMS и голосового вызова, если применение такого способа разрешено политикой;</span><span class="sxs-lookup"><span data-stu-id="4f6c6-109">Add a phone number for a user, who can then use that number for SMS and voice call authentication if they're enabled to use it by policy</span></span>
* <span data-ttu-id="4f6c6-110">обновить или удалить номер телефона, назначенный пользователю;</span><span class="sxs-lookup"><span data-stu-id="4f6c6-110">Update or delete the phone number assigned to a user</span></span>
* <span data-ttu-id="4f6c6-111">включить или отключить номер для входа с помощью SMS;</span><span class="sxs-lookup"><span data-stu-id="4f6c6-111">Enable or disable the number for SMS sign-in</span></span>
* <span data-ttu-id="4f6c6-112">сбросить пароль пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-112">Reset a user's password</span></span>

<span data-ttu-id="4f6c6-113">API — это основной инструмент для управления способами проверки подлинности пользователей.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-113">The APIs are a key tool to manage your users' authentication methods.</span></span>

<span data-ttu-id="4f6c6-114">С помощью данного руководства вы научитесь:</span><span class="sxs-lookup"><span data-stu-id="4f6c6-114">In this tutorial, you'll learn how to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="4f6c6-115">выполнять проверку подлинности в Azure AD с правильными ролями и разрешениями;</span><span class="sxs-lookup"><span data-stu-id="4f6c6-115">Authenticate to Azure AD with the right roles and permissions</span></span>
> * <span data-ttu-id="4f6c6-116">проверять способы проверки подлинности пользователя;</span><span class="sxs-lookup"><span data-stu-id="4f6c6-116">Check the user's authentication methods</span></span>
> * <span data-ttu-id="4f6c6-117">добавлять новые номера телефонов пользователю;</span><span class="sxs-lookup"><span data-stu-id="4f6c6-117">Add new phone numbers for the user</span></span>
> * <span data-ttu-id="4f6c6-118">удалять номера телефона у пользователя;</span><span class="sxs-lookup"><span data-stu-id="4f6c6-118">Remove a phone number from the user</span></span>
> * <span data-ttu-id="4f6c6-119">сбрасывать пароль пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-119">Reset the user's password</span></span>

## <a name="step-1-authenticate-to-azure-ad-with-the-right-roles-and-permissions"></a><span data-ttu-id="4f6c6-120">Этап 1: проверка подлинности в Azure AD с правильными ролями и разрешениями</span><span class="sxs-lookup"><span data-stu-id="4f6c6-120">Step 1: Authenticate to Azure AD with the right roles and permissions</span></span>

<span data-ttu-id="4f6c6-121">С помощью любимого[инструмента взаимодействия с Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph) выполните вход, используя учетную запись с одной из этих ролей:</span><span class="sxs-lookup"><span data-stu-id="4f6c6-121">Using your favorite [tool for interacting with Microsoft Graph](use-the-api.md#tools-for-interacting-with-microsoft-graph), sign in using an account with one of these roles:</span></span>

* <span data-ttu-id="4f6c6-122">глобальный администратор;</span><span class="sxs-lookup"><span data-stu-id="4f6c6-122">Global administrator</span></span>
* <span data-ttu-id="4f6c6-123">привилегированный администратор проверки подлинности;</span><span class="sxs-lookup"><span data-stu-id="4f6c6-123">Privileged authentication administrator</span></span>
* <span data-ttu-id="4f6c6-124">администратор проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-124">Authentication administrator</span></span>

<span data-ttu-id="4f6c6-125">Теперь можно изменить разрешения.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-125">Next, modify your permissions.</span></span> <span data-ttu-id="4f6c6-126">В этом руководстве мы будем использовать метод [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview), поэтому убедитесь, что он включен в песочнице Graph или в приложении.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-126">We'll use [UserAuthenticationMethod.ReadWrite.All](permissions-reference.md#user-authentication-method-permissions-preview) for this tutorial, so make sure it's enabled in Graph Explorer or your app.</span></span>

<span data-ttu-id="4f6c6-127">После назначения и предоставления области можно приступить к работе с API.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-127">Once the scope is assigned and consented, you can start using the API.</span></span> <span data-ttu-id="4f6c6-128">Здесь в примерах используется стандартный пользователь с именем Андрей Говоров.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-128">The examples here use a standard user named Avery Howard.</span></span> <span data-ttu-id="4f6c6-129">Необходимо использовать уже имеющуюся тестовую учетную запись или создать новую, соблюдая [эти инструкции](/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span><span class="sxs-lookup"><span data-stu-id="4f6c6-129">You should use a preexisting test account or create a new one following [these instructions](/azure/active-directory/fundamentals/add-users-azure-active-directory#add-a-new-user).</span></span> <span data-ttu-id="4f6c6-130">Это интерактивные API, поэтому не проверяйте их на реальных пользователях.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-130">These APIs are live so don't test them on real users.</span></span>

## <a name="step-2-check-the-users-authentication-methods"></a><span data-ttu-id="4f6c6-131">Этап 2: проверка способов проверки подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="4f6c6-131">Step 2: Check the user's authentication methods</span></span>

<span data-ttu-id="4f6c6-132">Сделайте вызов для отображения способов проверки подлинности пользователя</span><span class="sxs-lookup"><span data-stu-id="4f6c6-132">Make a call to see the user's authentication methods.</span></span> <span data-ttu-id="4f6c6-133">Введите URL-адрес, чтобы просмотреть профиль пользователя, и добавьте `/authentication/methods`:</span><span class="sxs-lookup"><span data-stu-id="4f6c6-133">Take the URL to see a user's profile and add `/authentication/methods`:</span></span>

### <a name="request"></a><span data-ttu-id="4f6c6-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6c6-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="4f6c6-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6c6-135">Response</span></span>

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

## <a name="step-3-add-new-phone-numbers-for-the-user"></a><span data-ttu-id="4f6c6-136">Этап 3: добавление новых номеров телефонов пользователю</span><span class="sxs-lookup"><span data-stu-id="4f6c6-136">Step 3: Add new phone numbers for the user</span></span>

<span data-ttu-id="4f6c6-137">На предыдущем этапе новый пользователь (Андрей) зарегистрировал только пароль.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-137">From the previous step, a new user (Avery) only has a password registered.</span></span> <span data-ttu-id="4f6c6-138">Чтобы назначить новый номер телефона, который будет использовать Андрей, выполните запрос `POST` с типом телефона и номером в теле.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-138">To assign a new phone number for Avery to use, make a `POST` request with the phone type and number in the body.</span></span> <span data-ttu-id="4f6c6-139">Чтобы сообщить системе о том, что номер телефона добавлен, вам также потребуется изменить окончание URL-адреса с `methods` на `phoneMethods`.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-139">To tell the system that a phone number is being added, you'll also need to change the end of the URL from `methods` to `phoneMethods`.</span></span>

### <a name="request"></a><span data-ttu-id="4f6c6-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6c6-140">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="4f6c6-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6c6-141">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "3179e48a-750b-4051-897c-87b9720928f7",
    "phoneNumber": "+1 2065550123",
    "phoneType": "mobile",
    "smsSignInState": "ready"
}
```

<span data-ttu-id="4f6c6-142">Чтобы добавить рабочий номер телефона Андрея, вам потребуется выполнить запрос `POST` повторно на этот же URL-адрес, но обновить тип и номер телефона.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-142">To add Avery's office number, you'll `POST` again to the same URL but update the phone type and number:</span></span>

### <a name="request"></a><span data-ttu-id="4f6c6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6c6-143">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="4f6c6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6c6-144">Response</span></span>

```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('avery.howard%40wingtiptoysonline.com')/authentication/phoneMethods/$entity",
    "id": "e37fc753-ff3b-4958-9484-eaa9425c82bc",
    "phoneNumber": "+1 4255550199",
    "phoneType": "office",
    "smsSignInState": "notSupported"
}
```

<span data-ttu-id="4f6c6-145">Выполните еще один запрос `GET` на URL-адрес способов проверки с помощью телефона для отображения всех номеров телефона Андрея:</span><span class="sxs-lookup"><span data-stu-id="4f6c6-145">Do one more `GET` to the phone methods URL to see all of Avery's phone numbers:</span></span>

### <a name="request"></a><span data-ttu-id="4f6c6-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6c6-146">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods
```

### <a name="response"></a><span data-ttu-id="4f6c6-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6c6-147">Response</span></span>

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

<span data-ttu-id="4f6c6-148">Убедитесь, что вы видите оба номера, как и предполагалось.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-148">Confirm that you can see both numbers as expected.</span></span>

## <a name="step-4-remove-a-phone-number-from-the-user"></a><span data-ttu-id="4f6c6-149">Этап 4: удаление номера телефона у пользователя</span><span class="sxs-lookup"><span data-stu-id="4f6c6-149">Step 4: Remove a phone number from the user</span></span>

<span data-ttu-id="4f6c6-150">В этом случае Андрей теперь работает из дома, поэтому вам нужно удалить рабочий номер из его учетной записи.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-150">In this scenario, Avery is now working from home you need to remove their office number from their account.</span></span> <span data-ttu-id="4f6c6-151">Необходимо выполнить запрос `DELETE` на URL-адрес рабочего телефона, который можно создать, добавив идентификатор рабочего номера в URL-адрес способов проверки по телефону.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-151">You need to call `DELETE` on the office phone URL, which you can create by appending the office phone's ID to the phone methods URL.</span></span> <span data-ttu-id="4f6c6-152">Просмотрите список номеров телефона Андрея: идентификатор рабочего номера телефона начинается с "e37f".</span><span class="sxs-lookup"><span data-stu-id="4f6c6-152">Look at Avery's list of phones above: the office phone ID starts with "e37f".</span></span>

### <a name="request"></a><span data-ttu-id="4f6c6-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6c6-153">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/phoneMethods/e37fc753-ff3b-4958-9484-eaa9425c82bc
```

<span data-ttu-id="4f6c6-154">В отклике нет данных, так как в нем больше нет рабочего номера.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-154">There's no data in the response because there's no more office phone as intended.</span></span> <span data-ttu-id="4f6c6-155">Чтобы убедиться в том, что номер был удален, просмотрите все способы для Андрея. Процедура `GET` аналогична той, которая была сделана ранее.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-155">You can confirm it's gone by looking at all of Avery's methods, which is the same `GET` that was made previously:</span></span>

### <a name="request"></a><span data-ttu-id="4f6c6-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6c6-156">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/methods
```

### <a name="response"></a><span data-ttu-id="4f6c6-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6c6-157">Response</span></span>

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

<span data-ttu-id="4f6c6-158">Как и предполагалось, пользователь снова сможет использовать только один номер мобильного телефона и пароль.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-158">As expected, the user is now back to only having one mobile phone and a password.</span></span>

## <a name="step-5-reset-the-users-password"></a><span data-ttu-id="4f6c6-159">Этап 5: сброс пароля пользователя</span><span class="sxs-lookup"><span data-stu-id="4f6c6-159">Step 5: Reset the user's password</span></span>

<span data-ttu-id="4f6c6-160">В этом сценарии Андрей забыл свой пароль и вам необходимо выполнить сброс его пароля.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-160">In this scenario, Avery has forgotten their password and you need to reset it for them.</span></span> <span data-ttu-id="4f6c6-161">Для сброса необходимо выполнить запрос `POST` на URL-адрес пароля (см. идентификатор, начинающийся с "28c1" выше в списке способов проверки подлинности Андрей), указав действие "resetPassword".</span><span class="sxs-lookup"><span data-stu-id="4f6c6-161">To reset, you'll make a `POST` to their password's URL (see the ID starting with "28c1" above in Avery's list of authentication methods), specifying the "resetPassword" action.</span></span> <span data-ttu-id="4f6c6-162">В теле запроса укажите новый пароль.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-162">Provide the new password in the request body.</span></span>

### <a name="request"></a><span data-ttu-id="4f6c6-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6c6-163">Request</span></span>

```http
POST https://graph.microsoft.com/beta/users/avery.howard@wingtiptoysonline.com/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-Type: application/json
```

```json
{
    "newPassword": "29sdjfw#fajsdA_a_3an3223"
}
```

### <a name="response"></a><span data-ttu-id="4f6c6-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6c6-164">Response</span></span>

``` http
Location: https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

<span data-ttu-id="4f6c6-165">Поскольку происходит синхронизация пароля с Active Directory в локальной инфраструктуре клиента, то этот процесс может занять несколько минут, поэтому у вас есть адрес, по которому можно проверить завершение процесса синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-165">Because this is syncing the password down to Active Directory in the tenant's on-prem infrastructure, it might take a few minutes, so you have an address where you can check to see if it's complete.</span></span> <span data-ttu-id="4f6c6-166">Этот адрес находится в заголовке расположения отклика, а для просмотра статуса выполните запрос `GET` по этому URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-166">This address is in the location header of the response, and to see the status do a `GET` on that URL.</span></span>

### <a name="request"></a><span data-ttu-id="4f6c6-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f6c6-167">Request</span></span>

```http
GET https://graph.microsoft.com/beta/users/ed178e23-7447-4892-baf8-fc46f8af26ce/authentication/operations/74bfa1a6-c0e0-4957-8c37-f91048f4959e?aadgdc=BY01P&aadgsu=ssprprod-a
```

### <a name="response"></a><span data-ttu-id="4f6c6-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f6c6-168">Response</span></span>

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

<span data-ttu-id="4f6c6-169">Выполнено!</span><span class="sxs-lookup"><span data-stu-id="4f6c6-169">And success!</span></span> <span data-ttu-id="4f6c6-170">Вы ознакомились с информацией о просмотре профиля пользователя, методах проверки подлинности, добавлении и удалении номеров телефонов, а также о сбросе пароля.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-170">You've walked through seeing a user's profile, their auth methods, adding and removing phone numbers, and resetting their password.</span></span> <span data-ttu-id="4f6c6-171">Теперь вы можете приступать к управлению способами для своих пользователей.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-171">Now you're ready to go manage your own users' methods.</span></span>

## <a name="api-reference"></a><span data-ttu-id="4f6c6-172">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="4f6c6-172">API reference</span></span>

<span data-ttu-id="4f6c6-173">Ищете справочные материалы по API для способов проверки подлинности?</span><span class="sxs-lookup"><span data-stu-id="4f6c6-173">Looking for the API reference for authentication methods?</span></span>

* <span data-ttu-id="4f6c6-174">См. статью [Обзор API способов проверки подлинности для Azure AD](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span><span class="sxs-lookup"><span data-stu-id="4f6c6-174">See [Azure AD authentication methods API overview](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta)</span></span>

## <a name="next-steps"></a><span data-ttu-id="4f6c6-175">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="4f6c6-175">Next steps</span></span>

* <span data-ttu-id="4f6c6-176">Узнайте, как [использовать API REST для способов проверки подлинности](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="4f6c6-176">Find out how to [use the authentication method REST APIs](/graph/api/resources/authenticationmethods-overview?view=graph-rest-beta).</span></span>
* <span data-ttu-id="4f6c6-177">Используйте Azure AD для [аутентификации](./auth/index.yml) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-177">Use Azure AD to [authenticate](./auth/index.yml) to Microsoft Graph.</span></span>
* <span data-ttu-id="4f6c6-178">Интегрируйте [вход в Azure AD](https://azure.microsoft.com/develop/identity/signin/) в свое приложение или в свой веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-178">Integrate [Azure AD sign-in](https://azure.microsoft.com/develop/identity/signin/) into your app or website.</span></span>
* <span data-ttu-id="4f6c6-179">Сведения о новых возможностях API Azure AD см. в [журнале изменений](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="4f6c6-179">See the [Changelog](changelog.md) for information about what's new in the Azure AD APIs.</span></span>
* <span data-ttu-id="4f6c6-180">Изучите [примеры](https://developer.microsoft.com/graph/graph/examples), чтобы получить более четкое представление об использовании Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4f6c6-180">Explore [examples](https://developer.microsoft.com/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>