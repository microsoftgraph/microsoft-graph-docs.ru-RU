---
title: Настройка единого входа на основе SAML с помощью API Microsoft Graph
description: Узнайте, как экономить время с помощью API Microsoft Graph, чтобы автоматизировать настройку единого входа на основе SAML.
author: kenwith
localization_priority: Priority
ms.prod: applications
ms.custom: scenarios:getting-started
ms.openlocfilehash: ea4a0a23b19b0b7a7250966f59e3a92e94a40618
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761474"
---
# <a name="configure-saml-based-single-sign-on-for-your-application-using-the-microsoft-graph-api"></a><span data-ttu-id="0bdac-103">Настройка единого входа на основе SAML для приложения с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0bdac-103">Configure SAML-based single sign-on for your application using the Microsoft Graph API</span></span>

<span data-ttu-id="0bdac-104">В этой статье вы узнаете, как создать и настроить единый вход на основе SAML для приложения в Azure Active Directory (Azure AD) с помощью API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0bdac-104">In this article, you'll learn how to create and configure a SAML-based single sign-on (SSO) for your application in Azure Active Directory (Azure AD) using the Microsoft Graph API.</span></span> <span data-ttu-id="0bdac-105">Конфигурация приложения включает основные URL-адреса SAML, политику сопоставления утверждений и использование сертификата для добавления пользовательского ключа подписи.</span><span class="sxs-lookup"><span data-stu-id="0bdac-105">The application configuration includes basic SAML URLs, a claims mapping policy, and using a certificate to add a custom signing key.</span></span> <span data-ttu-id="0bdac-106">После создания приложения назначьте для него пользователя, который будет администратором.</span><span class="sxs-lookup"><span data-stu-id="0bdac-106">After the application is created, you assign a user to it to be an administrator.</span></span> <span data-ttu-id="0bdac-107">После этого вы сможете использовать URL-адрес, чтобы получить метаданные SAML AD Azure для дополнительной настройки приложения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-107">You then can use a URL to obtain Azure AD SAML metadata for additional configuration of the application.</span></span> 

<span data-ttu-id="0bdac-108">В этой статье в качестве примера используется шаблон приложения Azure AD AWS, но описанные здесь шаги можно применить для любого другого приложения на основе SAML, включенного в коллекцию Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0bdac-108">This article uses an AWS Azure AD application template as an example, but you can use the steps in this article for any SAML-based app in the Azure AD Gallery.</span></span>

>[!NOTE]
><span data-ttu-id="0bdac-109">Объекты отклика и ключи, приведенные в этой статье, могут быть сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-109">The response objects and keys shown in this article might be shortened for readability.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bdac-110">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="0bdac-110">Prerequisites</span></span>

- <span data-ttu-id="0bdac-111">В этом руководстве вам потребуется самозаверяющий сертификат, с помощью которого Azure AD может подписать отклик SAML.</span><span class="sxs-lookup"><span data-stu-id="0bdac-111">In this tutorial, you need a self-signed certificate that Azure AD can use to sign a SAML response.</span></span> <span data-ttu-id="0bdac-112">Вы можете использовать собственный сертификат или следующий код C#, чтобы создать тестовый сертификат.</span><span class="sxs-lookup"><span data-stu-id="0bdac-112">You can use your own certificate or you could use something like the following C# code to create a test certificate:</span></span>

    > <span data-ttu-id="0bdac-113">**Примечание**. Этот код предназначен **ТОЛЬКО** для обучения и справочных материалов и не должен использоваться "как есть" в рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="0bdac-113">**Note** This code is for learning and reference **ONLY** and should not be used as-is in production.</span></span>

    ```C#
    using System;
    using System.Security.Cryptography;
    using System.Security.Cryptography.X509Certificates;
    using System.Text;

    /* CONSOLE APP - PROOF OF CONCEPT CODE ONLY!!
     * This code uses a self-signed certificate and should not be used 
     * in production. This code is for reference and learning ONLY.
     */
    namespace Self_signed_cert
    {
      class Program
      {
        static void Main(string[] args)
        {
          // Generate a guid to use as a password and then create the cert.
          string password = Guid.NewGuid().ToString();
          var selfsignedCert = buildSelfSignedServerCertificate(password);

          // Print values so we can copy paste into the JSON fields.
          // Print out the private key in base64 format.
          Console.WriteLine("Private Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Pfx, password)), Environment.NewLine);

          // Print out the start date in ISO 8601 format.
          DateTime startDate = DateTime.Parse(selfsignedCert.GetEffectiveDateString()).ToUniversalTime();
          Console.WriteLine("startDateTime: " + startDate.ToString("o"));

          // Print out the end date in ISO 8601 format.
          DateTime endDate = DateTime.Parse(selfsignedCert.GetExpirationDateString()).ToUniversalTime();
          Console.WriteLine("endDateTime: " + endDate.ToString("o"));

          // Print the GUID used for keyId
          string signAndPasswordGuid = Guid.NewGuid().ToString();
          string verifyGuid = Guid.NewGuid().ToString();
          Console.WriteLine("keyId GUID for Sign and passwordCredentials: " + signAndPasswordGuid);
          Console.WriteLine("keyId GUID for Verify: " + verifyGuid);

          // Print out the password.
          Console.WriteLine("Password: {0}", password);

          // Print out a displayName to use as an example.
          Console.WriteLine("displayName: CN=Example");
          Console.WriteLine();

          // Print out the public key.
          Console.WriteLine("Public Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Cert)), Environment.NewLine);
          Console.WriteLine();

          // Generate the customKeyIdentifier using hash of thumbprint.
          Console.WriteLine("Cert thumprint: {0}{1}", selfsignedCert.Thumbprint, Environment.NewLine);
          Console.WriteLine("customKeyIdentifier:");
          string keyIdentifier = GetSha256FromThumbprint(selfsignedCert.Thumbprint);
          Console.WriteLine(keyIdentifier);
        }

        // Generate a self-signed certificate.
        private static X509Certificate2 buildSelfSignedServerCertificate(string password)
        {
          const string CertificateName = @"Microsoft Azure Federated SSO Certificate TEST";
          DateTime certificateStartDate = DateTime.UtcNow;
          DateTime certificateEndDate = certificateStartDate.AddYears(2).ToUniversalTime();

          X500DistinguishedName distinguishedName = new X500DistinguishedName($"CN={CertificateName}");

          using (RSA rsa = RSA.Create(2048))
          {
            var request = new CertificateRequest(distinguishedName, rsa, HashAlgorithmName.SHA256, RSASignaturePadding.Pkcs1);

            request.CertificateExtensions.Add (
              new X509KeyUsageExtension(X509KeyUsageFlags.DataEncipherment | X509KeyUsageFlags.KeyEncipherment | X509KeyUsageFlags.DigitalSignature, false)
            );

            var certificate = request.CreateSelfSigned(new DateTimeOffset(certificateStartDate), new DateTimeOffset(certificateEndDate));
                certificate.FriendlyName = CertificateName;

            return new X509Certificate2(certificate.Export(X509ContentType.Pfx, password), password, X509KeyStorageFlags.Exportable);
          }
        }

        // Generate hash from thumbprint.
        public static string GetSha256FromThumbprint(string thumbprint)
        {
          var message = Encoding.ASCII.GetBytes(thumbprint);
          SHA256Managed hashString = new SHA256Managed();
          return Convert.ToBase64String(hashString.ComputeHash(message));
        }
      }
    }
    ```

    <span data-ttu-id="0bdac-114">Чтобы завершить это руководство, запишите следующие значения из своего сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-114">To complete this tutorial you need to record the following values from your certificate:</span></span>

    - <span data-ttu-id="0bdac-115">Закрытый ключ</span><span class="sxs-lookup"><span data-stu-id="0bdac-115">Private Key</span></span>
    - <span data-ttu-id="0bdac-116">Дата и время начала</span><span class="sxs-lookup"><span data-stu-id="0bdac-116">Start date and time</span></span>
    - <span data-ttu-id="0bdac-117">Дата и время окончания</span><span class="sxs-lookup"><span data-stu-id="0bdac-117">End date and time</span></span>
    - <span data-ttu-id="0bdac-118">Пароль сертификата</span><span class="sxs-lookup"><span data-stu-id="0bdac-118">Certificate password</span></span>
    - <span data-ttu-id="0bdac-119">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="0bdac-119">Display name</span></span>
    - <span data-ttu-id="0bdac-120">Открытый ключ</span><span class="sxs-lookup"><span data-stu-id="0bdac-120">Public key</span></span>
    - <span data-ttu-id="0bdac-121">Хэш отпечатка</span><span class="sxs-lookup"><span data-stu-id="0bdac-121">Hash of the thumbprint</span></span>
    - <span data-ttu-id="0bdac-122">Идентификатор ключа</span><span class="sxs-lookup"><span data-stu-id="0bdac-122">Key identifier</span></span>

    <span data-ttu-id="0bdac-123">В дополнение к значениям сертификата вам также потребуются два новых GUID для используемых keyId.</span><span class="sxs-lookup"><span data-stu-id="0bdac-123">In addition to the certificate values, you also need two new GUIDS for the keyIds that are used.</span></span> <span data-ttu-id="0bdac-124">В примере ниже показан результат приведенного выше кода.</span><span class="sxs-lookup"><span data-stu-id="0bdac-124">The following example shows the output of the previously listed code:</span></span>

    ```
    Private Key: MIIKW...AIBAzTVKCAgfQ

    startDateTime: 2020-12-17T20:33:07.0000000Z
    endDateTime: 2022-12-17T20:33:07.0000000Z
    keyId GUID for Sign and passwordCredentials: ed4f28e8-a502-4440-bfba-6038cb8506aa
    keyId GUID for Verify: e7b8c96e-dec3-4023-9c8b-ff40fa7faa3a
    Password: 74a7e867-e4f1-49a5-82fe-2087bf53e7df
    displayName: CN=Example

    Public Key: MIIDAz...pJTZg==

    Cert thumprint: 14B73D02E5094675063DF66A42B914DAD71633D7

    customKeyIdentifier:
    dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=
    ```

- <span data-ttu-id="0bdac-125">В этом руководстве предполагается, что вы используете песочницу Microsoft Graph, но вы можете использовать Postman или создать собственное клиентское приложение, чтобы вызывать Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0bdac-125">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="0bdac-126">Чтобы вызвать API Microsoft Graph в этом руководстве, используйте учетную запись с ролью глобального администратора и соответствующими разрешениями.</span><span class="sxs-lookup"><span data-stu-id="0bdac-126">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="0bdac-127">Для этого руководства требуются делегированные разрешения `Application.ReadWrite.All`, `AppRoleAssignment.ReadWrite.All`, `Policy.Read.All` и `Policy.ReadWrite.ApplicationConfiguration`.</span><span class="sxs-lookup"><span data-stu-id="0bdac-127">For this tutorial, the `Application.ReadWrite.All`, `AppRoleAssignment.ReadWrite.All`, `Policy.Read.All`, and `Policy.ReadWrite.ApplicationConfiguration` delegated permissions are needed.</span></span> <span data-ttu-id="0bdac-128">Чтобы настроить разрешения в песочнице Microsoft Graph, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="0bdac-128">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>

    1. <span data-ttu-id="0bdac-129">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="0bdac-129">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="0bdac-130">Выберите вариант **Вход с помощью учетной записи Майкрософт** и войдите, используя учетную запись глобального администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0bdac-130">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="0bdac-131">После успешного входа вы увидите данные учетной записи пользователя на панели слева.</span><span class="sxs-lookup"><span data-stu-id="0bdac-131">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="0bdac-132">Щелкните значок параметров справа от сведений об учетной записи пользователя и нажмите **Выбор разрешений**.</span><span class="sxs-lookup"><span data-stu-id="0bdac-132">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![Выбор разрешений Microsoft Graph](./images/application-saml-sso-configure-api/set-permissions.png)
        
    4. <span data-ttu-id="0bdac-134">Прокрутите список разрешений до разрешений `AppRoleAssignment`, разверните **AppRoleAssignment (1)** и выберите разрешение **AppRoleAssignment.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="0bdac-134">Scroll through the list of permissions to the `AppRoleAssignment` permissions, expand **AppRoleAssignment (1)**, and select the **AppRoleAssignment.ReadWrite.All** permission.</span></span> <span data-ttu-id="0bdac-135">Прокрутите ниже список разрешений до разрешений `Application`, разверните **Application (2)** и выберите разрешение **Application.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="0bdac-135">Scroll further down the list of permissions to the `Application` permissions, expand **Application (2)**, and select the **Application.ReadWrite.All** permission.</span></span> <span data-ttu-id="0bdac-136">Перейдите к разрешениям `Policy`, разверните **Policy (13)** и выберите разрешения **Policy.Read.All** и **Policy.ReadWrite.ApplicationConfiguration**.</span><span class="sxs-lookup"><span data-stu-id="0bdac-136">Continue to the `Policy` permissions, expand **Policy (13)**, and select the **Policy.Read.All**  and **Policy.ReadWrite.ApplicationConfiguration** permissions.</span></span>

        ![Прокрутка списка и выбор разрешений approleassignment, application и policy](./images/application-saml-sso-configure-api/select-permissions.png)

    5. <span data-ttu-id="0bdac-138">Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-138">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="0bdac-139">Вам не нужно предоставлять согласие от имени организации для этих разрешений.</span><span class="sxs-lookup"><span data-stu-id="0bdac-139">You do not need to consent on behalf of your organization for these permissions.</span></span>

        ![Согласие на разрешения](./images/application-saml-sso-configure-api/accept-permissions.png)

## <a name="step-1-create-the-application"></a><span data-ttu-id="0bdac-141">Шаг 1. Создание приложения</span><span class="sxs-lookup"><span data-stu-id="0bdac-141">Step 1: Create the application</span></span>

<span data-ttu-id="0bdac-142">В Azure AD есть коллекция, содержащая тысячи предварительно интегрированных приложений, которые можно использовать в качестве шаблонов для приложения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-142">Azure AD has a gallery that contains thousands of pre-integrated applications that you can use as a template for your application.</span></span> <span data-ttu-id="0bdac-143">В шаблоне приложения описаны метаданные для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-143">The application template describes the metadata for that application.</span></span> <span data-ttu-id="0bdac-144">По этому шаблону вы можете создать экземпляр приложения и субъект-службу в клиенте для управления им.</span><span class="sxs-lookup"><span data-stu-id="0bdac-144">Using this template, you can create an instance of the application and service principal in your tenant for management.</span></span> 

<span data-ttu-id="0bdac-145">Чтобы создать приложение из коллекции, сначала получите идентификатор шаблона приложения и используйте его для создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-145">To create the application from the gallery, you first get the identifier of the application template and then use that identifier to create the application.</span></span>

### <a name="retrieve-the-gallery-application-template-identifier"></a><span data-ttu-id="0bdac-146">Получение идентификатора шаблона для приложения из коллекции</span><span class="sxs-lookup"><span data-stu-id="0bdac-146">Retrieve the gallery application template identifier</span></span>

 <span data-ttu-id="0bdac-147">В этом руководстве вы получаете идентификатор шаблона приложения для `Amazon Web Services (AWS)`.</span><span class="sxs-lookup"><span data-stu-id="0bdac-147">In this tutorial, you retrieve the identifier of the application template for `Amazon Web Services (AWS)`.</span></span> <span data-ttu-id="0bdac-148">Запишите значение свойства **id**, которое понадобится позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="0bdac-148">Record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-149">Request</span></span>

```http
GET https://graph.microsoft.com/beta/applicationTemplates?$filter=displayName eq 'Amazon Web Services (AWS)'
```

#### <a name="response"></a><span data-ttu-id="0bdac-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdac-150">Response</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applicationTemplates",
  "value": [
    {
      "id": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
      "displayName": "Amazon Web Services (AWS)",
      "homePageUrl": "http://aws.amazon.com/",
      "supportedSingleSignOnModes": [
        "password",
        "saml",
        "external"
      ],
      "supportedProvisioningTypes": [
        "sync"
      ],
      "logoUrl": "https://az495088.vo.msecnd.net/app-logo/aws_215.png",
      "categories": [
        "developerServices",
        "topApps"
      ],
      "publisher": "Amazon",
      "description": null
    }
  ]
}
```

### <a name="create-the-application"></a><span data-ttu-id="0bdac-151">Создание приложения</span><span class="sxs-lookup"><span data-stu-id="0bdac-151">Create the application</span></span>

<span data-ttu-id="0bdac-152">Используя значение **id**, записанное для шаблона приложения, создайте экземпляр приложения и субъект-службу в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0bdac-152">Using the **id** value that you recorded for the application template, create an instance of the application and service principal in your tenant.</span></span> <span data-ttu-id="0bdac-153">Запишите значение свойства **objectId** приложения и значение свойства **objectId** для субъекта-службы, чтобы применить их позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="0bdac-153">Record the value of the **objectId** property of the application and the value of the **objectId** property for the service principal to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-154">Request</span></span>

```http
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```

> [!NOTE]
> <span data-ttu-id="0bdac-155">Подождите некоторое время, пока приложение будет подготовлено в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0bdac-155">Allow some time for the app to be provisioned into your Azure AD tenant.</span></span> <span data-ttu-id="0bdac-156">Это не происходит сразу.</span><span class="sxs-lookup"><span data-stu-id="0bdac-156">It is not instant.</span></span> <span data-ttu-id="0bdac-157">Одной из стратегий является выполнение запроса GET для объекта приложения или субъекта-службы каждые 5–10 секунд до тех пор, пока запрос не будет успешным.</span><span class="sxs-lookup"><span data-stu-id="0bdac-157">One strategy is to do a GET query on the application or service principal object every 5-10 seconds until the query is successful.</span></span>

#### <a name="response"></a><span data-ttu-id="0bdac-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bdac-158">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.applicationServicePrincipal",
  "application": {
    "objectId": "8f558912-0ca3-4f1e-ab6e-66ad7fa4e7bb",
    "appId": "536c33dc-dc28-42c8-ba1d-406524d83ec3",
    "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
    "displayName": "AWS Contoso",
    "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
    "identifierUris": [],
    "publicClient": null,
    "replyUrls": [
      "https://signin.aws.amazon.com/saml"
    ],
    "logoutUrl": null,
    "samlMetadataUrl": null,
    "errorUrl": null,
    "groupMembershipClaims": null,
    "availableToOtherTenants": false
  },
  "servicePrincipal": {
    "objectId": "3161ab85-8f57-4ae0-82d3-7a1f71680b27",
    "deletionTimestamp": null,
    "accountEnabled": true,
    "appId": "536c33dc-dc28-42c8-ba1d-406524d83ec3",
    "appDisplayName": "AWS Contoso",
    "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
    "appRoleAssignmentRequired": true,
    "displayName": "AWS Contoso",
    "errorUrl": null,
    "logoutUrl": null,
    "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
    "samlMetadataUrl": null,
    "microsoftFirstParty": null,
    "publisherName": "Contoso",
    "preferredTokenSigningKeyThumbprint": null,
    "replyUrls": [
      "https://signin.aws.amazon.com/saml"
    ],
    "servicePrincipalNames": [
      "536c33dc-dc28-42c8-ba1d-406524d83ec3"
    ],
    "tags": [
      "WindowsAzureActiveDirectoryIntegratedApp"
    ],
    "notificationEmailAddresses": [],
    "keyCredentials": [],
    "passwordCredentials": []
  }
}
```

## <a name="step-2-configure-single-sign-on"></a><span data-ttu-id="0bdac-159">Шаг 2. Настройка единого входа</span><span class="sxs-lookup"><span data-stu-id="0bdac-159">Step 2: Configure single sign-on</span></span>

<span data-ttu-id="0bdac-160">В этом руководстве вы настраиваете `saml` в качестве режима единого входа для субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="0bdac-160">In this tutorial, you set `saml` as the single sign-on mode in the service principal.</span></span> <span data-ttu-id="0bdac-161">Используйте значение **objectId** для субъекта-службы, записанное ранее.</span><span class="sxs-lookup"><span data-stu-id="0bdac-161">Use the **objectId** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-162">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: servicePrincipal/json

{
  "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a><span data-ttu-id="0bdac-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdac-163">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls"></a><span data-ttu-id="0bdac-164">Настройка основных URL-адресов SAML</span><span class="sxs-lookup"><span data-stu-id="0bdac-164">Set basic SAML URLs</span></span>

<span data-ttu-id="0bdac-165">Используя значение **objectId** для приложения, записанное ранее, настройте URI идентификатора и URI перенаправления для AWS в объекте приложения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-165">Using the **objectId** for the application that you recorded earlier, set the identifier URI and redirect URI for AWS in the application object.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-166">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/applications/8f558912-0ca3-4f1e-ab6e-66ad7fa4e7bb
Content-type: applications/json

{
  "web": {
    "redirectUris": [
      "https://signin.aws.amazon.com/saml"
    ] 
  },
  "identifierUris": [
    "https://signin.aws.amazon.com/saml"
  ]    
}
```

#### <a name="response"></a><span data-ttu-id="0bdac-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bdac-167">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="add-app-roles-optional"></a><span data-ttu-id="0bdac-168">Добавление ролей приложения (необязательно)</span><span class="sxs-lookup"><span data-stu-id="0bdac-168">Add app roles (Optional)</span></span>

<span data-ttu-id="0bdac-169">Если приложение ожидает получить сведения о роли в маркере, добавьте определение ролей в объект приложения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-169">If the application requires the role information in the token, add the definition of the roles in the application object.</span></span> 

> [!NOTE] 
> <span data-ttu-id="0bdac-170">При добавлении ролей приложения не изменяйте стандартные роли приложения `msiam_access`.</span><span class="sxs-lookup"><span data-stu-id="0bdac-170">When adding app roles, don't modify the default app roles `msiam_access`.</span></span> 

<span data-ttu-id="0bdac-171">Используйте значение **objectId** для субъекта-службы, записанное ранее.</span><span class="sxs-lookup"><span data-stu-id="0bdac-171">Use the **objectId** for the service principal that you recorded earlier.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-172">Request</span></span>

```http
PATCH https://graph.microsoft.com/beta/serviceprincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: serviceprincipals/json

{
  "appRoles": [
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "msiam_access",
      "displayName": "msiam_access",
      "id": "7dfd756e-8c27-4472-b2b7-38c17fc5de5e",
      "isEnabled": true,
      "origin": "Application",
      "value": null
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Admin,WAAD",
      "displayName": "Admin,WAAD",
      "id": "454dc4c2-8176-498e-99df-8c4efcde41ef",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Finance,WAAD",
      "displayName": "Finance,WAAD",
      "id": "8642d5fa-18a3-4245-ab8c-a96000c1a217",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-finance,arn:aws:iam::212743507312:saml-provider/WAAD"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="0bdac-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bdac-173">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a><span data-ttu-id="0bdac-174">Шаг 3. Настройка сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="0bdac-174">Step 3: Configure claims mapping</span></span>

### <a name="create-a-claims-mapping-policy"></a><span data-ttu-id="0bdac-175">Создание политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="0bdac-175">Create a claims mapping policy</span></span>

<span data-ttu-id="0bdac-176">В дополнение к основным утверждениям настройте следующие, чтобы служба Azure AD включала их в маркер SAML.</span><span class="sxs-lookup"><span data-stu-id="0bdac-176">In addition to the basic claims, configure the following claims for Azure AD to emit in the SAML token:</span></span>

| <span data-ttu-id="0bdac-177">Имя утверждения</span><span class="sxs-lookup"><span data-stu-id="0bdac-177">Claim name</span></span> | <span data-ttu-id="0bdac-178">Источник</span><span class="sxs-lookup"><span data-stu-id="0bdac-178">Source</span></span>  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | <span data-ttu-id="0bdac-179">assignedroles</span><span class="sxs-lookup"><span data-stu-id="0bdac-179">assignedroles</span></span>| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | <span data-ttu-id="0bdac-180">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="0bdac-180">userprincipalname</span></span> |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | <span data-ttu-id="0bdac-181">"900"</span><span class="sxs-lookup"><span data-stu-id="0bdac-181">"900"</span></span> |
| <span data-ttu-id="0bdac-182">roles</span><span class="sxs-lookup"><span data-stu-id="0bdac-182">roles</span></span> | <span data-ttu-id="0bdac-183">assignedroles</span><span class="sxs-lookup"><span data-stu-id="0bdac-183">assignedroles</span></span> |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | <span data-ttu-id="0bdac-184">userprincipalname</span><span class="sxs-lookup"><span data-stu-id="0bdac-184">userprincipalname</span></span> |

> [!NOTE]
> <span data-ttu-id="0bdac-185">Некоторые ключи в политике сопоставления утверждений чувствительны к регистру (например, "Version").</span><span class="sxs-lookup"><span data-stu-id="0bdac-185">Some keys in the claims mapping policy are case sensitive (for example, "Version").</span></span> <span data-ttu-id="0bdac-186">Если появляется сообщение об ошибке "Свойство имеет недопустимое значение", это может быть проблема, связанная с регистром.</span><span class="sxs-lookup"><span data-stu-id="0bdac-186">If you receive an error message such as "Property has an invalid value", it might be a case sensitive issue.</span></span>

<span data-ttu-id="0bdac-187">Создайте политику сопоставления утверждений и запишите значение свойства **id**, которое понадобится позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="0bdac-187">Create the claims mapping policy and record the value of the **id** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-188">Request</span></span>

```http
POST https://graph.microsoft.com/beta/policies/claimsMappingPolicies
Content-type: claimsMappingPolicies/json

{
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

#### <a name="response"></a><span data-ttu-id="0bdac-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdac-189">Response</span></span>

```http
HTTP/1.1 201 OK
Content-type: claimsMappingPolicies/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/claimsMappingPolicies/$entity",
  "id": "218e7879-5330-4ca6-8bca-ddb1f2402e73",
  "deletedDateTime": null,
  "definition": [
    "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Source\":\"user\",\"ID\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
  "displayName": "AWS Claims Policy",
  "isOrganizationDefault": false
}
```

### <a name="assign-a-claims-mapping-policy-to-a-service-principal"></a><span data-ttu-id="0bdac-190">Назначение политики сопоставления утверждений субъекту-службе</span><span class="sxs-lookup"><span data-stu-id="0bdac-190">Assign a claims mapping policy to a service principal</span></span>

<span data-ttu-id="0bdac-191">Используйте значение **objectId** для субъекта-службы, записанное ранее, чтобы назначить ему политику сопоставления утверждений.</span><span class="sxs-lookup"><span data-stu-id="0bdac-191">Use the **objectId** for the service principal that you recorded earlier to assign a claims mapping policy to it.</span></span> <span data-ttu-id="0bdac-192">В тексте запроса используйте значение свойства **id** для политики сопоставления утверждений.</span><span class="sxs-lookup"><span data-stu-id="0bdac-192">Use the value of the **id** property for the claims mapping policy in the body of the request.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-193">Request</span></span>

```http
POST https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27/claimsMappingPolicies/$ref
Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73"
}
```

#### <a name="response"></a><span data-ttu-id="0bdac-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdac-194">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-4-configure-a-signing-certificate"></a><span data-ttu-id="0bdac-195">Шаг 4. Настройка сертификата для подписи</span><span class="sxs-lookup"><span data-stu-id="0bdac-195">Step 4: Configure a signing certificate</span></span>

<span data-ttu-id="0bdac-196">Назначьте сертификат приложению.</span><span class="sxs-lookup"><span data-stu-id="0bdac-196">Assign your certificate to the application.</span></span> 

#### <a name="request"></a><span data-ttu-id="0bdac-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-197">Request</span></span>

<span data-ttu-id="0bdac-198">В тексте запроса введите следующие значения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-198">In the request body, provide these values:</span></span>

<span data-ttu-id="0bdac-199">**keyCredentials — вход**</span><span class="sxs-lookup"><span data-stu-id="0bdac-199">**keyCredentials - Sign**</span></span>

- <span data-ttu-id="0bdac-200">**customKeyIdentifier** — хэш отпечатка сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-200">**customKeyIdentifier** - The hash of the certificate thumbprint.</span></span>
- <span data-ttu-id="0bdac-201">**endDateTime** — дата и время окончания сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-201">**endDateTime** - The end date and time of the certificate.</span></span>
- <span data-ttu-id="0bdac-202">**keyId** — идентификатор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0bdac-202">**keyId** - The identifier for the credential.</span></span> <span data-ttu-id="0bdac-203">Совпадает с аргументом keyId для **passwordCredentials**.</span><span class="sxs-lookup"><span data-stu-id="0bdac-203">Same as the keyId for the **passwordCredentials**.</span></span>
- <span data-ttu-id="0bdac-204">**startDateTime** — дата начала сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-204">**startDateTime** - The start date of the certificate.</span></span>
- <span data-ttu-id="0bdac-205">**key** — закрытый ключ сертификата в кодировке Base-64.</span><span class="sxs-lookup"><span data-stu-id="0bdac-205">**key** - The base-64 encoded private key of the certificate.</span></span>
- <span data-ttu-id="0bdac-206">**displayName** — отображаемое имя учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0bdac-206">**displayName** - The display name for the credentials.</span></span>

<span data-ttu-id="0bdac-207">**keyCredentials — проверка**</span><span class="sxs-lookup"><span data-stu-id="0bdac-207">**keyCredentials - Verify**</span></span>

- <span data-ttu-id="0bdac-208">**customKeyIdentifier** — хэш отпечатка сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-208">**customKeyIdentifier** - The hash of the certificate thumbprint.</span></span>
- <span data-ttu-id="0bdac-209">**endDateTime** — дата и время окончания сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-209">**endDateTime** - The end date and time of the certificate.</span></span>
- <span data-ttu-id="0bdac-210">**keyId** — идентификатор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0bdac-210">**keyId** - The identifier for the credential.</span></span>
- <span data-ttu-id="0bdac-211">**startDateTime** — дата начала сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-211">**startDateTime** - The start date of the certificate.</span></span>
- <span data-ttu-id="0bdac-212">**key** — открытый ключ сертификата в кодировке Base-64.</span><span class="sxs-lookup"><span data-stu-id="0bdac-212">**key** - The base-64 encoded public key of the certificate.</span></span>
- <span data-ttu-id="0bdac-213">**displayName** — отображаемое имя учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0bdac-213">**displayName** - The display name for the credentials.</span></span>

<span data-ttu-id="0bdac-214">**passwordCredentials**</span><span class="sxs-lookup"><span data-stu-id="0bdac-214">**passwordCredentials**</span></span>

- <span data-ttu-id="0bdac-215">**customKeyIdentifier** — хэш отпечатка сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-215">**customKeyIdentifier** - The hash of the certificate thumbprint.</span></span>
- <span data-ttu-id="0bdac-216">**keyId** — идентификатор учетных данных.</span><span class="sxs-lookup"><span data-stu-id="0bdac-216">**keyId** - The identifier for the credential.</span></span> <span data-ttu-id="0bdac-217">Совпадает с аргументом keyId для **keyCredentials — вход**.</span><span class="sxs-lookup"><span data-stu-id="0bdac-217">Same as the keyId for the **keyCredentials - Sign**.</span></span>
- <span data-ttu-id="0bdac-218">**endDateTime** — дата и время окончания сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-218">**endDateTime** - The end date and time of the certificate.</span></span>
- <span data-ttu-id="0bdac-219">**startDateTime** — дата начала сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-219">**startDateTime** - The start date of the certificate.</span></span>
- <span data-ttu-id="0bdac-220">**secretText** — пароль сертификата.</span><span class="sxs-lookup"><span data-stu-id="0bdac-220">**secretText** - The password for the certificate.</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: servicePrincipals/json

{
  "keyCredentials":[
    {
      "customKeyIdentifier": "dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=",
      "endDateTime": 2022-12-17T20:33:07.0000000Z",
      "keyId": "ed4f28e8-a502-4440-bfba-6038cb8506aa",
      "startDateTime": "2020-12-17T20:33:07.0000000Z",
      "type": "X509CertAndPassword",
      "usage": "Sign",
      "key":"MIIKIAIBAz.....HBgUrDgMCERE20nuTptI9MEFCh2Ih2jaaLZBZGeZBRFVNXeZmAAgIH0A==",
      "displayName": "CN=Example"
    },
    {
      "customKeyIdentifier": "dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=",
      "endDateTime": "2022-12-17T20:33:07.0000000Z",
      "keyId": "e35a7d11-fef0-49ad-9f3e-aacbe0a42c42",
      "startDateTime": "2020-12-17T20:33:07.0000000Z",
      "type": "AsymmetricX509Cert",
      "usage": "Verify",
      "key": "MIIDJzCCAg+gAw......CTxQvJ/zN3bafeesMSueR83hlCSyg==",
      "displayName": "CN=Example"
    }
  ],
  "passwordCredentials": [
    {
      "customKeyIdentifier": "dD5ft4q5qrAQVusP6dDI7qKPnvZQbhkCxl1uNXQXwX0=",
      "keyId": "ed4f28e8-a502-4440-bfba-6038cb8506aa",
      "endDateTime": "2022-01-27T19:40:33Z",
      "startDateTime": "2020-04-20T19:40:33Z",
      "secretText": "74a7e867-e4f1-49a5-82fe-2087bf53e7df"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="0bdac-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bdac-221">Response</span></span>

```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a><span data-ttu-id="0bdac-222">Активация пользовательского ключа подписывания</span><span class="sxs-lookup"><span data-stu-id="0bdac-222">Activate the custom signing key</span></span>

<span data-ttu-id="0bdac-223">Присвойте свойству **preferredTokenSigningKeyThumbprint** субъекта-службы значение отпечатка сертификата, который должен использоваться в Azure AD для подписи отклика SAML.</span><span class="sxs-lookup"><span data-stu-id="0bdac-223">You need to set the **preferredTokenSigningKeyThumbprint** property of the service principal to the thumbprint of the certificate that you want Azure AD to use to sign the SAML response.</span></span> 

#### <a name="request"></a><span data-ttu-id="0bdac-224">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-224">Request</span></span>

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27

Content-type: servicePrincipals/json

{
    "preferredTokenSigningKeyThumbprint": "14B73D02E5094675063DF66A42B914DAD71633D7"
}
```

#### <a name="response"></a><span data-ttu-id="0bdac-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bdac-225">Response</span></span>

```http
HTTP/1.1 204
```

## <a name="step-5-assign-users"></a><span data-ttu-id="0bdac-226">Шаг 5. Назначение пользователей</span><span class="sxs-lookup"><span data-stu-id="0bdac-226">Step 5: Assign users</span></span>

### <a name="create-a-user-account"></a><span data-ttu-id="0bdac-227">Создание учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="0bdac-227">Create a user account</span></span>

<span data-ttu-id="0bdac-228">В этом руководстве создается учетная запись пользователя, которая добавляется в приложение.</span><span class="sxs-lookup"><span data-stu-id="0bdac-228">For this tutorial, you create a user account that is added to the application.</span></span> <span data-ttu-id="0bdac-229">В тексте запроса измените contoso.com на доменное имя своего клиента.</span><span class="sxs-lookup"><span data-stu-id="0bdac-229">In the request body, change contoso.com to the domain name of your tenant.</span></span> <span data-ttu-id="0bdac-230">Информацию о клиенте можно найти на странице обзора в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0bdac-230">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="0bdac-231">Запишите **id** пользователя, чтобы применить его позднее в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="0bdac-231">Record the **id** of the user to be used later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-232">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a><span data-ttu-id="0bdac-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdac-233">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "mytestuser1@contoso.com"
}
```

### <a name="assign-a-user-to-the-application"></a><span data-ttu-id="0bdac-234">Назначение пользователя приложению</span><span class="sxs-lookup"><span data-stu-id="0bdac-234">Assign a user to the application</span></span>

<span data-ttu-id="0bdac-235">Назначьте субъекту-службе созданного пользователя и роль приложения `Admin,WAAD`.</span><span class="sxs-lookup"><span data-stu-id="0bdac-235">Assign the user that you created to the service principal and assign the `Admin,WAAD` app role.</span></span> 

<span data-ttu-id="0bdac-236">В тексте запроса введите следующие значения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-236">In the request body, provide these values:</span></span>

- <span data-ttu-id="0bdac-237">**principalId** — **идентификатор** созданной учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="0bdac-237">**principalId** - The **id** of the user account that you created.</span></span>
- <span data-ttu-id="0bdac-238">**appRoleId** — **идентификатор** добавленной роли приложения `Admin,WAAD`.</span><span class="sxs-lookup"><span data-stu-id="0bdac-238">**appRoleId** - The **id** of the `Admin,WAAD` app role that you added.</span></span>
- <span data-ttu-id="0bdac-239">**resourceId** — **идентификатор** субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="0bdac-239">**resourceId** - The **id** of the service principal.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-240">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27/appRoleAssignments
Content-type: appRoleAssignments/json

{
  "principalId": "3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4",
  "principalType": "User",
  "appRoleId":"454dc4c2-8176-498e-99df-8c4efcde41ef",
  "resourceId":"3161ab85-8f57-4ae0-82d3-7a1f71680b27"
}
```

#### <a name="response"></a><span data-ttu-id="0bdac-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdac-241">Response</span></span>

```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('39406665-d521-40b7-9218-55070cae56b5')/appRoleAssignments/$entity",
  "id": "jKL4BeO2yUag4xULULSkza2HXRq_atpHrViBM89X55s",
  "deletedDateTime": null,
  "appRoleId": "454dc4c2-8176-498e-99df-8c4efcde41ef",
  "createdDateTime": "2021-02-11T22:51:36.8978032Z",
  "principalDisplayName": "MyTestUser1",
  "principalId": "05f8a28c-b6e3-46c9-a0e3-150b50b4a4cd",
  "principalType": "User",
  "resourceDisplayName": "AWS Contoso",
  "resourceId": "39406665-d521-40b7-9218-55070cae56b5"
}
```

## <a name="step-6-get-azure-ad-saml-metadata"></a><span data-ttu-id="0bdac-242">Шаг 6. Получение метаданных SAML из Azure AD</span><span class="sxs-lookup"><span data-stu-id="0bdac-242">Step 6: Get Azure AD SAML metadata</span></span>

<span data-ttu-id="0bdac-243">Используйте следующий URL-адрес, чтобы получить метаданные SAML из Azure AD для конкретного настроенного приложения.</span><span class="sxs-lookup"><span data-stu-id="0bdac-243">Use the following URL to get the Azure AD SAML metadata for the specific configured application.</span></span> <span data-ttu-id="0bdac-244">Эти метаданные содержат такие сведения, как сертификат для подписи, идентификатор сущности Azure AD (entityID), служба единого входа Azure AD (SingleSignOnService) и т. д.</span><span class="sxs-lookup"><span data-stu-id="0bdac-244">The metadata contains information such as the signing certificate, Azure AD entityID, and Azure AD SingleSignOnService, among others.</span></span>

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

<span data-ttu-id="0bdac-245">Ниже показан пример того, что можно увидеть в приложении.</span><span class="sxs-lookup"><span data-stu-id="0bdac-245">The following shows an example of what you might see for your application:</span></span>

```
<EntityDescriptor xmlns="urn:oasis:names:tc:SAML:2.0:metadata" ID="_05fbbf53-e892-43c9-9300-1f6738ace02c" entityID="https://sts.windows.net/2f82f566-5953-43f4-9251-79c6009bdf24/">
<Signature xmlns="http://www.w3.org/2000/09/xmldsig#">

...

<SingleLogoutService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
</IDPSSODescriptor>
</EntityDescriptor>
```

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="0bdac-246">Шаг 7. Очистка ресурсов</span><span class="sxs-lookup"><span data-stu-id="0bdac-246">Step 7: Clean up resources</span></span>

<span data-ttu-id="0bdac-247">На этом шаге вы удаляете созданные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="0bdac-247">In this step, you remove the resources that you created.</span></span>


### <a name="delete-the-application"></a><span data-ttu-id="0bdac-248">Удаление приложения</span><span class="sxs-lookup"><span data-stu-id="0bdac-248">Delete the application</span></span>

<span data-ttu-id="0bdac-249">Удалите созданное приложение.</span><span class="sxs-lookup"><span data-stu-id="0bdac-249">Delete the application that you created.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-250">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-250">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/applications/4b01f51f-079b-4634-b767-7e19ad502cdb
```

#### <a name="response"></a><span data-ttu-id="0bdac-251">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdac-251">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-user-account"></a><span data-ttu-id="0bdac-252">Удаление учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="0bdac-252">Delete the user account</span></span>

<span data-ttu-id="0bdac-253">Удалите учетную запись пользователя MyTestUser1.</span><span class="sxs-lookup"><span data-stu-id="0bdac-253">Delete the MyTestUser1 user account.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-254">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-254">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4
```

#### <a name="response"></a><span data-ttu-id="0bdac-255">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdac-255">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-claims-mapping-policy"></a><span data-ttu-id="0bdac-256">Удаление политики сопоставления утверждений</span><span class="sxs-lookup"><span data-stu-id="0bdac-256">Delete the claims mapping policy</span></span>

<span data-ttu-id="0bdac-257">Удалите политику сопоставления утверждений.</span><span class="sxs-lookup"><span data-stu-id="0bdac-257">Delete the claims mapping policy.</span></span>

#### <a name="request"></a><span data-ttu-id="0bdac-258">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bdac-258">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73
```

#### <a name="response"></a><span data-ttu-id="0bdac-259">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bdac-259">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="0bdac-260">См. также</span><span class="sxs-lookup"><span data-stu-id="0bdac-260">See also</span></span>

- <span data-ttu-id="0bdac-261">Для AWS вы можете [включить подготовку пользователя](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api), чтобы автоматически получать все роли из учетной записи AWS.</span><span class="sxs-lookup"><span data-stu-id="0bdac-261">For AWS, you can [enable user provisioning](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api) to fetch all the roles from that AWS account.</span></span> <span data-ttu-id="0bdac-262">Дополнительные сведения см. в статье [Настройка утверждения роли, выдаваемого в маркере SAML](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span><span class="sxs-lookup"><span data-stu-id="0bdac-262">For more information, see [Configure the role claim issued in the SAML token](/azure/active-directory/develop/active-directory-enterprise-app-role-management).</span></span>
- <span data-ttu-id="0bdac-263">[Настройка утверждений, выпущенных в маркерах для конкретного приложения в клиенте](/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="0bdac-263">[Customize claims emitted in tokens for a specific app in a tenant](/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
- <span data-ttu-id="0bdac-264">Вы можете использовать API applicationTemplate для создания экземпляров [приложений не из коллекции](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal).</span><span class="sxs-lookup"><span data-stu-id="0bdac-264">You can use the applicationTemplate API to instantiate [Non-Gallery apps](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal).</span></span> <span data-ttu-id="0bdac-265">Используйте applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span><span class="sxs-lookup"><span data-stu-id="0bdac-265">Use applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>
- [<span data-ttu-id="0bdac-266">New-SelfSignedCertificate</span><span class="sxs-lookup"><span data-stu-id="0bdac-266">New-SelfSignedCertificate</span></span>](/powershell/module/pkiclient/new-selfsignedcertificate?view=win10-ps)
- [<span data-ttu-id="0bdac-267">applicationTemplate</span><span class="sxs-lookup"><span data-stu-id="0bdac-267">applicationTemplate</span></span>](/graph/api/resources/applicationtemplate?view=graph-rest-beta)
- [<span data-ttu-id="0bdac-268">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0bdac-268">appRoleAssignment</span></span>](/graph/api/resources/approleassignment?view=graph-rest-1.0)
- [<span data-ttu-id="0bdac-269">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="0bdac-269">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)
- [<span data-ttu-id="0bdac-270">application</span><span class="sxs-lookup"><span data-stu-id="0bdac-270">application</span></span>](/graph/api/resources/application?view=graph-rest-1.0)
- [<span data-ttu-id="0bdac-271">claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="0bdac-271">claimsMappingPolicy</span></span>](https://docs.microsoft.com/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)
- [<span data-ttu-id="0bdac-272">keyCredential</span><span class="sxs-lookup"><span data-stu-id="0bdac-272">keyCredential</span></span>](/graph/api/resources/keycredential?view=graph-rest-1.0)
