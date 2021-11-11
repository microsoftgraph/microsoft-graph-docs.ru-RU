---
title: Используйте microsoft Graph для настройки необходимых разрешений Azure AD Graph для регистрации приложений
description: Используйте microsoft Graph для настройки необходимых разрешений Azure AD Graph для регистрации приложений.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 25fac773056238bde7c50158eb09daf3f5080552
ms.sourcegitcommit: 6b5bee1a1cea92c1f3d6439110c4916eb8b249a5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/11/2021
ms.locfileid: "60908587"
---
# <a name="use-microsoft-graph-to-configure-required-azure-ad-graph-permissions-for-an-app-registration"></a>Используйте microsoft Graph для настройки необходимых разрешений Azure AD Graph для регистрации приложений

Azure Active Directory (Azure AD) Graph и будет отменена 30 июня 2022 г. В рамках этого пути отключено добавление разрешений Azure AD Graph необходимых разрешений для регистрации приложений через портал Azure. Рекомендуется выполнять контрольный [](migrate-azure-ad-graph-planning-checklist.md) список планирования миграции приложений, чтобы помочь вам перейти к API [Graph](/graph/overview) Microsoft.

Однако может потребоваться добавить в приложение дополнительные Graph Azure AD. В этой статье приводится руководство по использованию microsoft Graph для настройки необходимых разрешений для Azure AD Graph регистрации приложения.

> [!CAUTION]
> Любое приложение с помощью Azure AD Graph будет по-прежнему работать после 30 июня 2022 г. Дополнительные сведения см. в Graph [Приложения Azure AD](migrate-azure-ad-graph-overview.md)в Microsoft Graph.

## <a name="option-1-use-the-microsoft-graph-api"></a>Вариант 1. Использование API Graph Microsoft

API Graph приложения [](/graph/api/resources/application) Майкрософт включает свойство **requiredResourceAccess,** которое является коллекцией объектов [requiredResourceAccess.](/graph/api/resources/requiredresourceaccess) Используйте это свойство для настройки необходимых разрешений Azure AD Graph, как описано в следующих действиях.

### <a name="prerequisites"></a>Предварительные требования

Для выполнения следующих действий необходимы следующие ресурсы и привилегии:

+ Запустите запросы HTTP в инструменте по вашему выбору, например в [приложении, через Graph Explorer](https://aka.ms/ge)или Postman.
+ Запустите API как пользователь в роли глобального администратора или администратора приложений или как владелец целевой регистрации приложения. Дополнительные сведения о действиях, поддерживаемых этими ролями, см. в встроенной роли [Azure AD.](/azure/active-directory/roles/permissions-reference)
+ Приложению, используемом для внесения этих изменений, необходимо предоставить `Application.ReadWrite.All` разрешение.

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Шаг 1. Определение идентификации разрешений для службы Azure AD Graph, необходимых вашему приложению

Определение разрешений Azure AD Graph, необходимых вашему приложению, их ID-разрешений, а также ролей приложений (разрешений приложений) или делегирования разрешений. Вы можете получить документы разрешений из существующей регистрации приложений, которая имеет разрешение, настроенное путем прочтения  его свойства **requiredResourceAccess** либо в манифесте приложения на портале Azure, либо через API microsoft Graph. 

Azure AD Graph является уникальным приложением Azure AD, которое идентифицировано  `00000002-0000-0000-c000-000000000000` **свойством resourceAppId** свойства **requiredResourceAccess.**

### <a name="request"></a>Запрос

В следующем запросе извлекается Graph Azure AD и типы разрешений из существующего приложения, идентифицированного **id.** `f7748341-825c-46e9-a111-5e3b56ae015b`

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-get-serviceprincipal-azureadgraph"
}-->

```msgraph-interactive
https://graph.microsoft.com/v1.0/applications/f7748341-825c-46e9-a111-5e3b56ae015b?$select=requiredResourceAccess
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications(requiredResourceAccess)/$entity",
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

Из этого вывода, это разрешение ID делегированного разрешения User.Read в то время как это разрешение `311a71cc-e848-46a1-bdf8-97ff7156d8e6`  `3afa6a7d-9b1a-42eb-948e-1650a849e176` ID роли приложения *Application.Read.All.*

### <a name="step-2-add-required-azure-ad-graph-permissions-to-your-app"></a>Шаг 2. Добавление необходимых разрешений Azure AD Graph в приложение

В следующем примере API приложения [Update](/graph/api/application-update) вызывается для добавления необходимых разрешений Azure AD Graph в регистрацию приложений, идентифицированную по объекту `581088ba-83c5-4975-b8af-11d2d7a76e98` ID. На шаге 1 эти разрешения были соответственно делегирована *разрешениями и* ролью приложения *User.Read и Application.Read.All.*

> [!IMPORTANT]
> Чтобы обновить **свойство requiredResourceAccess,** необходимо передать существующие и новые разрешения. Передача только новых разрешений переописывает и удаляет существующие разрешения.

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

Убедитесь, что у регистрации приложения есть необходимые разрешения API, которые вы добавили в  шаге 2 с помощью API Microsoft Graph или с помощью страницы регистрации приложений на портале Azure.

#### <a name="use-the-microsoft-graph-get-applicationid-api"></a>Используйте API microsoft Graph GET /application/{id}

Следующий запрос извлекает свойства **id** и **requiredResourceAccess** приложения, идентифицированного **объектным id.** `581088ba-83c5-4975-b8af-11d2d7a76e98`

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98?$select=id,requiredResourceAccess
```

>**Примечание:** Несмотря на то, что вы настроили необходимые приложениям разрешения, эти разрешения не были предоставлены. Многие разрешения требуют согласия администратора, прежде чем они могут использоваться для доступа к данным организации.

## <a name="option-2-use-microsoft-graph-powershell"></a>Вариант 2. Использование Microsoft Graph PowerShell

В [кодлет Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true) в Microsoft Graph PowerShell включен параметр **RequiredResourceAccess,** который является коллекцией объектов **IMicrosoftGraphRequiredResourceAccess.** Этот параметр используется для настройки необходимых разрешений Azure AD Graph, как описано в следующих действиях.

### <a name="prerequisites"></a>Предварительные требования

Для выполнения следующих действий необходимы следующие привилегии:

+ Сеанс PowerShell с проверкой подлинности (например, с `Connect-MgGraph` помощью).
+ Microsoft Graph PowerShell должно быть предоставлено `Application.ReadWrite.All` разрешение.
+ Зарегистрированный пользователь должен получить роли глобального администратора или администратора приложений Azure AD или быть владельцем целевой регистрации приложения. Дополнительные сведения о действиях, поддерживаемых этими ролями, см. в встроенной роли [Azure AD.](/azure/active-directory/roles/permissions-reference)

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>Шаг 1. Определение идентификации разрешений для службы Azure AD Graph, необходимых вашему приложению

Определение разрешений Azure AD Graph, необходимых вашему приложению, их ID-разрешений, а также ролей приложений (разрешений приложений) или делегирования разрешений. Вы можете получить документы разрешений из существующей регистрации приложений, которая имеет разрешение, настроенное с помощью чтения  свойства **RequiredResourceAccess** либо в Манифесте приложения на портале Azure, либо с помощью скрипта PowerShell.

### <a name="request"></a>Запрос

Создайте новый скрипт PowerShell с **fetchPermissions.ps1** и добавьте следующий код. Этот код извлекает Graph Azure AD и типы разрешений из существующей регистрации приложения, идентифицированной по объекту `f7748341-825c-46e9-a111-5e3b56ae015b` ID. Замените `f7748341-825c-46e9-a111-5e3b56ae015b` исходный код объекта приложения.

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All" 

## Replace f7748341-825c-46e9-a111-5e3b56ae015b with the object ID of the existing app registration; then read and output the permission IDs and their types
$sourceAppId= 'f7748341-825c-46e9-a111-5e3b56ae015b' 
$sourceApp = Get-MgApplication -ApplicationId $sourceAppId 
$sourceApp.RequiredResourceAccess.ResourceAccess
```

Запустите сценарий с помощью следующей команды
```powershell
.\fetchPermissions.ps1
```

### <a name="response"></a>Отклик

Ниже приведен пример результата.

```powershell
Id                                   Type
--                                   ----
311a71cc-e848-46a1-bdf8-97ff7156d8e6 Scope
3afa6a7d-9b1a-42eb-948e-1650a849e176 Role
```

Из этого вывода, это разрешение ID делегированного разрешения User.Read в то время как это разрешение `311a71cc-e848-46a1-bdf8-97ff7156d8e6`  `3afa6a7d-9b1a-42eb-948e-1650a849e176` ID роли приложения *Application.Read.All.*

### <a name="step-2-add-azure-ad-graph-permissions-to-your-app"></a>Шаг 2. Добавление разрешений Azure AD Graph в приложение

Создайте новый скрипт PowerShell с **updatePermissions.ps1** и добавьте следующий код. Этот код добавляет необходимые разрешения Azure AD Graph для регистрации приложения, идентифицированного по объекту `581088ba-83c5-4975-b8af-11d2d7a76e98` ID. На шаге 1 эти разрешения были соответственно делегирована *разрешениями и* ролью приложения *User.Read и Application.Read.All.*

> [!IMPORTANT]
> Чтобы обновить **свойство RequiredResourceAccess,** необходимо передать существующие и новые разрешения. Передача только новых разрешений переописывает и удаляет существующие разрешения.

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

## <a name="see-also"></a>См. также

+ [API приложения](/graph/api/resources/application)
+ [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true)
