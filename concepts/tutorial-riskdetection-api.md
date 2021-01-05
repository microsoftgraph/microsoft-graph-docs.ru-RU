---
title: Учебник. Определение и устранение рисков с помощью API Microsoft Graph
description: Узнайте, как выявлять и устранять риски с помощью API Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8157760c8b0e5c9afb19c39a008870e2f7fe6009
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753762"
---
# <a name="tutorial-identify-and-remediate-risks-using-microsoft-graph-apis"></a><span data-ttu-id="6ee22-103">Учебник. Определение и устранение рисков с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="6ee22-103">Tutorial: Identify and remediate risks using Microsoft Graph APIs</span></span>

<span data-ttu-id="6ee22-104">Защита идентификации Azure AD предоставляет организациям представление о риске на основе удостоверений и различных способах исследования и автоматического устранения риска.</span><span class="sxs-lookup"><span data-stu-id="6ee22-104">Azure AD Identity Protection provides organizations insight into identity-based risk and different ways to investigate and automatically remediate risk.</span></span> <span data-ttu-id="6ee22-105">API защиты идентификации, используемые в этом руководстве, помогут вам определить риск и настроить рабочий процесс для подтверждения компрометации или устранения.</span><span class="sxs-lookup"><span data-stu-id="6ee22-105">The Identity Protection APIs used in this tutorial can help you identify risk and configure a workflow to confirm compromise or enable remediation.</span></span> <span data-ttu-id="6ee22-106">Дополнительные сведения см. [в этой теме.](/azure/active-directory/identity-protection/concept-identity-protection-risks)</span><span class="sxs-lookup"><span data-stu-id="6ee22-106">For more information, see [What is risk?](/azure/active-directory/identity-protection/concept-identity-protection-risks)</span></span>

<span data-ttu-id="6ee22-107">В этом руководстве вы узнаете, как создать рискованный вход и устранять состояние риска пользователя с помощью политики условного доступа, которая требует многофакторной проверки подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="6ee22-107">In this tutorial, you learn how to generate a risky sign-in and remediate the risk status of the user with a conditional access policy that requires multi-factor authentication (MFA).</span></span> <span data-ttu-id="6ee22-108">В дополнительном разделе показано, как заблокировать для пользователя вход с помощью политики условного доступа и снизить риск для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ee22-108">An optional section shows you how to block the user from signing in also using a conditional access policy, and dismissing the user risk.</span></span>

><span data-ttu-id="6ee22-109">**Примечание.** Объекты ответа, показанные в этом руководстве, могут быть сокращены для учитаемости.</span><span class="sxs-lookup"><span data-stu-id="6ee22-109">**Note:** The response objects shown in this tutorial might be shortened for readability.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="6ee22-110">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6ee22-110">Prerequisites</span></span>

<span data-ttu-id="6ee22-111">Чтобы успешно выполнить это руководство, убедитесь, что у вас есть необходимые условия:</span><span class="sxs-lookup"><span data-stu-id="6ee22-111">To successfully complete this tutorial, make sure that you have the required prerequisites:</span></span>

- <span data-ttu-id="6ee22-112">Для использования API обнаружения рисков вам требуется лицензия Azure AD Premium P1 или P2.</span><span class="sxs-lookup"><span data-stu-id="6ee22-112">You must have an Azure AD Premium P1 or P2 license to use the risk detection API.</span></span>
- <span data-ttu-id="6ee22-113">В этом руководстве используется браузер tor для анонимного вход на портал Azure.</span><span class="sxs-lookup"><span data-stu-id="6ee22-113">This tutorial uses the Tor browser to sign in to the Azure portal anonymously.</span></span> <span data-ttu-id="6ee22-114">Для выполнения задачи можно использовать любой анонимный браузер.</span><span class="sxs-lookup"><span data-stu-id="6ee22-114">You can use any anonymous browser to accomplish the task.</span></span> <span data-ttu-id="6ee22-115">Чтобы скачать браузер tor, см. ["Скачать браузер tor".](https://www.torproject.org/download/)</span><span class="sxs-lookup"><span data-stu-id="6ee22-115">To download the Tor browser, see [Download Tor Browser](https://www.torproject.org/download/).</span></span>
- <span data-ttu-id="6ee22-116">В этом руководстве предполагается, что вы используете проводник Microsoft Graph, но можете использовать Postman или создать собственное клиентские приложения для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6ee22-116">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="6ee22-117">Чтобы вызвать API Microsoft Graph в этом руководстве, необходимо использовать учетную запись с ролью глобального администратора и соответствующими разрешениями.</span><span class="sxs-lookup"><span data-stu-id="6ee22-117">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="6ee22-118">Чтобы настроить разрешения в проводнике Microsoft Graph, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="6ee22-118">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>
    1. <span data-ttu-id="6ee22-119">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="6ee22-119">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="6ee22-120">Выберите **вход с помощью Майкрософт** и во входе с помощью учетной записи глобального администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6ee22-120">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="6ee22-121">После успешного входе вы можете увидеть сведения об учетной записи пользователя в области слева.</span><span class="sxs-lookup"><span data-stu-id="6ee22-121">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="6ee22-122">Выберите значок параметров справа от сведений учетной записи пользователя, а затем выберите **"Выбор разрешений".**</span><span class="sxs-lookup"><span data-stu-id="6ee22-122">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![Установка разрешений](./images/tutorial-riskdetection-api/set-permissions.png)
        
    4. <span data-ttu-id="6ee22-124">Прокрутите список разрешений для этих разрешений:</span><span class="sxs-lookup"><span data-stu-id="6ee22-124">Scroll through the list of permissions to these permissions:</span></span>
        - <span data-ttu-id="6ee22-125">**IdentityRiskEvents (2)**, развернуть и выбрать `IdentityRiskEvent.Read.All`</span><span class="sxs-lookup"><span data-stu-id="6ee22-125">**IdentityRiskEvents (2)**, expand and then select `IdentityRiskEvent.Read.All`</span></span>
        - <span data-ttu-id="6ee22-126">**IdentityRiskyUser (2)**, развернуть и выбрать `IdentityRiskyUser.ReadWrite.All`</span><span class="sxs-lookup"><span data-stu-id="6ee22-126">**IdentityRiskyUser (2)**, expand and then select `IdentityRiskyUser.ReadWrite.All`</span></span>
        - <span data-ttu-id="6ee22-127">**Политика (13),** развернуть, а затем выбрать `Policy.Read.All` и `Policy.ReadWrite.ConditionalAccess`</span><span class="sxs-lookup"><span data-stu-id="6ee22-127">**Policy (13)**, expand and then select `Policy.Read.All` and `Policy.ReadWrite.ConditionalAccess`</span></span>
        - <span data-ttu-id="6ee22-128">**Пользователь (8)**, развернуть и выбрать `User.ReadWrite.All`</span><span class="sxs-lookup"><span data-stu-id="6ee22-128">**User (8)**, expand and then select `User.ReadWrite.All`</span></span>
        
        ![Поиск разрешений](./images/tutorial-riskdetection-api/permissions-consent.png)
    
    5. <span data-ttu-id="6ee22-130">Выберите **"Согласие",** а затем выберите **"Принять",** чтобы принять согласие на разрешения.</span><span class="sxs-lookup"><span data-stu-id="6ee22-130">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="6ee22-131">Для получения этих разрешений не требуется согласие от имени вашей организации.</span><span class="sxs-lookup"><span data-stu-id="6ee22-131">You do not need to consent on behalf of your organization for these permissions.</span></span>

        ![Принятие разрешений](./images/tutorial-riskdetection-api/accept-permissions.png)

## <a name="step-1-create-a-user-account"></a><span data-ttu-id="6ee22-133">Шаг 1. Создание учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="6ee22-133">Step 1: Create a user account</span></span>

<span data-ttu-id="6ee22-134">В этом руководстве вы создаете учетную запись пользователя, используемую для проверки обнаружения рисков.</span><span class="sxs-lookup"><span data-stu-id="6ee22-134">For this tutorial, you create a user account that is used to test risk detections.</span></span> <span data-ttu-id="6ee22-135">В теле запроса `contoso.com` измените доменное имя клиента.</span><span class="sxs-lookup"><span data-stu-id="6ee22-135">In the request body, change `contoso.com` to the domain name of your tenant.</span></span> <span data-ttu-id="6ee22-136">Сведения о клиенте можно найти на странице обзора Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6ee22-136">You can find tenant information on the Azure Active Directory overview page.</span></span>

### <a name="request"></a><span data-ttu-id="6ee22-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee22-137">Request</span></span>

``` http
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

### <a name="response"></a><span data-ttu-id="6ee22-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee22-138">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "givenName": null,
  "jobTitle": null,
  "mail": null,
  "mobilePhone": null,
  "officeLocation": null,
  "preferredLanguage": null,
  "surname": null,
  "userPrincipalName": "MyTestUser1@contoso.com"
}
```

## <a name="step-2-trigger-a-risk-detection"></a><span data-ttu-id="6ee22-139">Шаг 2. Запуск обнаружения рисков</span><span class="sxs-lookup"><span data-stu-id="6ee22-139">Step 2: Trigger a risk detection</span></span>

### <a name="trigger-a-risk-detection"></a><span data-ttu-id="6ee22-140">Запуск обнаружения рисков</span><span class="sxs-lookup"><span data-stu-id="6ee22-140">Trigger a risk detection</span></span>

<span data-ttu-id="6ee22-141">Один из способов обнаружения рисков для учетной записи пользователя — анонимный вход на портал Azure.</span><span class="sxs-lookup"><span data-stu-id="6ee22-141">One way to trigger a risk detection on a user account is to sign in to the Azure portal anonymously.</span></span> <span data-ttu-id="6ee22-142">В этом руководстве браузер tor используется для анонимного входов.</span><span class="sxs-lookup"><span data-stu-id="6ee22-142">In this tutorial, the Tor browser is used to sign in anonymously.</span></span> 

1. <span data-ttu-id="6ee22-143">Откройте браузер и введите `portal.azure.com` адрес сайта.</span><span class="sxs-lookup"><span data-stu-id="6ee22-143">Open the browser and enter `portal.azure.com` for the site address.</span></span>
2. <span data-ttu-id="6ee22-144">Во sign in to the portal using the credentials for the **MyTestUser1** account that you previously created.</span><span class="sxs-lookup"><span data-stu-id="6ee22-144">Sign in to the portal using the credentials for the **MyTestUser1** account that you previously created.</span></span> <span data-ttu-id="6ee22-145">Вам будет предложено изменить существующий пароль.</span><span class="sxs-lookup"><span data-stu-id="6ee22-145">You will be asked to change the existing password.</span></span>

### <a name="list-risk-detections"></a><span data-ttu-id="6ee22-146">Список обнаружений рисков</span><span class="sxs-lookup"><span data-stu-id="6ee22-146">List risk detections</span></span>

<span data-ttu-id="6ee22-147">Когда вы вошел на портал Azure с помощью анонимного браузера, было `anonymizedIPAddress` обнаружено событие риска.</span><span class="sxs-lookup"><span data-stu-id="6ee22-147">When you signed in to the Azure portal using the anonymous browser, an `anonymizedIPAddress` risk event was detected.</span></span> <span data-ttu-id="6ee22-148">Параметр запроса можно использовать для получения только обнаружений рисков, связанных с учетной записью `$filter` **пользователя MyTestUser1.**</span><span class="sxs-lookup"><span data-stu-id="6ee22-148">You can use the `$filter` query parameter to get only the risk detections that are associated with the **MyTestUser1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="6ee22-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee22-149">Request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a><span data-ttu-id="6ee22-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee22-150">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#riskDetections",
  "value": [
    {
      "id": "d52a631815aaa527bf642b196715da5cf0f35b6879204ea5b5c99b21bd4c16f4",
      "requestId": "06f7fd18-b8f1-407d-86a3-f6cbe3a4be00",
      "correlationId": "2a38abff-5701-4073-a81e-fd3aac09cba3",
      "riskType": "anonymizedIPAddress",
      "riskEventType": "anonymizedIPAddress",
      "riskState": "atRisk",
      "riskLevel": "medium",
      "riskDetail": "none",
      "source": "IdentityProtection",
      "detectionTimingType": "realtime",
      "activity": "signin",
      "tokenIssuerType": "AzureAD",
      "ipAddress": "178.17.170.23",
      "activityDateTime": "2020-11-03T20:51:34.6245276Z",
      "detectedDateTime": "2020-11-03T20:51:34.6245276Z",
      "lastUpdatedDateTime": "2020-11-03T20:53:12.1984203Z",
      "userId": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com",
      "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
      "location": {
        "city": "Chisinau",
        "state": "Chisinau",
        "countryOrRegion": "MD",
        "geoCoordinates": {
          "latitude": 47.0269,
          "longitude": 28.8416
        }
      }
    }
  ]
}
```

> <span data-ttu-id="6ee22-151">**Примечание.** Для возврата события может потребоваться несколько минут.</span><span class="sxs-lookup"><span data-stu-id="6ee22-151">**Note:** It may take a few minutes for the event to be returned.</span></span>

## <a name="step-3-create-a-conditional-access-policy"></a><span data-ttu-id="6ee22-152">Шаг 3. Создание политики условного доступа</span><span class="sxs-lookup"><span data-stu-id="6ee22-152">Step 3: Create a conditional access policy</span></span>

<span data-ttu-id="6ee22-153">Вы можете использовать политики условного доступа в организации, чтобы позволить пользователям самостоятельно устранять угрозы при обнаружении риска.</span><span class="sxs-lookup"><span data-stu-id="6ee22-153">You can leverage conditional access policies in your organization to allow users to self-remediate when risk is detected.</span></span> <span data-ttu-id="6ee22-154">Самостоятельное исправление позволяет пользователям разблокировать себя для безопасного доступа к своим ресурсам после выполнения запроса политики.</span><span class="sxs-lookup"><span data-stu-id="6ee22-154">Self-remediation enables your users to unblock themselves to access their resources securely after completing the policy prompt.</span></span> <span data-ttu-id="6ee22-155">На этом этапе создается политика условного доступа, которая требует, чтобы пользователь вошел с помощью MFA, если обнаружен средний или высокий риск.</span><span class="sxs-lookup"><span data-stu-id="6ee22-155">In this step, you create a conditional access policy that requires the user to sign in using MFA if a medium or high risk detection occurs.</span></span>

### <a name="set-up-multi-factor-authentication"></a><span data-ttu-id="6ee22-156">Настройка многофакторной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6ee22-156">Set up multi-factor authentication</span></span>

<span data-ttu-id="6ee22-157">При настройке учетной записи для MFA можно выбрать один из нескольких способов проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ee22-157">When setting up an account for MFA, you can choose from several methods for authenticating the user.</span></span> <span data-ttu-id="6ee22-158">Выберите лучший способ для вашей ситуации, чтобы завершить это руководство.</span><span class="sxs-lookup"><span data-stu-id="6ee22-158">Choose the best method for your situation to complete this tutorial.</span></span> 

1. <span data-ttu-id="6ee22-159">Во sign in to the [keep your account secure](https://aka.ms/MFASetup) site using the **MyTestUser1** account.</span><span class="sxs-lookup"><span data-stu-id="6ee22-159">Sign in the to the [keep your account secure](https://aka.ms/MFASetup) site using the **MyTestUser1** account.</span></span>
2. <span data-ttu-id="6ee22-160">Выполните процедуру настройки MFA, используя соответствующий метод для вашей ситуации, например, отправив на телефон текстовое сообщение.</span><span class="sxs-lookup"><span data-stu-id="6ee22-160">Complete the MFA setup procedure using the appropriate method for your situation, such as having a text message sent to your phone.</span></span>

### <a name="create-the-conditional-access-policy"></a><span data-ttu-id="6ee22-161">Создание политики условного доступа</span><span class="sxs-lookup"><span data-stu-id="6ee22-161">Create the conditional access policy</span></span>

<span data-ttu-id="6ee22-162">Политика условного доступа позволяет устанавливать условия политики для определения уровней риска для входов.</span><span class="sxs-lookup"><span data-stu-id="6ee22-162">The conditional access policy provides the ability to set the conditions of the policy to identify sign-in risk levels.</span></span> <span data-ttu-id="6ee22-163">Уровни риска: `low` `medium` , , `high` `none` .</span><span class="sxs-lookup"><span data-stu-id="6ee22-163">Risk levels can be `low`, `medium`, `high`, `none`.</span></span> <span data-ttu-id="6ee22-164">В ответе, возвращенном из списка обнаружений рисков для **MyTestUser1,** мы видим, что уровень риска составляет `medium` .</span><span class="sxs-lookup"><span data-stu-id="6ee22-164">In the response that was returned from listing the risk detections for **MyTestUser1**, we can see that the risk level is `medium`.</span></span> <span data-ttu-id="6ee22-165">В этом примере показано, как требовать MFA для **MyTestUser1,** который был определен как рискованный пользователь.</span><span class="sxs-lookup"><span data-stu-id="6ee22-165">This example shows how to require MFA for **MyTestUser1** who was identified as a risky user.</span></span>

#### <a name="request"></a><span data-ttu-id="6ee22-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee22-166">Request</span></span> 

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies 
Content-type: application/json
 
{ 
  "displayName": "Policy for risky sign-in", 
  "state": "enabled", 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "applications": { 
      "includeApplications": ["All"]
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ] 
  } 
} 
```

#### <a name="response"></a><span data-ttu-id="6ee22-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee22-167">Response</span></span> 

```
{ 
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity", 
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8", 
  "displayName": "Policy for risky sign-in", 
  "createdDateTime": "2020-11-03T20:56:38.6210843Z", 
  "modifiedDateTime": null, 
  "state": "enabled", 
  "sessionControls": null, 
  "conditions": { 
    "signInRiskLevels": [ 
      "high", 
      "medium" 
    ], 
    "clientAppTypes": [  
      "all"  
    ], 
    "platforms": null, 
    "locations": null, 
    "applications": { 
      "includeApplications": [ 
        "All" 
      ], 
      "excludeApplications": [], 
      "includeUserActions": [] 
    }, 
    "users": { 
      "includeUsers": [ 
        "4628e7df-dff3-407c-a08f-75f08c0806dc" 
      ], 
      "excludeUsers": [], 
      "includeGroups": [], 
      "excludeGroups": [], 
      "includeRoles": [], 
      "excludeRoles": [] 
    } 
  }, 
  "grantControls": { 
    "operator": "OR", 
    "builtInControls": [ 
      "mfa" 
    ], 
    "customAuthenticationFactors": [], 
    "termsOfUse": [] 
  } 
} 
```

<span data-ttu-id="6ee22-168">После применения этой политики условного доступа учетная запись **MyTestUser1** теперь необходима для использования MFA при входе, так как уровень риска для входов средний или   высокий.</span><span class="sxs-lookup"><span data-stu-id="6ee22-168">With this conditional access policy in place, the **MyTestUser1** account is now required to use MFA when signing in because the sign-in risk level is medium or high.</span></span> 

### <a name="sign-in-and-complete-multi-factor-authentication"></a><span data-ttu-id="6ee22-169">Вход и завершение многофакторной проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6ee22-169">Sign in and complete multi-factor authentication</span></span> 

<span data-ttu-id="6ee22-170">При входе в анонимный браузер обнаруживается риск, но он устраняется с помощью MFA.</span><span class="sxs-lookup"><span data-stu-id="6ee22-170">By signing in to the anonymous browser, a risk is detected, but it is remediated by completing MFA.</span></span> 

1. <span data-ttu-id="6ee22-171">Откройте браузер и введите  `portal.azure.com`   адрес сайта.</span><span class="sxs-lookup"><span data-stu-id="6ee22-171">Open the browser and enter `portal.azure.com` for the site address.</span></span> 
2. <span data-ttu-id="6ee22-172">Во sign in to the portal using the credentials for the **MyTestUser1**   account and complete the MFA process.</span><span class="sxs-lookup"><span data-stu-id="6ee22-172">Sign in to the portal using the credentials for the **MyTestUser1** account and complete the MFA process.</span></span> 

### <a name="list-risk-detections"></a><span data-ttu-id="6ee22-173">Список обнаружений рисков</span><span class="sxs-lookup"><span data-stu-id="6ee22-173">List risk detections</span></span>

<span data-ttu-id="6ee22-174">Так как MFA завершен.</span><span class="sxs-lookup"><span data-stu-id="6ee22-174">Because MFA was completed.</span></span> <span data-ttu-id="6ee22-175">Теперь при составлении списка обнаружений рисков **событие riskState** показывается как `remediated` .</span><span class="sxs-lookup"><span data-stu-id="6ee22-175">Now, when you list risk detections the **riskState** shows the event as `remediated`.</span></span>

#### <a name="request"></a><span data-ttu-id="6ee22-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee22-176">Request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskDetections?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a><span data-ttu-id="6ee22-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee22-177">Response</span></span>

```http
{
  "id": "ba9d45f16d8f87f6ae974efda7336b2120962a398cb362dfd9e5bdc8e9d149d0",
  "requestId": "156c01fb-31cf-4a10-b9a9-beee93e6a400",
  "correlationId": "a8aaac45-fe22-46df-babf-10a8dba85d62",
  "riskType": "anonymizedIPAddress",
  "riskEventType": "anonymizedIPAddress",
  "riskState": "remediated",
  "riskLevel": "medium",
  "riskDetail": "userPassedMFADrivenByRiskBasedPolicy",
  "source": "IdentityProtection",
  "detectionTimingType": "realtime",
  "activity": "signin",
  "tokenIssuerType": "AzureAD",
  "ipAddress": "185.220.101.213",
  "activityDateTime": "2020-11-12T23:45:22.4092789Z",
  "detectedDateTime": "2020-11-12T23:45:22.4092789Z",
  "lastUpdatedDateTime": "2020-11-12T23:47:57.7831423Z",
  "userId": "4b608561-9258-44ba-8cdb-3286dcbf0e3b",
  "userDisplayName": "MyTestUser1",
  "userPrincipalName": "MyTestUser1@contoso.com",
    "additionalInfo": "[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; rv:78.0) Gecko/20100101 Firefox/78.0\"}]",
  "location": {
    "city": "Schoenwalde-Glien",
    "state": "Brandenburg",
    "countryOrRegion": "DE",
    "geoCoordinates": {
      "latitude": 52.61983,
      "longitude": 13.12743
    }
  }
}
```

## <a name="step-4-optional-block-the-user-from-signing-in"></a><span data-ttu-id="6ee22-178">Шаг 4 (необязательно) Блокировка пользователя при входе</span><span class="sxs-lookup"><span data-stu-id="6ee22-178">Step 4 (Optional) Block the user from signing in</span></span>

<span data-ttu-id="6ee22-179">Вместо того чтобы предоставлять пользователю возможность самостоятельного устранения, можно заблокировать вход пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ee22-179">Instead of providing the opportunity for the user to self-remediate, you can block the user from signing in.</span></span> <span data-ttu-id="6ee22-180">На этом этапе создается новая политика условного доступа, которая блокирует вход пользователя в случае обнаружения среднего или высокого риска.</span><span class="sxs-lookup"><span data-stu-id="6ee22-180">In this step, you create a new conditional access policy that blocks the user from signing in if a medium or high risk detection occurs.</span></span> <span data-ttu-id="6ee22-181">Разница в политиках заключается в том, **что для builtInControls** установлено значение `block` .</span><span class="sxs-lookup"><span data-stu-id="6ee22-181">The difference in policies is that the **builtInControls** is set to `block`.</span></span>

### <a name="request"></a><span data-ttu-id="6ee22-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee22-182">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies
Content-type: application/json

{
  "displayName": "Policy for risky sign-in block access",
  "state": "enabled",
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "applications": {
      "includeApplications": ["All"]
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ]
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="6ee22-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee22-183">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/conditionalAccess/policies/$entity",
  "id": "9ad78153-b1f8-4714-adc1-1445727678a8",
  "displayName": "Policy for risky sign-in block access",
  "createdDateTime": "2020-11-03T20:56:38.6210843Z",
  "modifiedDateTime": null,
  "state": "enabled",
  "sessionControls": null,
  "conditions": {
    "signInRiskLevels": [
      "high",
      "medium"
    ],
    "clientAppTypes": [ 
      "all" 
    ],
    "platforms": null,
    "locations": null,
    "applications": {
      "includeApplications": [
        "All"
      ],
      "excludeApplications": [],
      "includeUserActions": []
    },
    "users": {
      "includeUsers": [
        "4628e7df-dff3-407c-a08f-75f08c0806dc"
      ],
      "excludeUsers": [],
      "includeGroups": [],
      "excludeGroups": [],
      "includeRoles": [],
      "excludeRoles": []
    }
  },
  "grantControls": {
    "operator": "OR",
    "builtInControls": [
      "block"
    ],
    "customAuthenticationFactors": [],
    "termsOfUse": []
  }
}
```

<span data-ttu-id="6ee22-184">После данной политики условного доступа учетная запись **MyTestUser1** не может войти в нее, так как уровень риска для входов `medium` составляет или `high` .</span><span class="sxs-lookup"><span data-stu-id="6ee22-184">With this conditional access policy in place, the **MyTestUser1** account is now blocked from signing in because the sign-in risk level is `medium` or `high`.</span></span>

![Заблокированный вход](./images/tutorial-riskdetection-api/conditionalaccess-policy.png)

## <a name="step-5-dismiss-risky-users"></a><span data-ttu-id="6ee22-186">Шаг 5. Отклонение рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="6ee22-186">Step 5: Dismiss risky users</span></span>

<span data-ttu-id="6ee22-187">Если вы считаете, что пользователь не находится под угрозой и не хотите применять политику условного доступа, можно вручную отклонять этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6ee22-187">If you believe the user is not at risk, and you don’t want to enforce a conditional access policy, you can manually dismiss the risky user.</span></span>

### <a name="dismiss-the-risky-user"></a><span data-ttu-id="6ee22-188">Отклонение рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="6ee22-188">Dismiss the risky user</span></span>

#### <a name="request"></a><span data-ttu-id="6ee22-189">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee22-189">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "4628e7df-dff3-407c-a08f-75f08c0806dc"
  ]
}
```

#### <a name="response"></a><span data-ttu-id="6ee22-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee22-190">Response</span></span>

```http
HTTP/1.1 204 No Content
```        

### <a name="list-risky-users"></a><span data-ttu-id="6ee22-191">Список рискованных пользователей</span><span class="sxs-lookup"><span data-stu-id="6ee22-191">List risky users</span></span>

<span data-ttu-id="6ee22-192">После того как пользователь с риском будет отклонен, вы увидите в ответе список рискованных пользователей, для учетной записи **пользователя MyTestUser1** теперь есть уровень риска и уровень риска `none` . `dismissed`</span><span class="sxs-lookup"><span data-stu-id="6ee22-192">After dismissing the risk user, you can see in the response when listing risky users that the **MyTestUser1** user account now has a risk level of `none` and a riskState of `dismissed`.</span></span>

#### <a name="request"></a><span data-ttu-id="6ee22-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee22-193">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers?$filter=userDisplayName eq 'MyTestUser1'
```

#### <a name="response"></a><span data-ttu-id="6ee22-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee22-194">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers",
  "value": [
    {
      "id": "4628e7df-dff3-407c-a08f-75f08c0806dc",
      "isDeleted": false,
      "isProcessing": false,
      "riskLevel": "none",
      "riskState": "dismissed",
      "riskDetail": "adminDismissedAllRiskForUser",
      "riskLastUpdatedDateTime": "2020-11-03T21:48:53.4298425Z",
      "userDisplayName": "MyTestUser1",
      "userPrincipalName": "MyTestUser1@contoso.com"
    }
  ]
}
```

## <a name="step-6-clean-up-resources"></a><span data-ttu-id="6ee22-195">Шаг 6. Очистка ресурсов</span><span class="sxs-lookup"><span data-stu-id="6ee22-195">Step 6: Clean up resources</span></span>

<span data-ttu-id="6ee22-196">На этом этапе удаляются созданные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="6ee22-196">In this step, you remove the resources that you created.</span></span>

### <a name="delete-the-user-account"></a><span data-ttu-id="6ee22-197">Удаление учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="6ee22-197">Delete the user account</span></span>

<span data-ttu-id="6ee22-198">Удалите **учетную запись пользователя MyTestUser1.**</span><span class="sxs-lookup"><span data-stu-id="6ee22-198">Delete the **MyTestUser1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="6ee22-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee22-199">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/4628e7df-dff3-407c-a08f-75f08c0806dc
```

#### <a name="response"></a><span data-ttu-id="6ee22-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee22-200">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-conditional-access-policy"></a><span data-ttu-id="6ee22-201">Удаление политики условного доступа</span><span class="sxs-lookup"><span data-stu-id="6ee22-201">Delete the conditional access policy</span></span>

<span data-ttu-id="6ee22-202">Удалите созданную политику условного доступа.</span><span class="sxs-lookup"><span data-stu-id="6ee22-202">Delete the conditional access policy that you created.</span></span>

#### <a name="request"></a><span data-ttu-id="6ee22-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ee22-203">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/groups/9ad78153-b1f8-4714-adc1-1445727678a8
```

#### <a name="response"></a><span data-ttu-id="6ee22-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ee22-204">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="6ee22-205">См. также</span><span class="sxs-lookup"><span data-stu-id="6ee22-205">See also</span></span>

<span data-ttu-id="6ee22-206">В этом руководстве вы использовали множество API для выполнения задач.</span><span class="sxs-lookup"><span data-stu-id="6ee22-206">In this tutorial, you used many APIs to accomplish tasks.</span></span> <span data-ttu-id="6ee22-207">Изучите справочник по API для этих API, чтобы узнать больше о том, что могут делать API.</span><span class="sxs-lookup"><span data-stu-id="6ee22-207">Explore the API reference for these APIs to learn more about what the APIs can do.</span></span>

- [<span data-ttu-id="6ee22-208">Что такое защита идентификации?</span><span class="sxs-lookup"><span data-stu-id="6ee22-208">What is Identity Protection?</span></span>](/azure/active-directory/identity-protection/overview-identity-protection)
- [<span data-ttu-id="6ee22-209">Что такое условный доступ?</span><span class="sxs-lookup"><span data-stu-id="6ee22-209">What is Conditional Access?</span></span>](/azure/active-directory/conditional-access/overview)
- [<span data-ttu-id="6ee22-210">Как это работает: многофакторная проверка подлинности Azure</span><span class="sxs-lookup"><span data-stu-id="6ee22-210">How it works: Azure Multi-Factor Authentication</span></span>](/azure/active-directory/authentication/concept-mfa-howitworks)
- [<span data-ttu-id="6ee22-211">conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="6ee22-211">conditionalAccessPolicy</span></span>](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-1.0)
- [<span data-ttu-id="6ee22-212">riskDetection</span><span class="sxs-lookup"><span data-stu-id="6ee22-212">riskDetection</span></span>](/graph/api/resources/riskdetection?view=graph-rest-1.0)
- [<span data-ttu-id="6ee22-213">riskyUser</span><span class="sxs-lookup"><span data-stu-id="6ee22-213">riskyUser</span></span>](/graph/api/resources/riskyuser?view=graph-rest-1.0)
- [<span data-ttu-id="6ee22-214">user</span><span class="sxs-lookup"><span data-stu-id="6ee22-214">user</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
