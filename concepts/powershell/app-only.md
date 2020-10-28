---
title: Использование проверки подлинности только для приложений с помощью SDK Microsoft Graph PowerShell
description: Узнайте, как использовать проверку подлинности только для приложений, чтобы включить неинтерактивные сценарии с пакетом SDK PowerShell для Microsoft Graph.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 6cad5979e5bd7523174a792465d015dfe7d3d217
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782930"
---
# <a name="use-app-only-authentication-with-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="722bd-103">Использование проверки подлинности только для приложений с помощью SDK Microsoft Graph PowerShell</span><span class="sxs-lookup"><span data-stu-id="722bd-103">Use app-only authentication with the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="722bd-104">Пакет SDK для PowerShell поддерживает два типа проверки подлинности: [делегированный доступ](..\auth-v2-user.md)и [доступ только для приложений](..\auth-v2-service.md).</span><span class="sxs-lookup"><span data-stu-id="722bd-104">The PowerShell SDK supports two types of authentication: [delegated access](..\auth-v2-user.md), and [app-only access](..\auth-v2-service.md).</span></span> <span data-ttu-id="722bd-105">Это руководство посвящено настройке, необходимой для включения доступа только к приложениям.</span><span class="sxs-lookup"><span data-stu-id="722bd-105">This guide will focus on the configuration needed to enable app-only access.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="722bd-106">Доступ только к приложениям предоставляет разрешения непосредственно приложению и требует от администратора разрешения на требуемые области разрешений.</span><span class="sxs-lookup"><span data-stu-id="722bd-106">App-only access grants permissions directly to an application, and requires an administrator to consent to the required permission scopes.</span></span> <span data-ttu-id="722bd-107">Более подробную информацию о доступе к приложениям можно узнать в [статье платформа идентификации Майкрософт и процесс учетных данных клиента OAuth 2,0](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span><span class="sxs-lookup"><span data-stu-id="722bd-107">For more details on app-only access, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

<span data-ttu-id="722bd-108">Давайте разберем, как настроить доступ только к приложениям для простого скрипта, чтобы вывести список пользователей и групп в клиенте Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="722bd-108">Let's walk through configuring app-only access for a simple script to list users and groups in your Microsoft 365 tenant.</span></span>

## <a name="configuration"></a><span data-ttu-id="722bd-109">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="722bd-109">Configuration</span></span>

<span data-ttu-id="722bd-110">Прежде чем вы сможете использовать доступ только к приложениям с помощью пакета SDK, вам потребуется следующее.</span><span class="sxs-lookup"><span data-stu-id="722bd-110">Before you can use app-only access with the SDK, you need the following.</span></span>

- <span data-ttu-id="722bd-111">Сертификат, который будет использоваться в качестве учетных данных для приложения.</span><span class="sxs-lookup"><span data-stu-id="722bd-111">A certificate to use as a credential for the application.</span></span> <span data-ttu-id="722bd-112">Это может быть самозаверяющий сертификат или сертификат из центра сертификации.</span><span class="sxs-lookup"><span data-stu-id="722bd-112">This can be a self-signed certificate or a certificate from an authority.</span></span>
- <span data-ttu-id="722bd-113">Необходимо [зарегистрировать приложение](/azure/active-directory/develop/app-objects-and-service-principals) в Azure AD, настроить его с использованием областей разрешений, необходимых вашему сценарию, и предоставить общий доступ к открытому ключу для сертификата.</span><span class="sxs-lookup"><span data-stu-id="722bd-113">You must [register an application](/azure/active-directory/develop/app-objects-and-service-principals) in Azure AD, configure it with the permission scopes your scenario requires, and share the public key for your certificate.</span></span>

### <a name="certificate"></a><span data-ttu-id="722bd-114">Сертификат</span><span class="sxs-lookup"><span data-stu-id="722bd-114">Certificate</span></span>

<span data-ttu-id="722bd-115">Вам потребуется сертификат X. 509, установленный в доверенном хранилище пользователя на компьютере, на котором будет выполняться сценарий.</span><span class="sxs-lookup"><span data-stu-id="722bd-115">You will need an X.509 certificate installed in your user's trusted store on the machine where you will run the script.</span></span> <span data-ttu-id="722bd-116">Кроме того, вам потребуется открытый ключ сертификата, экспортированный в CER-, PEM-или CRT-формате.</span><span class="sxs-lookup"><span data-stu-id="722bd-116">You'll also need the certificate's public key exported in .cer, .pem, or .crt format.</span></span> <span data-ttu-id="722bd-117">Вам потребуется значение субъекта сертификата.</span><span class="sxs-lookup"><span data-stu-id="722bd-117">You'll need the value of the certificate subject.</span></span>

### <a name="register-the-application"></a><span data-ttu-id="722bd-118">Регистрация приложения</span><span class="sxs-lookup"><span data-stu-id="722bd-118">Register the application</span></span>

<span data-ttu-id="722bd-119">Вы можете зарегистрировать приложение либо на [портале Azure Active Directory](https://aad.portal.azure.com), либо с помощью PowerShell.</span><span class="sxs-lookup"><span data-stu-id="722bd-119">You can register the application either in the [Azure Active Directory portal](https://aad.portal.azure.com), or using PowerShell.</span></span>

# <a name="portal"></a>[<span data-ttu-id="722bd-120">Портал</span><span class="sxs-lookup"><span data-stu-id="722bd-120">Portal</span></span>](#tab/azure-portal)

1. <span data-ttu-id="722bd-121">Откройте браузер и перейдите в [центр администрирования Azure Active Directory](https://aad.portal.azure.com) и войдите в систему с помощью администратора организации клиента Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="722bd-121">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using an Microsoft 365 tenant organization admin.</span></span>

1. <span data-ttu-id="722bd-122">Выберите **Azure Active Directory** на панели навигации слева, затем выберите **Регистрация приложений** в разделе **Управление** .</span><span class="sxs-lookup"><span data-stu-id="722bd-122">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage** .</span></span>

    ![<span data-ttu-id="722bd-123">Снимок экрана с регистрациями приложений</span><span class="sxs-lookup"><span data-stu-id="722bd-123">A screenshot of the App registrations</span></span> ](./images/aad-portal-app-registrations.png)

1. <span data-ttu-id="722bd-124">Выберите **Новая регистрация** .</span><span class="sxs-lookup"><span data-stu-id="722bd-124">Select **New registration** .</span></span> <span data-ttu-id="722bd-125">На странице **Зарегистрировать приложение** задайте необходимые значения следующим образом.</span><span class="sxs-lookup"><span data-stu-id="722bd-125">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="722bd-126">Введите **имя** `Graph PowerShell Script`.</span><span class="sxs-lookup"><span data-stu-id="722bd-126">Set **Name** to `Graph PowerShell Script`.</span></span>
    - <span data-ttu-id="722bd-127">Установите **Поддерживаемые типы учетных** записей **только для учетных записей в данном организационном каталоге** .</span><span class="sxs-lookup"><span data-stu-id="722bd-127">Set **Supported account types** to **Accounts in this organizational directory only** .</span></span>
    - <span data-ttu-id="722bd-128">Оставьте пустым **URI перенаправления** .</span><span class="sxs-lookup"><span data-stu-id="722bd-128">Leave **Redirect URI** blank.</span></span>

    ![Снимок страницы "регистрация приложения"](./images/register-app.png)

1. <span data-ttu-id="722bd-130">Нажмите **Зарегистрировать** .</span><span class="sxs-lookup"><span data-stu-id="722bd-130">Select **Register** .</span></span> <span data-ttu-id="722bd-131">На странице **сценариев PowerShell Graph** СКОПИРУЙТЕ значения **идентификатора Application (Client)** и **идентификатора каталога (клиента)** и сохраните их.</span><span class="sxs-lookup"><span data-stu-id="722bd-131">On the **Graph PowerShell Script** page, copy the values of the **Application (client) ID** and **Directory (tenant) ID** and save them.</span></span>

    ![Снимок экрана с ИДЕНТИФИКАТОРом приложения для новой регистрации приложения](./images/aad-application-id.png)

1. <span data-ttu-id="722bd-133">Выберите **разрешения API** в разделе **Управление** .</span><span class="sxs-lookup"><span data-stu-id="722bd-133">Select **API Permissions** under **Manage** .</span></span> <span data-ttu-id="722bd-134">Нажмите кнопку **Добавить разрешение** .</span><span class="sxs-lookup"><span data-stu-id="722bd-134">Choose **Add a permission** .</span></span>

1. <span data-ttu-id="722bd-135">Выберите **Microsoft Graph** , а затем — **разрешения приложений** .</span><span class="sxs-lookup"><span data-stu-id="722bd-135">Select **Microsoft Graph** , then **Application Permissions** .</span></span> <span data-ttu-id="722bd-136">Добавьте **User. Read. ALL** и **Group. Read. ALL** , а затем выберите **Добавить разрешения** .</span><span class="sxs-lookup"><span data-stu-id="722bd-136">Add **User.Read.All** and **Group.Read.All** , then select **Add permissions** .</span></span>

1. <span data-ttu-id="722bd-137">В **настроенных разрешениях** удалите делегированного **пользователя.** разрешение на чтение **в Microsoft Graph** , выбрав элемент **...** справа от разрешения и выбрав пункт **удалить разрешение** .</span><span class="sxs-lookup"><span data-stu-id="722bd-137">In the **Configured permissions** , remove the delegated **User.Read** permission under **Microsoft Graph** by selecting the **...** to the right of the permission and selecting **Remove permission** .</span></span> <span data-ttu-id="722bd-138">Нажмите кнопку **Да, удалить** для подтверждения.</span><span class="sxs-lookup"><span data-stu-id="722bd-138">Select **Yes, remove** to confirm.</span></span>

1. <span data-ttu-id="722bd-139">Нажмите кнопку **предоставить согласие администратора для...** , а затем выберите **Да** , чтобы предоставить согласие администратора для настроенных разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="722bd-139">Select the **Grant admin consent for...** button, then select **Yes** to grant admin consent for the configured application permissions.</span></span> <span data-ttu-id="722bd-140">В столбце **состояние** в **настроенной таблице разрешений** изменяется значение **предоставлено для...** .</span><span class="sxs-lookup"><span data-stu-id="722bd-140">The **Status** column in the **Configured permissions** table changes to **Granted for ...** .</span></span>

    ![Снимок экрана с настроенными разрешениями для веб-перехватчика с предоставлением разрешения администратора](./images/configured-permissions.png)

1. <span data-ttu-id="722bd-142">Выберите **Сертификаты и секреты** в разделе **Управление** .</span><span class="sxs-lookup"><span data-stu-id="722bd-142">Select **Certificates & secrets** under **Manage** .</span></span> <span data-ttu-id="722bd-143">Нажмите кнопку **отправить сертификат** .</span><span class="sxs-lookup"><span data-stu-id="722bd-143">Select the **Upload certificate** button.</span></span> <span data-ttu-id="722bd-144">Перейдите к файлу открытого ключа сертификата и нажмите кнопку **Добавить** .</span><span class="sxs-lookup"><span data-stu-id="722bd-144">Browse to your certificate's public key file and select **Add** .</span></span>

# <a name="powershell"></a>[<span data-ttu-id="722bd-145">PowerShell</span><span class="sxs-lookup"><span data-stu-id="722bd-145">PowerShell</span></span>](#tab/powershell)

> [!NOTE]
> <span data-ttu-id="722bd-146">Необходимо [установить](installation.md) пакет SDK для Microsoft Graph PowerShell, прежде чем выполнять указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="722bd-146">You must have the Microsoft Graph PowerShell SDK [installed](installation.md) before following these steps.</span></span>

<span data-ttu-id="722bd-147">Вы можете заинтересовать: "я могу использовать пакет SDK PowerShell для регистрации приложения, чтобы можно было использовать пакет SDK PowerShell?"</span><span class="sxs-lookup"><span data-stu-id="722bd-147">You may be wondering: "I can use the PowerShell SDK to register an app, so that I can use the PowerShell SDK?"</span></span> <span data-ttu-id="722bd-148">Нет!</span><span class="sxs-lookup"><span data-stu-id="722bd-148">Yes!</span></span> <span data-ttu-id="722bd-149">В этом случае используется пакет SDK PowerShell с делегированным доступом, вход в систему в качестве администратора и создание регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="722bd-149">In this case, you're using the PowerShell SDK with delegated access, logging in as an administrator, and creating the app registration.</span></span> <span data-ttu-id="722bd-150">Затем с помощью регистрации этого приложения вы можете использовать пакет SDK для PowerShell с доступом только для приложений, что позволит использовать сценарии для автоматической установки.</span><span class="sxs-lookup"><span data-stu-id="722bd-150">Then, using that app registration, you're able to use the PowerShell SDK with app-only access, allowing for unattended scripts.</span></span>

1. <span data-ttu-id="722bd-151">С помощью текстового редактора создайте новый файл с именем **RegisterAppOnly.ps1** .</span><span class="sxs-lookup"><span data-stu-id="722bd-151">Use a text editor to create a new file named **RegisterAppOnly.ps1** .</span></span> <span data-ttu-id="722bd-152">Вставьте в файл следующий код.</span><span class="sxs-lookup"><span data-stu-id="722bd-152">Paste the following code into the file.</span></span>

    :::code language="powershell" source="RegisterAppOnly.ps1":::

1. <span data-ttu-id="722bd-153">Сохраните файл.</span><span class="sxs-lookup"><span data-stu-id="722bd-153">Save the file.</span></span> <span data-ttu-id="722bd-154">Откройте PowerShell в каталоге, содержащем **RegisterAppOnly.ps1** и выполните следующую команду.</span><span class="sxs-lookup"><span data-stu-id="722bd-154">Open PowerShell in the directory that contains **RegisterAppOnly.ps1** and run the following command.</span></span>

    ```powershell
    .\RegisterAppOnly.ps1 -AppName "Graph PowerShell Script" -CertPath "PATH_TO_PUBLIC_KEY_FILE"
    ```

1. <span data-ttu-id="722bd-155">Откройте браузер по своему запросу.</span><span class="sxs-lookup"><span data-stu-id="722bd-155">Open your browser as prompted.</span></span> <span data-ttu-id="722bd-156">Войдите в систему с учетной записью администратора и примите соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="722bd-156">Sign in with an administrator account and accept the permissions.</span></span>

1. <span data-ttu-id="722bd-157">Просмотрите выходные данные приглашения `Please go to the following URL in your browser to provide admin consent` .</span><span class="sxs-lookup"><span data-stu-id="722bd-157">Review the output for the prompt `Please go to the following URL in your browser to provide admin consent`.</span></span> <span data-ttu-id="722bd-158">Скопируйте предоставленный URL-адрес и вставьте его в браузере.</span><span class="sxs-lookup"><span data-stu-id="722bd-158">Copy the URL provided and paste it in your browser.</span></span> <span data-ttu-id="722bd-159">Войдите в систему, используя учетную запись администратора, чтобы предоставить согласие администратора для нового зарегистрированного приложения.</span><span class="sxs-lookup"><span data-stu-id="722bd-159">Sign in with an administrator account to grant admin consent to your newly registered application.</span></span>

    > [!NOTE]
    > <span data-ttu-id="722bd-160">После предоставления согласия администратора браузер отобразит сообщение об ошибке: `AADSTS500113: No reply address is registered for the application` .</span><span class="sxs-lookup"><span data-stu-id="722bd-160">After granting admin consent, the browser will display an error: `AADSTS500113: No reply address is registered for the application`.</span></span> <span data-ttu-id="722bd-161">Это связано с тем, что регистрация приложения не включает URL-адрес перенаправления.</span><span class="sxs-lookup"><span data-stu-id="722bd-161">This is because the app registration does not include a redirect URL.</span></span> <span data-ttu-id="722bd-162">Эту ошибку можно игнорировать.</span><span class="sxs-lookup"><span data-stu-id="722bd-162">This error can be ignored.</span></span>

1. <span data-ttu-id="722bd-163">Просмотрите остальные выходные данные PowerShell для команды, `Connect-MgGraph` заполненные значениями для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="722bd-163">Review the rest of the PowerShell output for `Connect-MgGraph` command pre-filled with the values for your app registration.</span></span>

---

## <a name="authenticate"></a><span data-ttu-id="722bd-164">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="722bd-164">Authenticate</span></span>

<span data-ttu-id="722bd-165">После выполнения описанных выше действий по настройке необходимо выполнить три части информации.</span><span class="sxs-lookup"><span data-stu-id="722bd-165">You should have three pieces of information after completing the configuration steps above.</span></span>

- <span data-ttu-id="722bd-166">Тема сертификата, отправленного в регистрацию приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="722bd-166">Certificate subject of the certificate uploaded to your Azure AD app registration.</span></span>
- <span data-ttu-id="722bd-167">Идентификатор приложения для регистрации приложения.</span><span class="sxs-lookup"><span data-stu-id="722bd-167">Application ID for your app registration.</span></span>
- <span data-ttu-id="722bd-168">Идентификатор клиента.</span><span class="sxs-lookup"><span data-stu-id="722bd-168">Your tenant ID.</span></span>

<span data-ttu-id="722bd-169">Используйте их для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="722bd-169">Let's use those to test authentication.</span></span> <span data-ttu-id="722bd-170">Откройте PowerShell и выполните следующую команду, заменив заполнители сведениями.</span><span class="sxs-lookup"><span data-stu-id="722bd-170">Open PowerShell and run the following command, replacing the placeholders with your information.</span></span>

```powershell
Connect-MgGraph -ClientID YOUR_APP_ID -TenantId YOUR_TENANT_ID -CertificateName YOUR_CERT_SUBJECT
```

<span data-ttu-id="722bd-171">В случае успеха вы увидите, что `Welcome To Microsoft Graph!` .</span><span class="sxs-lookup"><span data-stu-id="722bd-171">If this succeeds, you will see `Welcome To Microsoft Graph!`.</span></span> <span data-ttu-id="722bd-172">Запустите, `Get-MgContext` чтобы убедиться, что вы прошли проверку подлинности только для приложений.</span><span class="sxs-lookup"><span data-stu-id="722bd-172">Run `Get-MgContext` to verify that you've authenticated with app-only.</span></span> <span data-ttu-id="722bd-173">Выходные данные должны выглядеть так, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="722bd-173">The output should look like the following.</span></span>

```powershell
ClientId              : YOUR_APP_ID
TenantId              : YOUR_TENANT_ID
CertificateThumbprint :
Scopes                : {Group.Read.All, User.Read.All}
AuthType              : AppOnly
CertificateName       : YOUR_CERT_SUBJECT
Account               :
AppName               : Graph PowerShell Script
ContextScope          : Process
```

## <a name="create-the-script"></a><span data-ttu-id="722bd-174">Создание скрипта</span><span class="sxs-lookup"><span data-stu-id="722bd-174">Create the script</span></span>

<span data-ttu-id="722bd-175">Создайте новый файл с именем **GraphAppOnly.ps1** и добавьте следующий код.</span><span class="sxs-lookup"><span data-stu-id="722bd-175">Create a new file named **GraphAppOnly.ps1** and add the following code.</span></span>

```powershell
# Authenticate
Connect-MgGraph -ClientID YOUR_APP_ID -TenantId YOUR_TENANT_ID -CertificateName YOUR_CERT_SUBJECT

Write-Host "USERS:"
Write-Host "======================================================"
# List first 50 users
Get-MgUser -Property "id,displayName" -PageSize 50 | Format-Table DisplayName, Id

Write-Host "GROUPS:"
Write-Host "======================================================"
# List first 50 groups
Get-MgGroup -Property "id,displayName" -PageSize 50 | Format-Table DisplayName, Id

# Disconnect
Disconnect-MgGraph
```

<span data-ttu-id="722bd-176">Замените заполнители в `Connect-MgGraph` команде информацией.</span><span class="sxs-lookup"><span data-stu-id="722bd-176">Replace the placeholders in the `Connect-MgGraph` command with your information.</span></span> <span data-ttu-id="722bd-177">Сохраните файл, а затем откройте PowerShell в каталоге, в котором вы создали файл.</span><span class="sxs-lookup"><span data-stu-id="722bd-177">Save the file, then open PowerShell in the directory where you created the file.</span></span> <span data-ttu-id="722bd-178">Выполните сценарий с помощью приведенной ниже команды.</span><span class="sxs-lookup"><span data-stu-id="722bd-178">Run the script with the following command.</span></span>

```powershell
.\GraphAppOnly.ps1
```

<span data-ttu-id="722bd-179">Сценарий выводит список пользователей и групп, похожий на приведенные ниже выходные данные (сокращенный для краткости).</span><span class="sxs-lookup"><span data-stu-id="722bd-179">The script outputs a list of users and groups similar to the output below (truncated for brevity).</span></span>

```powershell
Welcome To Microsoft Graph!
USERS:
======================================================

DisplayName              Id
-----------              --
Conf Room Adams          88d1ba68-8ff5-4de2-90ed-768c00abcfae
Adele Vance              3103c7b9-cfe6-4cd3-a696-f88909b9a609
MOD Administrator        da3a885e-2d97-41de-9347-5271ef321b58
...

GROUPS:
======================================================

DisplayName                         Id
-----------                         --
App Development                     06dce3e5-d310-4add-ab2c-be728fb9076e
All Employees                       1a1cd42d-9801-4e9d-9b77-5215886174ef
Mark 8 Project Team                 2bf1b0d0-81f6-4e80-b971-d1db69f8d651
...
```
