---
title: Настройка необходимых разрешений Azure AD Graph для регистрации приложений
description: Настройка необходимых разрешений Azure AD Graph для регистрации приложений.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: fa74def34e93bed88513e564931a5b6557ed1bc8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334991"
---
# <a name="configure-required-azure-ad-graph-permissions-for-an-app-registration"></a>Настройка необходимых разрешений Azure AD Graph для регистрации приложений

Azure Active Directory (Azure AD) Graph и будет отменена в ближайшем будущем. В рамках этого пути амортизации добавление разрешений Azure AD Graph для регистрации приложений через портал Azure теперь отключено. Рекомендуется выполнять контрольный список планирования миграции [приложений](migrate-azure-ad-graph-planning-checklist.md), чтобы помочь вам перейти к API [Graph](/graph/overview) Microsoft.

Однако для доступа к ресурсам может потребоваться временное Graph Azure AD. В этой статье описаны следующие четыре метода настройки необходимых разрешений Azure AD Graph для регистрации приложения:

1. [С помощью портала Azure можно найти API, которые использует организация](#option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses)
1. [Обновление манифеста приложения на портале Azure](#option-2-update-the-application-manifest-on-the-azure-portal)
1. [Использование API Microsoft Graph](#option-3-use-the-microsoft-graph-api)
1. [Использование SDK Graph Microsoft Graph PowerShell](#option-4-use-the-microsoft-graph-powershell-sdk)

> [!CAUTION]
> Любое приложение с Graph Azure AD по-прежнему перестает функционировать после выхода Graph API Azure API. Дополнительные сведения см. в [Graph Azure AD в Microsoft Graph](migrate-azure-ad-graph-overview.md).

## <a name="option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses"></a>Вариант 1. Используйте портал Azure, чтобы найти API, которые использует организация

1. Во входе на [портал Azure](https://portal.azure.com) в качестве глобального администратора или администратора приложений.
1. Поиск и выбор **Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В **окне регистраций** приложений в вкладке **Все** приложения выберите приложение, для которого необходимо добавить Graph Azure AD. Это открывает области **Обзор регистрации** приложений.
1. В левой области окна в группе **Управление** меню выберите **разрешения API**. В этом случае раскрываются **настроенные разрешения для** регистрации приложения. Выберите **Добавить разрешение**.
1. В **раскрытом** окне разрешений API запроса переключение на **API** моя организация использует вкладку и поиск или `Windows Azure Active Directory` `00000002-0000-0000-c000-000000000000`. Выберите из фильтрованного списка, чтобы выявить **окно Azure Active Directory Graph** разрешений.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AzureADGraphPermissionsAPI.png" alt-text="API Graph Azure AD Windows Azure Active Directory и clientID 00000002-0000-0000-c000-0000000000000000000." border="true":::

1. Выберите **вкладку Делегирование** разрешений или разрешений приложений, чтобы выбрать из делегированного и приложения разрешений соответственно. Выберите **Добавление разрешений** для добавления разрешения на регистрацию приложения.
1. После добавления необходимых разрешений в окне Настройка разрешений выберите согласие администратора Гранта  на предоставление разрешений Azure AD Graph регистрации приложения.

## <a name="option-2-update-the-application-manifest-on-the-azure-portal"></a>Вариант 2. Обновление манифеста приложения на портале Azure

1. Во входе на [портал Azure](https://portal.azure.com) в качестве глобального администратора или администратора приложений.
1. Поиск и выбор **Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В **окне регистраций** приложений в вкладке **Все** приложения выберите приложение, для которого необходимо добавить Graph Azure AD. Это открывает области **Обзор регистрации** приложений.
1. В левой области окна в группе **Управление** меню выберите **Манифест**. Это открывает редактор, который позволяет напрямую редактировать атрибуты объекта регистрации приложений.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppRegistrationManifest.png" alt-text="Файл манифеста регистрации приложений позволяет изменять атрибуты приложения." border="true":::

1. Тщательно отредактировать **свойство requiredResourceAccess в** файле манифеста приложения, чтобы добавить следующие сведения:
    >**Примечание:** Вы можете изменить манифест приложения на портале Azure или выбрать Скачать  для локального редактирования манифеста, а затем использовать  Upload для повторного его применения в приложении.
+ Добавьте свойство **resourceAppId** и назначьте значение`00000002-0000-0000-c000-000000000000`, представляющее Azure AD Graph
+ Добавьте **свойство resourceAccess и** назначьте необходимые разрешения.

    В следующем фрагменте JSON показано свойство **requiredResourceAccess** с Azure AD Graph в качестве ресурса и назначено *user.Read* и *Application.Read.All* oauth2PermissionScope (делегированная разрешение) и appRole (разрешение приложения) соответственно.    

    ```JSON
    "requiredResourceAccess": [
        {
            "resourceAppId": "00000002-0000-0000-c000-000000000000",
            "resourceAccess": [
                {
                    "id": "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
                    "type": "Scope"
                },
                {
                    "id": "3afa6a7d-9b1a-42eb-948e-1650a849e176",
                    "type": "Role"
                }
            ]
        }
    ],
    ```

7. Сохраните изменения.
8. Выберите **разрешения API** и в настроенных  разрешениях для регистрации приложения выберите согласие администратора  Grant для предоставления разрешений Azure AD Graph регистрации приложения.

## <a name="option-3-use-the-microsoft-graph-api"></a>Вариант 3. Используйте API Graph Microsoft

API Graph приложения Майкрософт включает [](/graph/api/resources/application) свойство **requiredResourceAccess**, которое является коллекцией объектов [requiredResourceAccess](/graph/api/resources/requiredresourceaccess). Используйте это свойство для настройки необходимых разрешений Azure AD Graph, как описано в следующих действиях.

### <a name="prerequisites"></a>Предварительные условия

Для выполнения следующих действий необходимы следующие ресурсы и привилегии:

+ Запустите запросы HTTP в инструменте по вашему выбору, например в [приложении, через Graph Explorer](https://aka.ms/ge) или Postman.
+ Запустите API как пользователь в роли глобального администратора или администратора приложений или как владелец целевой регистрации приложения. Дополнительные сведения о действиях, поддерживаемых этими ролями, см. в встроенной роли [Azure AD](/azure/active-directory/roles/permissions-reference).
+ Приложению, используемом для внесения этих изменений, необходимо предоставить `Application.ReadWrite.All` разрешение.

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Шаг 1. Определение идентификации разрешений для службы Azure AD Graph, необходимых вашему приложению

Определите разрешения Azure AD Graph, необходимые вашему приложению, их идентификации разрешений, а также роли приложений (разрешения приложений) или oauth2PermissionScopes (делегированные разрешения).

Azure AD Graph как объект servicePrincipal `00000002-0000-0000-c000-000000000000` `Windows Azure Active Directory` с его уникальным во всем мире приложением и как **его displayName** и **appDisplayName**. Запустите следующий запрос для получения основного объекта службы для Azure AD Graph.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-get-serviceprincipal-azureadgraph"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$filter=appId eq '00000002-0000-0000-c000-000000000000'
```

#### <a name="response"></a>Отклик

В объекте ответа в объекте **appRoles** перечислены сведения для Azure AD Graph разрешения приложений, а в **объекте oauth2PermissionScopes** перечислены сведения о делегирования разрешений.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals",
    "value": [
        {
            "id": "1804a6f8-e623-4520-8f40-ba1b0c11c42d",
            "accountEnabled": true,
            "appDisplayName": "Windows Azure Active Directory",
            "appDescription": null,
            "appId": "00000002-0000-0000-c000-000000000000",
            "appOwnerOrganizationId": "f8cdef31-a31e-4b4a-93e4-5f571e91255a",
            "appRoleAssignmentRequired": false,
            "displayName": "Windows Azure Active Directory",
            "servicePrincipalNames": [
                "https://graph.windows.net",
                "00000002-0000-0000-c000-000000000000/graph.microsoftazure.us",
                "00000002-0000-0000-c000-000000000000/graph.windows.net",
                "00000002-0000-0000-c000-000000000000/directory.windows.net",
                "00000002-0000-0000-c000-000000000000",
                "https://graph.windows.net/",
                "https://graph.microsoftazure.us"
            ],
            "servicePrincipalType": "Application",
            "signInAudience": "AzureADMultipleOrgs",
            "appRoles": [
                {
                    "allowedMemberTypes": [
                        "Application"
                    ],
                    "description": "Allows the app to read applications and service principals without a signed-in user",
                    "displayName": "Read all applications",
                    "id": "3afa6a7d-9b1a-42eb-948e-1650a849e176",
                    "isEnabled": true,
                    "origin": "Application",
                    "value": "Application.Read.All"
                }
            ],
            "oauth2PermissionScopes": [
                {
                    "adminConsentDescription": "Allows users to sign in to the app, and allows the app to read the profile of signed-in users. It also allow the app to read basic company information of signed-in users.",
                    "adminConsentDisplayName": "Sign in and read user profile",
                    "id": "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
                    "isEnabled": true,
                    "type": "User",
                    "userConsentDescription": "Allows you to sign in to the app with your work account and let the app read your profile. It also allows the app to read basic company information.",
                    "userConsentDisplayName": "Sign you in and read your profile",
                    "value": "User.Read"
                }
            ]
        }
    ]
}
```

Из вышеуказанного `311a71cc-e848-46a1-bdf8-97ff7156d8e6` усеченного вывода — это ID разрешений для делегированных разрешений *User.Read*`3afa6a7d-9b1a-42eb-948e-1650a849e176`, в то время как это разрешение ID для *приложения Application.Read.All*.

### <a name="step-2-add-required-azure-ad-graph-permissions-to-your-app"></a>Шаг 2. Добавление необходимых разрешений Azure AD Graph в приложение

В следующем примере API приложения [Update](/graph/api/application-update) вызывается для добавления необходимых разрешений Azure AD Graph в регистрацию приложений, идентифицированную по объекту ID`581088ba-83c5-4975-b8af-11d2d7a76e98`. На шаге 1 эти разрешения были *соответственно разрешениями User.Read* и *Application.Read.All* .

> [!IMPORTANT]
> Чтобы обновить **свойство requiredResourceAccess** , необходимо передать существующие и новые разрешения. Передача только новых разрешений переописывает и удаляет существующие разрешения.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-update-application"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98
Content-Type: application/json

{
    "requiredResourceAccess": [
        {
            "resourceAppId": "00000002-0000-0000-c000-000000000000",
            "resourceAccess": [
                {
                    "id": "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
                    "type": "Scope"
                },
                {
                    "id": "3afa6a7d-9b1a-42eb-948e-1650a849e176",
                    "type": "Role"
                }
            ]
        }
    ]
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="step-3-verify-that-the-required-azure-ad-graph-permissions-were-added-to-your-app"></a>Шаг 3. Убедитесь, что необходимые разрешения Azure AD Graph в приложение

Убедитесь, что регистрация приложения имеет необходимые разрешения azure AD Graph API, которые вы добавили в шаге 2 с помощью API Microsoft Graph или проверив страницу регистрации  приложений на портале Azure.

#### <a name="use-the-microsoft-graph-get-applicationid-api"></a>Используйте API microsoft Graph GET /application/{id}

Следующий запрос извлекает свойства **id** и **requiredResourceAccess** приложения, идентифицированного **объектным id**`581088ba-83c5-4975-b8af-11d2d7a76e98`.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98?$select=id,requiredResourceAccess
```

>**Примечание:** Несмотря на то, что вы настроили необходимые приложениям разрешения, эти разрешения не были предоставлены. Многие разрешения требуют согласия администратора, прежде чем они могут использоваться для доступа к данным организации.

## <a name="option-4-use-the-microsoft-graph-powershell-sdk"></a>Вариант 4. Использование SDK microsoft Graph PowerShell

В [кодлете Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true) в Microsoft Graph PowerShell SDK включен параметр **RequiredResourceAccess**, который является коллекцией объектов **IMicrosoftGraphRequiredResourceAccess**. Этот параметр используется для настройки необходимых разрешений Azure AD Graph, как описано в следующих действиях.

### <a name="prerequisites"></a>Предварительные условия

Для выполнения следующих действий необходимы следующие привилегии:

+ Сеанс PowerShell с проверкой подлинности (например, с помощью `Connect-MgGraph`).
+ Microsoft Graph PowerShell должно быть предоставлено `Application.ReadWrite.All` разрешение.
+ Зарегистрированный пользователь должен получить роли глобального администратора или администратора приложений Azure AD или быть владельцем целевой регистрации приложения. Дополнительные сведения о действиях, поддерживаемых этими ролями, см. в встроенной роли [Azure AD](/azure/active-directory/roles/permissions-reference).

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Шаг 1. Определение идентификации разрешений для службы Azure AD Graph, необходимых вашему приложению

Определение разрешений Azure AD Graph, необходимых вашему приложению, их идентификации разрешений, а также роли приложений (разрешения приложений) или делегирование разрешений.

Azure AD Graph как объект ServicePrincipal `00000002-0000-0000-c000-000000000000` `Windows Azure Active Directory` с его уникальным во всем мире приложением и как **displayName** и **AppDisplayName**. Запустите следующий запрос для получения объекта ServicePrincipal для Azure AD Graph.

#### <a name="request"></a>Запрос

Создайте новый скрипт PowerShell с **fetchPermissions.ps1** и добавьте следующий код. В этом коде извлекаются Graph и типы разрешений Azure AD. Вывод отображает и форматирует выход объектов **AppRoles** и **Oauth2PermissionScopes** .

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All"

# Retrieve the service principal details for Azure AD Graph API.
$AADGraph = Get-MgServicePrincipal -Filter "appId eq '00000002-0000-0000-c000-000000000000'"

# Format output of the request above and display AppRoles (application permissions) and oauth2PermissionScopes (delegated permissions)
Echo "Azure AD Graph service principal object and its supported permissions:"
Echo "Application permissions:"
$AADGraph.AppRoles | Format-List
Echo "Delegated permissions:"
$AADGraph.Oauth2PermissionScopes | Format-List
```

Запустите сценарий с помощью следующей команды
```powershell
.\fetchPermissions.ps1
```

#### <a name="response"></a>Отклик

Ниже приведен пример результата.

```powershell
Welcome To Microsoft Graph!
Azure AD Graph service principal object and its supported permissions:
Application permissions:


AllowedMemberTypes   : {Application}
Description          : Allows the app to read applications and service principals without a signed-in user
DisplayName          : Read all applications
Id                   : 3afa6a7d-9b1a-42eb-948e-1650a849e176
IsEnabled            : True
Origin               : Application
Value                : Application.Read.All
AdditionalProperties : {}

Delegated permissions:


AdminConsentDescription : Allows users to sign in to the app, and allows the app to read the profile of signed-in users. It also allow the app to read basic company information of signed-in users.
AdminConsentDisplayName : Sign in and read user profile
Id                      : 311a71cc-e848-46a1-bdf8-97ff7156d8e6
IsEnabled               : True
Origin                  :
Type                    : User
UserConsentDescription  : Allows you to sign in to the app with your work account and let the app read your profile. It also allows the app to read basic company information.
UserConsentDisplayName  : Sign you in and read your profile
Value                   : User.Read
AdditionalProperties    : {}
```

Из этого вывода, `311a71cc-e848-46a1-bdf8-97ff7156d8e6` это разрешение ID делегированного разрешения *User.Read*`3afa6a7d-9b1a-42eb-948e-1650a849e176`, в то время как это разрешение ID *разрешения application.Read.All* разрешения приложения.

### <a name="step-2-add-azure-ad-graph-permissions-to-your-app"></a>Шаг 2. Добавление разрешений Azure AD Graph в приложение

Создайте новый скрипт PowerShell с **updatePermissions.ps1** и добавьте следующий код. Этот код добавляет необходимые разрешения Azure AD Graph регистрацию приложения, идентифицированную по объекту ID`581088ba-83c5-4975-b8af-11d2d7a76e98`. На шаге 1 эти разрешения были *соответственно разрешениями User.Read* и *Application.Read.All* .

> [!IMPORTANT]
> Чтобы обновить **свойство RequiredResourceAccess** , необходимо передать существующие и новые разрешения. Передача только новых разрешений переописывает и удаляет существующие разрешения.

#### <a name="request"></a>Запрос

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All" 

## Replace 581088ba-83c5-4975-b8af-11d2d7a76e98 with the object ID of the app you wish to add new permissions to
$applicationId = '581088ba-83c5-4975-b8af-11d2d7a76e98' 

$app = Get-MgApplication -ApplicationId $applicationId

## Azure AD Graph's globally unique appId is 00000002-0000-0000-c000-000000000000 identified by the ResourceAppId
$aadAccess = $app.RequiredResourceAccess | Where-Object { $_.ResourceAppId -eq '00000002-0000-0000-c000-000000000000' } 

if($null -eq $aadAccess){ 
    $app.RequiredResourceAccess += @{  
        ResourceAppId = "00000002-0000-0000-c000-000000000000"; 
        ResourceAccess = @( 

                ## Replace the following with values of ID and type for all permissions - both new and existing permissions - you want to configure for the app
                @{ 
                    # User.Read delegated permission Sign in and read user profile 
                    id = "311a71cc-e848-46a1-bdf8-97ff7156d8e6";  
                    type = "Scope"; 
                }, 
                @{ 
                    # Application.Read.All app role (application permission) to view application data
                    id = "3afa6a7d-9b1a-42eb-948e-1650a849e176"; 
                    type = "Role"; 
                }
            ) 
     } 
} 

Update-MgApplication -ApplicationId $applicationId -RequiredResourceAccess $app.RequiredResourceAccess 
```

Запустите скрипт с помощью следующей команды.
```powershell
.\updatePermissions.ps1
```

### <a name="response"></a>Отклик

Ниже приведен пример результата.

```powershell
Welcome To Microsoft Graph!
```

>**Примечание:** Несмотря на то, что вы настроили необходимые приложениям разрешения, эти разрешения не были предоставлены. Многие разрешения требуют согласия администратора, прежде чем они могут использоваться для доступа к данным организации.

## <a name="see-also"></a>Дополнительные ресурсы

+ [API приложения](/graph/api/resources/application)
+ [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true)
