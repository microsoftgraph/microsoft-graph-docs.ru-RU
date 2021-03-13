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
# <a name="configure-saml-based-single-sign-on-for-your-application-using-the-microsoft-graph-api"></a>Настройка единого входа на основе SAML для приложения с помощью API Microsoft Graph

В этой статье вы узнаете, как создать и настроить единый вход на основе SAML для приложения в Azure Active Directory (Azure AD) с помощью API Microsoft Graph. Конфигурация приложения включает основные URL-адреса SAML, политику сопоставления утверждений и использование сертификата для добавления пользовательского ключа подписи. После создания приложения назначьте для него пользователя, который будет администратором. После этого вы сможете использовать URL-адрес, чтобы получить метаданные SAML AD Azure для дополнительной настройки приложения. 

В этой статье в качестве примера используется шаблон приложения Azure AD AWS, но описанные здесь шаги можно применить для любого другого приложения на основе SAML, включенного в коллекцию Azure AD.

>[!NOTE]
>Объекты отклика и ключи, приведенные в этой статье, могут быть сокращены для удобства чтения.

## <a name="prerequisites"></a>Предварительные требования

- В этом руководстве вам потребуется самозаверяющий сертификат, с помощью которого Azure AD может подписать отклик SAML. Вы можете использовать собственный сертификат или следующий код C#, чтобы создать тестовый сертификат.

    > **Примечание**. Этот код предназначен **ТОЛЬКО** для обучения и справочных материалов и не должен использоваться "как есть" в рабочей среде.

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

    Чтобы завершить это руководство, запишите следующие значения из своего сертификата.

    - Закрытый ключ
    - Дата и время начала
    - Дата и время окончания
    - Пароль сертификата
    - Отображаемое имя
    - Открытый ключ
    - Хэш отпечатка
    - Идентификатор ключа

    В дополнение к значениям сертификата вам также потребуются два новых GUID для используемых keyId. В примере ниже показан результат приведенного выше кода.

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

- В этом руководстве предполагается, что вы используете песочницу Microsoft Graph, но вы можете использовать Postman или создать собственное клиентское приложение, чтобы вызывать Microsoft Graph. Чтобы вызвать API Microsoft Graph в этом руководстве, используйте учетную запись с ролью глобального администратора и соответствующими разрешениями. Для этого руководства требуются делегированные разрешения `Application.ReadWrite.All`, `AppRoleAssignment.ReadWrite.All`, `Policy.Read.All` и `Policy.ReadWrite.ApplicationConfiguration`. Чтобы настроить разрешения в песочнице Microsoft Graph, выполните следующие действия.

    1. Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).
    2. Выберите вариант **Вход с помощью учетной записи Майкрософт** и войдите, используя учетную запись глобального администратора Azure AD. После успешного входа вы увидите данные учетной записи пользователя на панели слева.
    3. Щелкните значок параметров справа от сведений об учетной записи пользователя и нажмите **Выбор разрешений**.

        ![Выбор разрешений Microsoft Graph](./images/application-saml-sso-configure-api/set-permissions.png)
        
    4. Прокрутите список разрешений до разрешений `AppRoleAssignment`, разверните **AppRoleAssignment (1)** и выберите разрешение **AppRoleAssignment.ReadWrite.All**. Прокрутите ниже список разрешений до разрешений `Application`, разверните **Application (2)** и выберите разрешение **Application.ReadWrite.All**. Перейдите к разрешениям `Policy`, разверните **Policy (13)** и выберите разрешения **Policy.Read.All** и **Policy.ReadWrite.ApplicationConfiguration**.

        ![Прокрутка списка и выбор разрешений approleassignment, application и policy](./images/application-saml-sso-configure-api/select-permissions.png)

    5. Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения. Вам не нужно предоставлять согласие от имени организации для этих разрешений.

        ![Согласие на разрешения](./images/application-saml-sso-configure-api/accept-permissions.png)

## <a name="step-1-create-the-application"></a>Шаг 1. Создание приложения

В Azure AD есть коллекция, содержащая тысячи предварительно интегрированных приложений, которые можно использовать в качестве шаблонов для приложения. В шаблоне приложения описаны метаданные для этого приложения. По этому шаблону вы можете создать экземпляр приложения и субъект-службу в клиенте для управления им. 

Чтобы создать приложение из коллекции, сначала получите идентификатор шаблона приложения и используйте его для создания приложения.

### <a name="retrieve-the-gallery-application-template-identifier"></a>Получение идентификатора шаблона для приложения из коллекции

 В этом руководстве вы получаете идентификатор шаблона приложения для `Amazon Web Services (AWS)`. Запишите значение свойства **id**, которое понадобится позже в этом руководстве.

#### <a name="request"></a>Запрос

```http
GET https://graph.microsoft.com/beta/applicationTemplates?$filter=displayName eq 'Amazon Web Services (AWS)'
```

#### <a name="response"></a>Ответ

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

### <a name="create-the-application"></a>Создание приложения

Используя значение **id**, записанное для шаблона приложения, создайте экземпляр приложения и субъект-службу в клиенте. Запишите значение свойства **objectId** приложения и значение свойства **objectId** для субъекта-службы, чтобы применить их позже в этом руководстве.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```

> [!NOTE]
> Подождите некоторое время, пока приложение будет подготовлено в клиенте Azure AD. Это не происходит сразу. Одной из стратегий является выполнение запроса GET для объекта приложения или субъекта-службы каждые 5–10 секунд до тех пор, пока запрос не будет успешным.

#### <a name="response"></a>Отклик

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

## <a name="step-2-configure-single-sign-on"></a>Шаг 2. Настройка единого входа

В этом руководстве вы настраиваете `saml` в качестве режима единого входа для субъекта-службы. Используйте значение **objectId** для субъекта-службы, записанное ранее.

#### <a name="request"></a>Запрос

```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27
Content-type: servicePrincipal/json

{
  "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a>Ответ

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls"></a>Настройка основных URL-адресов SAML

Используя значение **objectId** для приложения, записанное ранее, настройте URI идентификатора и URI перенаправления для AWS в объекте приложения.

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204
```

### <a name="add-app-roles-optional"></a>Добавление ролей приложения (необязательно)

Если приложение ожидает получить сведения о роли в маркере, добавьте определение ролей в объект приложения. 

> [!NOTE] 
> При добавлении ролей приложения не изменяйте стандартные роли приложения `msiam_access`. 

Используйте значение **objectId** для субъекта-службы, записанное ранее.

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a>Шаг 3. Настройка сопоставления утверждений

### <a name="create-a-claims-mapping-policy"></a>Создание политики сопоставления утверждений

В дополнение к основным утверждениям настройте следующие, чтобы служба Azure AD включала их в маркер SAML.

| Имя утверждения | Источник  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | assignedroles| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | userprincipalname |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | "900" |
| roles | assignedroles |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | userprincipalname |

> [!NOTE]
> Некоторые ключи в политике сопоставления утверждений чувствительны к регистру (например, "Version"). Если появляется сообщение об ошибке "Свойство имеет недопустимое значение", это может быть проблема, связанная с регистром.

Создайте политику сопоставления утверждений и запишите значение свойства **id**, которое понадобится позже в этом руководстве.

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Ответ

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

### <a name="assign-a-claims-mapping-policy-to-a-service-principal"></a>Назначение политики сопоставления утверждений субъекту-службе

Используйте значение **objectId** для субъекта-службы, записанное ранее, чтобы назначить ему политику сопоставления утверждений. В тексте запроса используйте значение свойства **id** для политики сопоставления утверждений.

#### <a name="request"></a>Запрос

```http
POST https://graph.microsoft.com/beta/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27/claimsMappingPolicies/$ref
Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73"
}
```

#### <a name="response"></a>Ответ

```http
HTTP/1.1 204
```

## <a name="step-4-configure-a-signing-certificate"></a>Шаг 4. Настройка сертификата для подписи

Назначьте сертификат приложению. 

#### <a name="request"></a>Запрос

В тексте запроса введите следующие значения.

**keyCredentials — вход**

- **customKeyIdentifier** — хэш отпечатка сертификата.
- **endDateTime** — дата и время окончания сертификата.
- **keyId** — идентификатор учетных данных. Совпадает с аргументом keyId для **passwordCredentials**.
- **startDateTime** — дата начала сертификата.
- **key** — закрытый ключ сертификата в кодировке Base-64.
- **displayName** — отображаемое имя учетных данных.

**keyCredentials — проверка**

- **customKeyIdentifier** — хэш отпечатка сертификата.
- **endDateTime** — дата и время окончания сертификата.
- **keyId** — идентификатор учетных данных.
- **startDateTime** — дата начала сертификата.
- **key** — открытый ключ сертификата в кодировке Base-64.
- **displayName** — отображаемое имя учетных данных.

**passwordCredentials**

- **customKeyIdentifier** — хэш отпечатка сертификата.
- **keyId** — идентификатор учетных данных. Совпадает с аргументом keyId для **keyCredentials — вход**.
- **endDateTime** — дата и время окончания сертификата.
- **startDateTime** — дата начала сертификата.
- **secretText** — пароль сертификата.

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

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a>Активация пользовательского ключа подписывания

Присвойте свойству **preferredTokenSigningKeyThumbprint** субъекта-службы значение отпечатка сертификата, который должен использоваться в Azure AD для подписи отклика SAML. 

#### <a name="request"></a>Запрос

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/3161ab85-8f57-4ae0-82d3-7a1f71680b27

Content-type: servicePrincipals/json

{
    "preferredTokenSigningKeyThumbprint": "14B73D02E5094675063DF66A42B914DAD71633D7"
}
```

#### <a name="response"></a>Отклик

```http
HTTP/1.1 204
```

## <a name="step-5-assign-users"></a>Шаг 5. Назначение пользователей

### <a name="create-a-user-account"></a>Создание учетной записи пользователя

В этом руководстве создается учетная запись пользователя, которая добавляется в приложение. В тексте запроса измените contoso.com на доменное имя своего клиента. Информацию о клиенте можно найти на странице обзора в Azure Active Directory. Запишите **id** пользователя, чтобы применить его позднее в этом руководстве.

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Ответ

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

### <a name="assign-a-user-to-the-application"></a>Назначение пользователя приложению

Назначьте субъекту-службе созданного пользователя и роль приложения `Admin,WAAD`. 

В тексте запроса введите следующие значения.

- **principalId** — **идентификатор** созданной учетной записи пользователя.
- **appRoleId** — **идентификатор** добавленной роли приложения `Admin,WAAD`.
- **resourceId** — **идентификатор** субъекта-службы.

#### <a name="request"></a>Запрос

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

#### <a name="response"></a>Ответ

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

## <a name="step-6-get-azure-ad-saml-metadata"></a>Шаг 6. Получение метаданных SAML из Azure AD

Используйте следующий URL-адрес, чтобы получить метаданные SAML из Azure AD для конкретного настроенного приложения. Эти метаданные содержат такие сведения, как сертификат для подписи, идентификатор сущности Azure AD (entityID), служба единого входа Azure AD (SingleSignOnService) и т. д.

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

Ниже показан пример того, что можно увидеть в приложении.

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

## <a name="step-7-clean-up-resources"></a>Шаг 7. Очистка ресурсов

На этом шаге вы удаляете созданные ресурсы.


### <a name="delete-the-application"></a>Удаление приложения

Удалите созданное приложение.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/applications/4b01f51f-079b-4634-b767-7e19ad502cdb
```

#### <a name="response"></a>Ответ

```http
No Content - 204
```

### <a name="delete-the-user-account"></a>Удаление учетной записи пользователя

Удалите учетную запись пользователя MyTestUser1.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/v1.0/users/3ee91cc2-8edc-4f1a-8d71-7dd61348f8c4
```

#### <a name="response"></a>Ответ

```http
No Content - 204
```

### <a name="delete-the-claims-mapping-policy"></a>Удаление политики сопоставления утверждений

Удалите политику сопоставления утверждений.

#### <a name="request"></a>Запрос

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/218e7879-5330-4ca6-8bca-ddb1f2402e73
```

#### <a name="response"></a>Ответ

```http
No Content - 204
```

## <a name="see-also"></a>См. также

- Для AWS вы можете [включить подготовку пользователя](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api), чтобы автоматически получать все роли из учетной записи AWS. Дополнительные сведения см. в статье [Настройка утверждения роли, выдаваемого в маркере SAML](/azure/active-directory/develop/active-directory-enterprise-app-role-management).
- [Настройка утверждений, выпущенных в маркерах для конкретного приложения в клиенте](/azure/active-directory/develop/active-directory-claims-mapping).
- Вы можете использовать API applicationTemplate для создания экземпляров [приложений не из коллекции](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal). Используйте applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.
- [New-SelfSignedCertificate](/powershell/module/pkiclient/new-selfsignedcertificate?view=win10-ps)
- [applicationTemplate](/graph/api/resources/applicationtemplate?view=graph-rest-beta)
- [appRoleAssignment](/graph/api/resources/approleassignment?view=graph-rest-1.0)
- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0)
- [application](/graph/api/resources/application?view=graph-rest-1.0)
- [claimsMappingPolicy](https://docs.microsoft.com/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)
- [keyCredential](/graph/api/resources/keycredential?view=graph-rest-1.0)
