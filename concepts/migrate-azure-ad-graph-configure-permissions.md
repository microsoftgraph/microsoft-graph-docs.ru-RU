---
title: Настройка необходимых Azure AD Graph для регистрации приложения
description: Настройте необходимые Azure AD Graph для регистрации приложения.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: a5c8e850f847a8fba3d6976d79715590ed85da62
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247268"
---
# <a name="configure-required-azure-ad-graph-permissions-for-an-app-registration"></a>Настройка необходимых Azure AD Graph для регистрации приложения

Azure Active Directory (Azure AD) Graph устарели и будут прекращены в ближайшем будущем. В рамках этого пути устаревания добавление Azure AD Graph к регистрации приложения через портал Azure отключено. Мы рекомендуем следовать контрольным спискам планирования миграции приложений, чтобы помочь вам перейти на [API microsoft Graph](/graph/overview).[](migrate-azure-ad-graph-planning-checklist.md)

Однако вашему приложению может потребоваться временное Azure AD Graph для доступа к ресурсам. В этой статье описаны следующие четыре метода настройки необходимых Azure AD Graph для регистрации приложения:

1. [Используйте портал Azure, чтобы найти API, которые использует ваша организация](#option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses)
1. [Обновление манифеста приложения на портал Azure](#option-2-update-the-application-manifest-on-the-azure-portal)
1. [Использование API Microsoft Graph](#option-3-use-the-microsoft-graph-api)
1. [Использование пакета SDK Microsoft Graph PowerShell](#option-4-use-the-microsoft-graph-powershell-sdk)

> [!CAUTION]
> Все приложения, использующие Azure AD Graph, по-прежнему перестанут работать после Azure AD API Graph прекращения поддержки. Дополнительные сведения см. в [статье "Перенос Azure AD Graph приложений в Microsoft Graph](migrate-azure-ad-graph-overview.md)".

## <a name="option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses"></a>Вариант 1. Используйте портал Azure, чтобы найти API, которые использует ваша организация

1. Войдите в портал Azure с [правами](https://portal.azure.com) глобального администратора или администратора приложений.
1. Найдите **и выберите Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В **окне Регистрация приложений** на вкладке "Все приложения" выберите приложение, для которого нужно Azure AD Graph разрешения. Откроется панель "Обзор" **регистрации** приложения.
1. В левой области окна в группе меню "Управление" выберите  **разрешения API**. Это показывает **настроенные разрешения для** регистрации приложения. Выберите **Добавить разрешение**.
1. В **появишемся** окне разрешений API запроса перейдите к **интерфейсам API** , используемым моей организацией, с помощью вкладки и `Windows Azure Active Directory` `00000002-0000-0000-c000-000000000000`найдите или . Выберите из отфильтрованного списка, **чтобы открыть окно Azure Active Directory Graph** разрешений.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AzureADGraphPermissionsAPI.png" alt-text="Azure AD API Graph идентифицируется по Windows Azure Active Directory и clientID 00000002-0000-0000-c000-0000000000000." border="true":::

1. Выберите **вкладку "Делегированные разрешения"** или **"Разрешения** приложения", чтобы выбрать из делегированных разрешений и разрешений приложения соответственно. Выберите **"Добавить разрешения** ", чтобы добавить разрешение на регистрацию приложения.
1. После добавления необходимых разрешений в окне "Настроенные разрешения" выберите "Предоставить согласие  администратора", чтобы предоставить Azure AD Graph разрешения на регистрацию приложения.

## <a name="option-2-update-the-application-manifest-on-the-azure-portal"></a>Вариант 2. Обновление манифеста приложения на портал Azure

1. Войдите в портал Azure с [правами](https://portal.azure.com) глобального администратора или администратора приложений.
1. Найдите **и выберите Azure Active Directory**.
1. В разделе **Управление** выберите **Регистрация приложений**.
1. В **окне Регистрация приложений** на вкладке "Все приложения" выберите приложение, для которого нужно Azure AD Graph разрешения. Откроется панель "Обзор" **регистрации** приложения.
1. В левой области окна в группе меню "Управление" выберите  "**Манифест"**. Откроется редактор, который позволяет напрямую редактировать атрибуты объекта регистрации приложения.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppRegistrationManifest.png" alt-text="Файл манифеста регистрации приложения позволяет изменять атрибуты приложения." border="true":::

1. Тщательно измените **свойство requiredResourceAccess** в файле манифеста приложения, чтобы добавить следующие сведения:
    >**Примечание:** Вы можете изменить манифест приложения на портал Azure или выбрать "Загрузить",  чтобы изменить манифест локально, а затем использовать Upload, чтобы  повторно применить его к приложению.
+ Добавьте свойство **resourceAppId** и назначьте значение, `00000002-0000-0000-c000-000000000000` представляющее Azure AD Graph
+ Добавьте свойство **resourceAccess** и назначьте необходимые разрешения.

    В следующем фрагменте кода JSON показано свойство **requiredResourceAccess** с Azure AD Graph в качестве ресурса и назначенные *User.Read* и *Application.Read.All* oauth2PermissionScope (делегированное разрешение) и appRole (разрешение приложения) соответственно.    

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
8. Выберите **разрешения API** и в разделе "Настроенные разрешения для регистрации приложения" выберите "Предоставить согласие администратора", чтобы предоставить Azure AD Graph разрешения на регистрацию приложения.

## <a name="option-3-use-the-microsoft-graph-api"></a>Вариант 3. Использование microsoft API Graph

API Graph Microsoft включает свойство [](/graph/api/resources/application) **requiredResourceAccess**, которое является коллекцией объектов [requiredResourceAccess](/graph/api/resources/requiredresourceaccess). Используйте это свойство для настройки необходимых Azure AD Graph разрешений, как описано в следующих шагах.

### <a name="prerequisites"></a>Необходимые условия

Для выполнения следующих действий вам потребуются следующие ресурсы и привилегии:

+ Выполните HTTP-запросы в выбранном средстве, например в [приложении, Graph Explorer](https://aka.ms/ge) или Postman.
+ Запустите API от имени пользователя с ролью глобального администратора или администратора приложений или от имени владельца регистрации целевого приложения. Дополнительные сведения о действиях, поддерживаемых этими ролями, см. Azure AD [встроенных ролей](/azure/active-directory/roles/permissions-reference).
+ Приложению, используемого для внесения этих изменений, должно быть предоставлено `Application.ReadWrite.All` разрешение.

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Шаг 1. Определение идентификаторов разрешений для Azure AD Graph разрешений, необходимых приложению

Определите Azure AD Graph, необходимые приложению, их идентификаторы разрешений, а также роли приложения (разрешения приложения) или oauth2PermissionScopes (делегированные разрешения).

Azure AD Graph как объект servicePrincipal `00000002-0000-0000-c000-000000000000` с его глобально уникальным идентификатором appId `Windows Azure Active Directory` и **как displayName** и **appDisplayName**. Выполните следующий запрос, чтобы получить объект субъекта-службы для Azure AD Graph.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-get-serviceprincipal-azureadgraph"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$filter=appId eq '00000002-0000-0000-c000-000000000000'
```

#### <a name="response"></a>Отклик

В объекте ответа в объекте **appRoles** перечислены Azure AD Graph разрешения приложения, а в **объекте oauth2PermissionScopes** — сведения о делегированных разрешениях.

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

Из указанных выше усеченных выходных данных — идентификатор разрешения для делегированного разрешения *User.Read*`3afa6a7d-9b1a-42eb-948e-1650a849e176`, `311a71cc-e848-46a1-bdf8-97ff7156d8e6` а идентификатор разрешения для *разрешения application.Read.All*.

### <a name="step-2-add-required-azure-ad-graph-permissions-to-your-app"></a>Шаг 2. Добавление необходимых Azure AD Graph разрешений в приложение

В следующем примере [вызывается](/graph/api/application-update) API приложения обновления для добавления необходимых разрешений Azure AD Graph к регистрации приложения, определяемой идентификатором объекта`581088ba-83c5-4975-b8af-11d2d7a76e98`. На шаге 1 эти разрешения были *делегированными разрешениями User.Read* и *Application.Read.All* соответственно.

> [!IMPORTANT]
> Чтобы обновить **свойство requiredResourceAccess** , необходимо передать как существующие, так и новые разрешения. Передача только новых разрешений перезаписывает и удаляет существующие разрешения.

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

### <a name="step-3-verify-that-the-required-azure-ad-graph-permissions-were-added-to-your-app"></a>Шаг 3. Убедитесь, что Azure AD Graph разрешения были добавлены в приложение.

Убедитесь, что у регистрации приложения есть необходимые разрешения Azure AD API Graph, добавленные на шаге 2 с помощью Microsoft API Graph или проверив страницу Регистрация приложений в  портал Azure.

#### <a name="use-the-microsoft-graph-get-applicationid-api"></a>Использование API GET /application/{id} microsoft Graph /application/{id}

Следующий запрос извлекает свойства **id** и **requiredResourceAccess** приложения, определенного идентификатором **объекта**`581088ba-83c5-4975-b8af-11d2d7a76e98`.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98?$select=id,requiredResourceAccess
```

>**Примечание:** Хотя вы настроите разрешения, необходимые приложению, эти разрешения не были предоставлены. Многие разрешения требуют согласия администратора, прежде чем их можно будет использовать для доступа к данным организации.

## <a name="option-4-use-the-microsoft-graph-powershell-sdk"></a>Вариант 4. Использование пакета SDK Microsoft Graph PowerShell

[Командлет Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true) в пакете SDK PowerShell для Microsoft Graph содержит параметр **RequiredResourceAccess**, который является коллекцией объектов **IMicrosoftGraphRequiredResourceAccess**. Используйте этот параметр для настройки необходимых Azure AD Graph разрешений, как описано в следующих шагах.

### <a name="prerequisites"></a>Необходимые условия

Для выполнения следующих действий требуются следующие привилегии:

+ Сеанс PowerShell, прошедший проверку подлинности (например, с использованием `Connect-MgGraph`).
+ Microsoft Graph PowerShell должно быть предоставлено `Application.ReadWrite.All` разрешение.
+ Вошедаму пользователю необходимо предоставить роль глобального администратора или администратора Azure AD каталога или быть владельцем регистрации целевого приложения. Дополнительные сведения о действиях, поддерживаемых этими ролями, см. Azure AD [встроенных ролей](/azure/active-directory/roles/permissions-reference).

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Шаг 1. Определение идентификаторов разрешений для Azure AD Graph разрешений, необходимых приложению

Определите Azure AD Graph, необходимые вашему приложению, их идентификаторы разрешений, а также роли приложения (разрешения приложения) или делегированные разрешения.

Azure AD Graph как объект ServicePrincipal `00000002-0000-0000-c000-000000000000` с его глобально уникальным идентификатором AppId `Windows Azure Active Directory` и **как displayName** и **AppDisplayName**. Выполните следующий запрос, чтобы получить объект ServicePrincipal для Azure AD Graph.

#### <a name="request"></a>Запрос

Создайте скрипт PowerShell с **именемfetchPermissions.ps1** и добавьте следующий код. Этот код извлекает Azure AD Graph и типы разрешений. Выходные данные отображают и форматирует выходные данные объектов **AppRoles** и **Oauth2PermissionScopes** .

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

Запустите скрипт с помощью следующей команды:
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

Из этих выходных `311a71cc-e848-46a1-bdf8-97ff7156d8e6` данных — идентификатор разрешения делегированного разрешения *User.Read*`3afa6a7d-9b1a-42eb-948e-1650a849e176`, а идентификатор разрешения *приложения Application.Read.All*.

### <a name="step-2-add-azure-ad-graph-permissions-to-your-app"></a>Шаг 2. Добавление Azure AD Graph в приложение

Создайте скрипт PowerShell с **именемupdatePermissions.ps1** и добавьте следующий код. Этот код добавляет необходимые разрешения Azure AD Graph к регистрации приложения, определяемой идентификатором объекта`581088ba-83c5-4975-b8af-11d2d7a76e98`. На шаге 1 эти разрешения были *делегированными разрешениями User.Read* и *Application.Read.All* соответственно.

> [!IMPORTANT]
> Чтобы обновить **свойство RequiredResourceAccess** , необходимо передать как существующие, так и новые разрешения. Передача только новых разрешений перезаписывает и удаляет существующие разрешения.

#### <a name="request"></a>Запрос

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All" 

## Azure AD Graph's globally unique appId is 00000002-0000-0000-c000-000000000000 identified by the ResourceAppId
$graphResourceId = "00000002-0000-0000-c000-000000000000"

## Replace 581088ba-83c5-4975-b8af-11d2d7a76e98 with the object ID of the app you wish to add new permissions to
$applicationId = '581088ba-83c5-4975-b8af-11d2d7a76e98' 

$app = Get-MgApplication -ApplicationId $applicationId

$aadAccess = $app.RequiredResourceAccess | Where-Object { $_.ResourceAppId -eq $graphResourceId } 

if ($null -eq $aadAccess) { 
    $app.RequiredResourceAccess += @{  
        ResourceAppId = $graphResourceId; 
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

    Update-MgApplication -ApplicationId $applicationId -RequiredResourceAccess $app.RequiredResourceAccess
}
else {
    $params = @{  
        ResourceAppId = $graphResourceId; 
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

    $params.ResourceAccess += $app.RequiredResourceAccess.ResourceAccess

    Update-MgApplication -ApplicationId $applicationId -RequiredResourceAccess $params 
}
```

Запустите скрипт, выполнив следующую команду.
```powershell
.\updatePermissions.ps1
```

### <a name="response"></a>Отклик

Ниже приведен пример результата.

```powershell
Welcome To Microsoft Graph!
```

>**Примечание:** Хотя вы настроите разрешения, необходимые приложению, эти разрешения не были предоставлены. Многие разрешения требуют согласия администратора, прежде чем их можно будет использовать для доступа к данным организации.

## <a name="see-also"></a>См. также

+ [API приложения](/graph/api/resources/application)
+ [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true)
