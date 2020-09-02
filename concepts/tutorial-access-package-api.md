---
title: 'Руководство: создание пакета Access с помощью API Microsoft Graph'
description: Узнайте, как создать пакет Access и запросить доступ к нему с помощью API Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afb5e048a0075ccb391c4edd5f74ced8ecd7755c
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330479"
---
# <a name="tutorial-create-an-access-package-using-microsoft-graph-apis"></a><span data-ttu-id="11bfa-103">Руководство: создание пакета Access с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="11bfa-103">Tutorial: Create an access package using Microsoft Graph APIs</span></span>

<span data-ttu-id="11bfa-104">Управление доступом ко всем ресурсам, необходимым для сотрудников, таких как группы, приложения и сайты, является важной функцией для организаций.</span><span class="sxs-lookup"><span data-stu-id="11bfa-104">Managing access to all the resources that employees need, such as groups, applications, and sites, is an important function for organizations.</span></span> <span data-ttu-id="11bfa-105">Вы хотите предоставить сотрудникам необходимый уровень доступа, который им необходим для продуктивности, и удалить доступ, когда он больше не нужен.</span><span class="sxs-lookup"><span data-stu-id="11bfa-105">You want to grant employees the right level of access they need to be productive and remove their access when it is no longer needed.</span></span> <span data-ttu-id="11bfa-106">[Управление обслуживанием Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-overview) с помощью API Microsoft Graph позволяет управлять этим типом доступа.</span><span class="sxs-lookup"><span data-stu-id="11bfa-106">[Azure Active Directory (Azure AD) entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-overview) using Microsoft Graph APIs enables you to manage this type of access.</span></span>

<span data-ttu-id="11bfa-107">В этом руководстве вы запросили разработку кода для создания пакета ресурсов для маркетинговой кампании, с которой внутренние пользователи могут самостоятельно выполнить запрос.</span><span class="sxs-lookup"><span data-stu-id="11bfa-107">In this tutorial, you've been asked to develop code to create a package of resources for a marketing campaign that internal users can self-service request.</span></span> <span data-ttu-id="11bfa-108">Запросы не требуют утверждения и срок действия доступа пользователя истечет через 30 дней.</span><span class="sxs-lookup"><span data-stu-id="11bfa-108">Requests do not require approval and user's access expires after 30 days.</span></span> <span data-ttu-id="11bfa-109">В этом руководстве ресурсы маркетинговой кампании — это всего лишь членство в одной группе, но может быть коллекцией групп, приложений или сайтов SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="11bfa-109">For this tutorial, the marketing campaign resources are just membership in a single group, but it could be a collection of groups, applications, or SharePoint Online sites.</span></span>

><span data-ttu-id="11bfa-110">**Примечание:** Объекты ответа, показанные в этом руководстве, могут быть сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="11bfa-110">**Note:** The response objects shown in this tutorial might be shortened for readability.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="11bfa-111">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="11bfa-111">Prerequisites</span></span>

<span data-ttu-id="11bfa-112">Для успешного выполнения этого руководства убедитесь, что у вас есть необходимые компоненты:</span><span class="sxs-lookup"><span data-stu-id="11bfa-112">To successfully complete this tutorial, make sure that you have the required prerequisites:</span></span>
- <span data-ttu-id="11bfa-113">Для управления обслуживанием Azure AD требуются определенные лицензии.</span><span class="sxs-lookup"><span data-stu-id="11bfa-113">Azure AD entitlement management requires specific licenses.</span></span> <span data-ttu-id="11bfa-114">Более подробную информацию можно узнать в статье [требования к лицензии](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-overview#license-requirements).</span><span class="sxs-lookup"><span data-stu-id="11bfa-114">For more information, see [License requirements](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-overview#license-requirements).</span></span> <span data-ttu-id="11bfa-115">В клиенте требуются следующие лицензии:</span><span class="sxs-lookup"><span data-stu-id="11bfa-115">The following licenses are required in your tenant:</span></span>
    - <span data-ttu-id="11bfa-116">Azure AD Premium P2</span><span class="sxs-lookup"><span data-stu-id="11bfa-116">Azure AD Premium P2</span></span>
    - <span data-ttu-id="11bfa-117">Лицензия Enterprise Mobility + Security (EMS)</span><span class="sxs-lookup"><span data-stu-id="11bfa-117">Enterprise Mobility + Security (EMS) E5 license</span></span>
- <span data-ttu-id="11bfa-118">В этом руководстве предполагается, что используется обозреватель Microsoft Graph, но вы можете использовать POST или создать собственное клиентское приложение для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="11bfa-118">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="11bfa-119">Чтобы вызвать API Microsoft Graph в этом руководстве, необходимо использовать учетную запись с ролью глобального администратора и соответствующими разрешениями.</span><span class="sxs-lookup"><span data-stu-id="11bfa-119">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="11bfa-120">В этом руководстве `User.ReadWrite.All` `Group.ReadWrite.All` `EntitlementManagement.ReadWrite.All` необходимы разрешения, и делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="11bfa-120">For this tutorial, the `User.ReadWrite.All`, `Group.ReadWrite.All`, and `EntitlementManagement.ReadWrite.All` delegated permissions are needed.</span></span> <span data-ttu-id="11bfa-121">Выполните следующие действия, чтобы задать разрешения в Microsoft Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="11bfa-121">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>
    1. <span data-ttu-id="11bfa-122">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="11bfa-122">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="11bfa-123">Выберите **Вход в систему с** помощью учетной записи Майкрософт и войдите с помощью учетной записи глобального администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="11bfa-123">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="11bfa-124">После успешного входа вы сможете просмотреть сведения об учетной записи пользователя в области слева.</span><span class="sxs-lookup"><span data-stu-id="11bfa-124">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="11bfa-125">Нажмите значок Параметры справа от сведений учетной записи пользователя, а затем выберите **пункт Выбор разрешений**.</span><span class="sxs-lookup"><span data-stu-id="11bfa-125">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![Выберите разрешения Microsoft Graph.](./images/tutorial-access-package-api/set-permissions.png)
        
    4. <span data-ttu-id="11bfa-127">Прокрутите список разрешений для `Group` разрешений, разверните **группу (2)**, выберите разрешение **Group. ReadWrite. ALL** .</span><span class="sxs-lookup"><span data-stu-id="11bfa-127">Scroll through the list of permissions to the `Group` permissions, expand **Group (2)**, select the **Group.ReadWrite.All** permission.</span></span>
    5. <span data-ttu-id="11bfa-128">Прокрутите список разрешений на все разрешения `User` , разверните **пользователь (8)**, нажмите клавишу **CTRL** и выберите разрешение **User. ReadWrite. ALL** .</span><span class="sxs-lookup"><span data-stu-id="11bfa-128">Scroll further down the list of permissions to the `User` permissions, expand **User (8)**, press the **Ctrl** key and select the **User.ReadWrite.All** permission.</span></span>

        ![Выполните поиск разрешений пользователя.](./images/tutorial-access-package-api/set-user-permission.png)
    
    6. <span data-ttu-id="11bfa-130">Нажмите кнопку **принять** , чтобы принять разрешение разрешений.</span><span class="sxs-lookup"><span data-stu-id="11bfa-130">Select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="11bfa-131">Вы не обязаны согласие от имени вашей организации для этих разрешений.</span><span class="sxs-lookup"><span data-stu-id="11bfa-131">You do not need to consent on behalf of your organization for these permissions.</span></span>
    7. <span data-ttu-id="11bfa-132">Выполните поиск `EntitlementManagement` разрешений, разверните **ентитлементманажемент (2)**, выберите разрешения правого доступа **. ReadWrite. ALL** , а затем выберите **согласие**.</span><span class="sxs-lookup"><span data-stu-id="11bfa-132">Search for the `EntitlementManagement` permissions, expand **EntitlementManagement (2)**, select the **Entitlement.ReadWrite.All** permission, and then select **Consent**.</span></span> <span data-ttu-id="11bfa-133">Так как для этого разрешения требуется согласие администратора и для учетной записи пользователя, созданной в этом руководстве, необходимо выбрать **согласие от имени вашей организации**.</span><span class="sxs-lookup"><span data-stu-id="11bfa-133">Because this permission requires admin consent and is needed by a user account that you create in this tutorial, you must select **Consent on behalf of your organization**.</span></span>

        ![Согласие для Организации](./images/tutorial-access-package-api/consent-for-organization.png)

## <a name="step-1-create-a-user-account-and-a-group"></a><span data-ttu-id="11bfa-135">Шаг 1: создание учетной записи пользователя и группы</span><span class="sxs-lookup"><span data-stu-id="11bfa-135">Step 1: Create a user account and a group</span></span>

<span data-ttu-id="11bfa-136">На этом шаге создается группа с именем " **маркетинговые ресурсы** " в каталоге, который является целевым ресурсом для управления обслуживанием.</span><span class="sxs-lookup"><span data-stu-id="11bfa-136">In this step, you create a group named **Marketing resources** in the directory that is the target resource for entitlement management.</span></span> <span data-ttu-id="11bfa-137">Вы также создаете учетную запись пользователя, которая настроена как внутренний запрашивающий.</span><span class="sxs-lookup"><span data-stu-id="11bfa-137">You also create a user account that is set up as an internal requestor.</span></span>

### <a name="create-a-user-account"></a><span data-ttu-id="11bfa-138">Создание учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="11bfa-138">Create a user account</span></span>

<span data-ttu-id="11bfa-139">В этом руководстве показано, как создать учетную запись пользователя, которая будет использоваться для запроса доступа к ресурсам в пакете Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-139">For this tutorial, you create a user account that is used to request access to the resources in the access package.</span></span> <span data-ttu-id="11bfa-140">При совершении этих вызовов замените `contoso.onmicrosoft.com` доменное имя клиента.</span><span class="sxs-lookup"><span data-stu-id="11bfa-140">When you make these calls, change `contoso.onmicrosoft.com` to the domain name of your tenant.</span></span> <span data-ttu-id="11bfa-141">Сведения о клиенте можно найти на странице "Обзор Azure Active Directory".</span><span class="sxs-lookup"><span data-stu-id="11bfa-141">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="11bfa-142">Запишите значение свойства **ID** , которое возвращается в дальнейшем для использования в руководстве.</span><span class="sxs-lookup"><span data-stu-id="11bfa-142">Record the value of the **id** property that is returned to be used later in the tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-143">Request</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"Requestor1",
  "mailNickname":"Requestor1",
  "userPrincipalName":"Requestor1@contoso.onmicrosoft.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a><span data-ttu-id="11bfa-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-144">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
  "deletedDateTime": null,
  "accountEnabled": true,
  "ageGroup": null,
  "businessPhones": [],
  "city": null,
  "createdDateTime": null,
  "creationType": null,
  "companyName": null,
  "consentProvidedForMinor": null,
  "country": null,
  "department": null,
  "displayName": "Requestor1",
  "employeeId": null,
  "faxNumber": null,
  "givenName": null,
  "imAddresses": [],
  "infoCatalogs": [],
  "isResourceAccount": null,
  "jobTitle": null,
  "legalAgeGroupClassification": null,
  "mail": null,
  "mailNickname": "Requestor1",
}
```

### <a name="create-a-group"></a><span data-ttu-id="11bfa-145">Создание группы</span><span class="sxs-lookup"><span data-stu-id="11bfa-145">Create a group</span></span>

<span data-ttu-id="11bfa-146">В этом руководстве описывается создание группы под названием " **маркетинговые ресурсы** ", которая является целевым ресурсом для управления обслуживанием.</span><span class="sxs-lookup"><span data-stu-id="11bfa-146">In this tutorial, you create a group named **Marketing resources** that is the target resource for entitlement management.</span></span> <span data-ttu-id="11bfa-147">Вы можете использовать существующую группу, если она уже есть.</span><span class="sxs-lookup"><span data-stu-id="11bfa-147">You can use an existing group if you already have one.</span></span> <span data-ttu-id="11bfa-148">Запишите значение свойства **ID** , которое возвращается для использования далее в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="11bfa-148">Record the value of the **id** property that is returned to use later in this tutorial.</span></span> 

#### <a name="request"></a><span data-ttu-id="11bfa-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-149">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json

{
  "description":"Marketing group",
  "displayName":"Marketing resources",
  "mailEnabled":false,
  "mailNickname":"markres",
  "securityEnabled":true
}
```

#### <a name="response"></a><span data-ttu-id="11bfa-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-150">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
  "id": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
  "deletedDateTime": null,
  "classification": null,
  "createdDateTime": "2020-06-24T16:47:37Z",
  "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
  "description": "Marketing group",
  "displayName": "Marketing resources",
  "expirationDateTime": null,
  "groupTypes": [],
  "infoCatalogs": [],
  "isAssignableToRole": null,
  "mail": null,
  "mailEnabled": false,
  "mailNickname": "markres"
}
```

## <a name="step-2-add-resources-to-a-catalog-and-create-an-access-package"></a><span data-ttu-id="11bfa-151">Шаг 2: Добавление ресурсов в каталог и создание пакета Access</span><span class="sxs-lookup"><span data-stu-id="11bfa-151">Step 2: Add resources to a catalog and create an access package</span></span>

<span data-ttu-id="11bfa-152">*Пакет Access* — это набор ресурсов, необходимых группе или проекту и управляемых политиками.</span><span class="sxs-lookup"><span data-stu-id="11bfa-152">An *access package* is a bundle of resources that a team or project needs and is governed with policies.</span></span> <span data-ttu-id="11bfa-153">Пакеты доступа определяются в контейнерах, которые называются каталогами.</span><span class="sxs-lookup"><span data-stu-id="11bfa-153">Access packages are defined in containers called catalogs.</span></span> <span data-ttu-id="11bfa-154">Каталоги могут ссылаться на ресурсы, такие как группы, приложения и сайты, которые используются в пакете Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-154">Catalogs can reference resources, such as groups, apps and sites, that are used in the access package.</span></span> <span data-ttu-id="11bfa-155">На этом этапе вы создадите пакет доступа к **маркетинговой кампании** в общем каталоге.</span><span class="sxs-lookup"><span data-stu-id="11bfa-155">In this step, you create a **Marketing Campaign** access package in the General catalog.</span></span> <span data-ttu-id="11bfa-156">Если у вас другой каталог, используйте его имя в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="11bfa-156">If you have a different catalog, use its name in the next section.</span></span>

### <a name="get-the-catalog-identifier"></a><span data-ttu-id="11bfa-157">Получение идентификатора каталога</span><span class="sxs-lookup"><span data-stu-id="11bfa-157">Get the catalog identifier</span></span>

<span data-ttu-id="11bfa-158">Чтобы добавить ресурсы в каталог, необходимо сначала получить его идентификатор.</span><span class="sxs-lookup"><span data-stu-id="11bfa-158">To add resources to the catalog, you must first get the identifier of it.</span></span> <span data-ttu-id="11bfa-159">Если вы используете общий каталог, выполните следующий запрос, чтобы получить идентификатор.</span><span class="sxs-lookup"><span data-stu-id="11bfa-159">If you are using the General catalog, run the following request to get its identifier.</span></span> <span data-ttu-id="11bfa-160">Если вы используете другой калалог, измените значение фильтра в запросе на имя каталога.</span><span class="sxs-lookup"><span data-stu-id="11bfa-160">If you are using a different calalog, change the filter value in the request to the name of your catalog.</span></span> <span data-ttu-id="11bfa-161">Запишите значение свойства **ID** , которое возвращается для использования далее в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="11bfa-161">Record the value of the **id** property that is returned to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-162">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs?$filter=(displayName eq 'General')
```

#### <a name="response"></a><span data-ttu-id="11bfa-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-163">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageCatalogs",
  "value": [ 
    {
      "id": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "displayName": "General",
      "description": "Built-in catalog.",
      "catalogType": "ServiceDefault",
      "catalogStatus": "Published",
      "isExternallyVisible": true,
      "createdBy": "Azure AD",
      "createdDateTime": "2020-05-30T10:58:05.363Z",
      "modifiedBy": "Azure AD",
      "modifiedDateTime": "2020-05-30T10:58:05.363Z"
    }
  ]
}
```

<span data-ttu-id="11bfa-164">Ответ должен содержать только каталог, имя которого указано в запросе.</span><span class="sxs-lookup"><span data-stu-id="11bfa-164">The response should only contain the catalog whose name you provided in the request.</span></span> <span data-ttu-id="11bfa-165">Если значения не возвращены, проверьте правильность имени каталога, прежде чем продолжить.</span><span class="sxs-lookup"><span data-stu-id="11bfa-165">If there are no values returned, check that the name of the catalog is correct before you proceed.</span></span>

### <a name="add-the-group-to-the-catalog"></a><span data-ttu-id="11bfa-166">Добавление группы в каталог</span><span class="sxs-lookup"><span data-stu-id="11bfa-166">Add the group to the catalog</span></span>

<span data-ttu-id="11bfa-167">Чтобы добавить группу, созданную для каталога, укажите следующие значения свойств:</span><span class="sxs-lookup"><span data-stu-id="11bfa-167">To add the group that you created to the catalog, provide the following property values:</span></span>
- <span data-ttu-id="11bfa-168">**каталогид** — **идентификатор** каталога, который вы используете</span><span class="sxs-lookup"><span data-stu-id="11bfa-168">**catalogId** - the **id** of the catalog that you are using</span></span>
- <span data-ttu-id="11bfa-169">**DisplayName** — имя группы.</span><span class="sxs-lookup"><span data-stu-id="11bfa-169">**displayName** - the name of the group</span></span>
- <span data-ttu-id="11bfa-170">**Description** — описание группы.</span><span class="sxs-lookup"><span data-stu-id="11bfa-170">**description** - the description of the group</span></span>
- <span data-ttu-id="11bfa-171">**оригинид** — **идентификатор** созданной группы.</span><span class="sxs-lookup"><span data-stu-id="11bfa-171">**originId** - the **id** of the group that you created</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-172">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
    "displayName": "Marketing resources",
    "description": "Marketing group",
    "resourceType": "AadGroup",
    "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "originSystem": "AadGroup"
  }
}
```

#### <a name="response"></a><span data-ttu-id="11bfa-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-173">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageResourceRequests/$entity",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "executeImmediately": false,
  "id": "44e521e0-fb6b-4d5e-a282-e7e68dc59493",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": ""
}
```

### <a name="get-catalog-resources"></a><span data-ttu-id="11bfa-174">Получение ресурсов каталога</span><span class="sxs-lookup"><span data-stu-id="11bfa-174">Get catalog resources</span></span>

<span data-ttu-id="11bfa-175">Дальнейшие действия, описанные в этом руководстве, потребуют **идентификатор** , назначенный ресурсу группы в каталоге.</span><span class="sxs-lookup"><span data-stu-id="11bfa-175">In later steps in this tutorial, you need the **id** that was assigned to the group resource in the catalog.</span></span> <span data-ttu-id="11bfa-176">Этот идентификатор, который представляет группу как ресурс в каталоге, отличается от идентификатора самой группы в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="11bfa-176">This identifier, which represents the group as a resource in the catalog, is different than the identifier of the group itself in Microsoft Graph.</span></span> <span data-ttu-id="11bfa-177">Это связано с тем, что каталог может иметь ресурсы, которые не представлены в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="11bfa-177">This is because a catalog can have resources which aren't represented in Microsoft Graph.</span></span>

<span data-ttu-id="11bfa-178">В запросе укажите **идентификатор** каталога, который вы используете.</span><span class="sxs-lookup"><span data-stu-id="11bfa-178">In the request, provide the **id** of the catalog that you are using.</span></span> <span data-ttu-id="11bfa-179">Запишите значение свойства **ID** для ресурса каталога группы.</span><span class="sxs-lookup"><span data-stu-id="11bfa-179">Record the value of the **id** property for the group catalog resource.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-180">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResources?$filter=(displayName eq 'Marketing resources')
```

#### <a name="response"></a><span data-ttu-id="11bfa-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-181">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageResources",
  "value": [
    {
      "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
      "displayName": "Marketing resources",
      "description": "Marketing group",
      "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "resourceType": "Security Group",
      "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "originSystem": "AadGroup",
      "isPendingOnboarding": false,
      "addedBy": "admin@contoso.onmicrosoft.com",
      "addedOn": "2020-08-21T19:27:29.967Z"
    }
  ]
}
```

### <a name="get-resources-roles"></a><span data-ttu-id="11bfa-182">Получение ролей ресурсов</span><span class="sxs-lookup"><span data-stu-id="11bfa-182">Get resources roles</span></span>

<span data-ttu-id="11bfa-183">Пакет Access назначает пользователей ролям ресурса.</span><span class="sxs-lookup"><span data-stu-id="11bfa-183">The access package assigns users to the roles of a resource.</span></span> <span data-ttu-id="11bfa-184">Типичной ролью группы является роль участника.</span><span class="sxs-lookup"><span data-stu-id="11bfa-184">The typical role of a group is the member role.</span></span> <span data-ttu-id="11bfa-185">Другие ресурсы, например сайты и приложения SharePoint Online, могут иметь множество ролей.</span><span class="sxs-lookup"><span data-stu-id="11bfa-185">Other resources, such as SharePoint Online sites and applications, might have many roles.</span></span> <span data-ttu-id="11bfa-186">Типичной ролью группы, используемой в пакете Access, является роль участника.</span><span class="sxs-lookup"><span data-stu-id="11bfa-186">The typical role of a group used in an access package is the member role.</span></span> <span data-ttu-id="11bfa-187">Роль участника потребуется при добавлении роли ресурса в пакет Access позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="11bfa-187">You'll need the member role when you add a resource role to the access package later in this tutorial.</span></span> 

<span data-ttu-id="11bfa-188">В запросе используйте **идентификатор** каталога и **идентификатор** ресурса Group в каталоге, который вы записали, чтобы получить **оригинид** роли ресурса члена.</span><span class="sxs-lookup"><span data-stu-id="11bfa-188">In the request, use the **id** of the catalog and the **id** of the group resource in the catalog that you recorded to get the **originId** of the Member resource role.</span></span> <span data-ttu-id="11bfa-189">Запишите значение свойства **оригинид** , которое будет использоваться далее в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="11bfa-189">Record the value of the **originId** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-190">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%274a1e21c5-8a76-4578-acb1-641160e076e8%27+and+displayName+eq+%27Member%27)&$expand=accessPackageResource
```

#### <a name="response"></a><span data-ttu-id="11bfa-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-191">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('ede67938-cda7-4127-a9ca-7c7bf86a19b7')/accessPackageResourceRoles(accessPackageResource())",
  "value": [
    {
      "id": "00000000-0000-0000-0000-000000000000",
      "displayName": "Member",
      "description": null,
      "originSystem": "AadGroup",
      "originId": "Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
      "accessPackageResource@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/$entity",
      "accessPackageResource": {
        "id": "4a1e21c5-8a76-4578-acb1-641160e076e8",
        "displayName": "Marketing resources",
        "description": "Marketing group",
        "url": "https://account.activedirectory.windowsazure.com/r?tenantId=d3030981-8fb9-4919-9980-5580caeddd75#/manageMembership?objectType=Group&objectId=e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "resourceType": "Security Group",
        "originId": "e93e24d1-2b65-4a6c-a1dd-654a12225487",
        "originSystem": "AadGroup",
        "isPendingOnboarding": false,
        "addedBy": "admin@contoso.onmicrosoft.com",
        "addedOn": "2020-06-26T17:13:23.723Z",
        "accessPackageResourceScopes@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackageCatalogs('cec5d6ab-c75d-47c0-9c1c-92e89f66e384')/accessPackageResourceRoles('00000000-0000-0000-0000-000000000000')/accessPackageResource/accessPackageResourceScopes",
        "accessPackageResourceScopes": []
      }
    }
  ]
}
```

<span data-ttu-id="11bfa-192">В случае успешного выполнения возвращается одно значение, представляющее роль участника для этой группы.</span><span class="sxs-lookup"><span data-stu-id="11bfa-192">If successful, a single value is returned, which represents the Member role of that group.</span></span> <span data-ttu-id="11bfa-193">Если роли не возвращаются, проверьте значения **ID** каталога и ресурса пакета Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-193">If no roles are returned, check the **id** values of the catalog and the access package resource.</span></span>

### <a name="create-the-access-package"></a><span data-ttu-id="11bfa-194">Создание пакета Access</span><span class="sxs-lookup"><span data-stu-id="11bfa-194">Create the access package</span></span>

<span data-ttu-id="11bfa-195">На этом шаге у вас есть каталог с ресурсом Group, и вы знаете, что вы используете роль ресурса "член группы" в пакете Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-195">At this point, you have a catalog with a group resource, and you know that you'll use the resource role of group member in the access package.</span></span> <span data-ttu-id="11bfa-196">Следующий шаг — создание пакета Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-196">The next step is to create the access package.</span></span> <span data-ttu-id="11bfa-197">После получения пакета Access можно добавить в него роль ресурса и создать политику, определяющую, как пользователи могут запрашивать доступ к этой роли ресурса.</span><span class="sxs-lookup"><span data-stu-id="11bfa-197">After you have the access package, you can add the resource role to it, and create a policy for how users can request access to that resource role.</span></span> <span data-ttu-id="11bfa-198">Для создания пакета доступа используется **идентификатор** каталога, записанный ранее.</span><span class="sxs-lookup"><span data-stu-id="11bfa-198">You use the **id** of the catalog that you recorded earlier to create the access package.</span></span> <span data-ttu-id="11bfa-199">Запишите **идентификатор** пакета доступа, который будет использоваться далее в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="11bfa-199">Record the **id** of the access package to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-200">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign"
}
```

#### <a name="response"></a><span data-ttu-id="11bfa-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-201">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages/$entity",
  "id": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign",
  "isHidden": false,
  "isRoleScopesVisible": false,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:45:33.2042281Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:45:33.2042281Z"
}
```

### <a name="add-a-resource-role-to-the-access-package"></a><span data-ttu-id="11bfa-202">Добавление роли ресурса в пакет Access</span><span class="sxs-lookup"><span data-stu-id="11bfa-202">Add a resource role to the access package</span></span>

<span data-ttu-id="11bfa-203">Добавьте роль участника для ресурса Group в пакет Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-203">Add the Member role of the group resource to the access package.</span></span> <span data-ttu-id="11bfa-204">В запросе укажите **идентификатор** пакета Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-204">In the request, provide the **id** of the access package.</span></span> <span data-ttu-id="11bfa-205">В тексте запроса укажите **идентификатор** ресурса каталога группы для акцесспаккажересаурце и предоставьте **оригинид** роли члена, который вы ранее записали.</span><span class="sxs-lookup"><span data-stu-id="11bfa-205">In the request body provide the **id** of the group catalog resource for accessPackageResource, and provide the **originId** of the Member role that you previously recorded.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-206">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/88203d16-0e31-41d4-87b2-dd402f1435e9/accessPackageResourceRoleScopes
Content-type: application/json

{
  "accessPackageResourceRole": {
    "originId":"Member_e93e24d1-2b65-4a6c-a1dd-654a12225487",
    "displayName":"Member",
    "originSystem":"AadGroup",
    "accessPackageResource": {
      "id":"4a1e21c5-8a76-4578-acb1-641160e076e8","resourceType":"Security Group",  
      "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
    }
  },
  "accessPackageResourceScope": {
    "originId":"e93e24d1-2b65-4a6c-a1dd-654a12225487","originSystem":"AadGroup"
  }
}
```

#### <a name="response"></a><span data-ttu-id="11bfa-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-207">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/entitlementManagement/accessPackages('88203d16-0e31-41d4-87b2-dd402f1435e9')/accessPackageResourceRoleScopes/$entity",
  "id": "e081321b-2802-4834-a6ca-6f598ce3cdf7_6dbd2209-9d14-4c76-b92b-fcb00e835fe1",
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-08-21T19:56:00.6320729Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-08-21T19:56:00.6320729Z"
}
```

<span data-ttu-id="11bfa-208">Пакет Access теперь имеет одну роль ресурса, которая является членством в группе.</span><span class="sxs-lookup"><span data-stu-id="11bfa-208">The access package now has one resource role, which is group membership.</span></span> <span data-ttu-id="11bfa-209">Роль назначается любому пользователю с пакетом доступа.</span><span class="sxs-lookup"><span data-stu-id="11bfa-209">The role is assigned to any user who has the access package.</span></span>

### <a name="create-an-access-package-policy"></a><span data-ttu-id="11bfa-210">Создание политики пакетов Access</span><span class="sxs-lookup"><span data-stu-id="11bfa-210">Create an access package policy</span></span>

<span data-ttu-id="11bfa-211">Теперь, когда вы создали пакет Access и добавили ресурсы и роли, вы можете определить, кто может получить доступ к нему, создав политику пакетов Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-211">Now that you created the access package and added resources and roles, you can decide who can access it by creating an access package policy.</span></span> <span data-ttu-id="11bfa-212">В этом руководстве показано, как включить созданную учетную запись **Requestor1** для запроса доступа к ресурсам в пакете Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-212">In this tutorial, you enable the **Requestor1** account that you created to request access to the resources in the access package.</span></span> <span data-ttu-id="11bfa-213">Для выполнения этой задачи необходимы следующие значения:</span><span class="sxs-lookup"><span data-stu-id="11bfa-213">For this task, you need these values:</span></span>
- <span data-ttu-id="11bfa-214">**идентификатор** пакета доступа для значения свойства **акцесспаккажеид**</span><span class="sxs-lookup"><span data-stu-id="11bfa-214">**id** of the access package for the value of the **accessPackageId** property</span></span>
- <span data-ttu-id="11bfa-215">**идентификатор** учетной записи пользователя **Requestor1** для значения свойства **ID** в **алловедрекуесторс**</span><span class="sxs-lookup"><span data-stu-id="11bfa-215">**id** of the **Requestor1** user account for the value of the **id** property in **allowedRequestors**</span></span>
 
<span data-ttu-id="11bfa-216">Значение свойства **дуратиониндайс** позволяет учетной записи **Requestor1** получать доступ к ресурсам в пакете Access в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="11bfa-216">The value of the **durationInDays** property enables the **Requestor1** account to access the resources in the access package for up to 30 days.</span></span> <span data-ttu-id="11bfa-217">Запишите значение свойства **ID** , которое возвращается для использования далее в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="11bfa-217">Record the value of the **id** property that is returned to use later in this tutorial.</span></span> 

#### <a name="request"></a><span data-ttu-id="11bfa-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-218">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
Content-type: application/json

{
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "accessReviewSettings": null,
  "durationInDays": 30,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.singleUser",
         "isBackup": false,
         "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
         "description": "Requestor1"
       }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

#### <a name="response"></a><span data-ttu-id="11bfa-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-219">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentPolicies/$entity",
  "id": "db440482-1210-4a60-9b55-3ac7a72f63ba",
  "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
  "displayName": "Specific users",
  "description": "Specific users can request assignment",
  "canExtend": false,
  "durationInDays": 30,
  "expirationDateTime": null,
  "createdBy": "admin@contoso.onmicrosoft.com",
  "createdDateTime": "2020-06-29T19:47:44.7399675Z",
  "modifiedBy": "admin@contoso.onmicrosoft.com",
  "modifiedDateTime": "2020-06-29T19:47:44.7555489Z",
  "accessReviewSettings": null,
  "requestorSettings": {
    "scopeType": "SpecificDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": [
      {
        "@odata.type": "#microsoft.graph.singleUser",
        "isBackup": false,
        "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
        "description": "Requestor1"
      }
    ]
  },
  "requestApprovalSettings": {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  }
}
```

## <a name="step-3-request-access"></a><span data-ttu-id="11bfa-220">Шаг 3: запрос доступа</span><span class="sxs-lookup"><span data-stu-id="11bfa-220">Step 3: Request access</span></span>

<span data-ttu-id="11bfa-221">На этом этапе учетная запись пользователя **Requestor1** запрашивает доступ к ресурсам в пакете Access.</span><span class="sxs-lookup"><span data-stu-id="11bfa-221">In this step, the **Requestor1** user account requests access to the resources in the access package.</span></span>

<span data-ttu-id="11bfa-222">Чтобы запросить доступ к ресурсам в пакете Access, необходимо указать следующие значения:</span><span class="sxs-lookup"><span data-stu-id="11bfa-222">To request access to resources in the access package, you need to provide these values:</span></span>
- <span data-ttu-id="11bfa-223">**идентификатор** учетной записи пользователя **Requestor1** , созданной для значения свойства **targetId**</span><span class="sxs-lookup"><span data-stu-id="11bfa-223">**id** of the **Requestor1** user account that you created for the value of the **targetId** property</span></span>
- <span data-ttu-id="11bfa-224">**идентификатор** политики назначения для значения свойства **ассигнментполициид**</span><span class="sxs-lookup"><span data-stu-id="11bfa-224">**id** of the assignment policy for the value of the **assignmentPolicyId** property</span></span>
- <span data-ttu-id="11bfa-225">**идентификатор** пакета доступа для значения свойства **акцесспаккажеид**</span><span class="sxs-lookup"><span data-stu-id="11bfa-225">**id** of the access package for the value of **accessPackageId** property</span></span>

<span data-ttu-id="11bfa-226">В ответ вы можете просмотреть состояние **принятого** и **отправленного**сообщения.</span><span class="sxs-lookup"><span data-stu-id="11bfa-226">In the response you can see the status of **Accepted** and a state of **Submitted**.</span></span> <span data-ttu-id="11bfa-227">Запишите значение свойства **ID** , которое возвращается для получения состояния запроса позже.</span><span class="sxs-lookup"><span data-stu-id="11bfa-227">Record the value of the **id** property that is returned to get the status of the request later.</span></span>

<span data-ttu-id="11bfa-228">Если вы еще не сделали этого, выйдите из учетной записи администратора, которая использовалась в обозревателе Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="11bfa-228">If you haven't done so already, sign out of the administrator account that you were using in Microsoft Graph Explorer.</span></span> <span data-ttu-id="11bfa-229">Войдите в созданную учетную запись пользователя **Requestor1** .</span><span class="sxs-lookup"><span data-stu-id="11bfa-229">Sign in to the **Requestor1** user account that you created.</span></span> <span data-ttu-id="11bfa-230">Вам будет предложено сменить пароль, если вы первый раз входите в нее.</span><span class="sxs-lookup"><span data-stu-id="11bfa-230">You will be asked to change the password if it is the first time you are signing in.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-231">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "UserAdd",
  "accessPackageAssignment":{
     "targetId":"007d1c7e-7fa8-4e33-b678-5e437acdcddc",
     "assignmentPolicyId":"db440482-1210-4a60-9b55-3ac7a72f63ba",
     "accessPackageId":"88203d16-0e31-41d4-87b2-dd402f1435e9"
  }
}
```

#### <a name="response"></a><span data-ttu-id="11bfa-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-232">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

## <a name="step-4-validate-that-access-has-been-assigned"></a><span data-ttu-id="11bfa-233">Шаг 4: Проверка назначения доступа</span><span class="sxs-lookup"><span data-stu-id="11bfa-233">Step 4: Validate that access has been assigned</span></span>

<span data-ttu-id="11bfa-234">На этом этапе вы подтверждаете, что учетной записи пользователя **Requestor1** был назначен пакет доступа и он теперь является участником группы " **маркетинговые ресурсы** ".</span><span class="sxs-lookup"><span data-stu-id="11bfa-234">In this step, you confirm that the **Requestor1** user account was assigned the access package and that they are now a member of the **Marketing resources** group.</span></span>

<span data-ttu-id="11bfa-235">Выйдите из учетной записи Requestor1 и войдите в учетную запись администратора, чтобы увидеть состояние запроса.</span><span class="sxs-lookup"><span data-stu-id="11bfa-235">Sign out of the Requestor1 account and sign back in to the administrator account to see the status of the request.</span></span>

### <a name="get-the-status-of-the-request"></a><span data-ttu-id="11bfa-236">Получение состояния запроса</span><span class="sxs-lookup"><span data-stu-id="11bfa-236">Get the status of the request</span></span>

<span data-ttu-id="11bfa-237">Используйте значение свойства **ID** запроса для получения текущего состояния.</span><span class="sxs-lookup"><span data-stu-id="11bfa-237">Use the value of the **id** property of the request to get the current status of it.</span></span> <span data-ttu-id="11bfa-238">В ответе вы можете увидеть состояние "выполнено", а состояние " **выполнено** " изменено на " **доставлено**".</span><span class="sxs-lookup"><span data-stu-id="11bfa-238">In the response, you can see the status changed to **Fulfilled** and the state changed to **Delivered**.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-239">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-239">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/a6bb6942-3ae1-4259-9908-0133aaee9377
```

#### <a name="response"></a><span data-ttu-id="11bfa-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-240">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
  "createdDateTime": "2020-06-29T20:24:24.683Z",
  "completedDate": "2020-06-29T20:24:47.937Z",
  "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
  "requestType": "UserAdd",
  "requestState": "Delivered",
  "requestStatus": "FulfilledNotificationTriggered",
  "isValidationOnly": false,
  "expirationDateTime": null,
  "justification": null
}
```

### <a name="get-access-package-assignments"></a><span data-ttu-id="11bfa-241">Назначения для получения пакетов Access</span><span class="sxs-lookup"><span data-stu-id="11bfa-241">Get access package assignments</span></span>

<span data-ttu-id="11bfa-242">Вы также можете использовать **идентификатор** созданной вами политики пакета Access, чтобы увидеть, что для учетной записи пользователя **Requestor1** назначены ресурсы.</span><span class="sxs-lookup"><span data-stu-id="11bfa-242">You can also use the **id** of the access package policy that you created to see that resources have been assigned to the **Requestor1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-243">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-243">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'
```

#### <a name="response"></a><span data-ttu-id="11bfa-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-244">Response</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignments",
  "value": [
    {
      "id": "a6bb6942-3ae1-4259-9908-0133aaee9377",
      "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
      "accessPackageId": "88203d16-0e31-41d4-87b2-dd402f1435e9",
      "assignmentPolicyId": "db440482-1210-4a60-9b55-3ac7a72f63ba",
      "targetId": "2bc42425-6dc5-4f2a-9ebb-7a7464481eb0",
      "assignmentStatus": "Delivered",
      "assignmentState": "Delivered",
      "isExtended": false,
      "expiredDateTime": null
    }
  ]
}
```

### <a name="get-the-members-of-the-group"></a><span data-ttu-id="11bfa-245">Получение членов группы</span><span class="sxs-lookup"><span data-stu-id="11bfa-245">Get the members of the group</span></span>

<span data-ttu-id="11bfa-246">После предоставления запроса вы можете использовать **идентификатор** , записанный для группы " **маркетинговые ресурсы** ", чтобы убедиться в том, что в нее добавлена учетная запись пользователя **Requestor1** .</span><span class="sxs-lookup"><span data-stu-id="11bfa-246">After the request has been granted, you can use the **id** that you recorded for the **Marketing resources** group to see that the **Requestor1** user account has been added to it.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-247">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/groups/e93e24d1-2b65-4a6c-a1dd-654a12225487/members
```

#### <a name="response"></a><span data-ttu-id="11bfa-248">Отклик:</span><span class="sxs-lookup"><span data-stu-id="11bfa-248">Response:</span></span>

```http
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "007d1c7e-7fa8-4e33-b678-5e437acdcddc",
      "deletedDateTime": null,
      "accountEnabled": true,
      "ageGroup": null,
      "businessPhones": [],
      "city": null,
      "createdDateTime": "2020-06-23T18:43:24Z",
      "creationType": null,
      "companyName": null,
      "consentProvidedForMinor": null,
      "country": null,
      "department": null,
      "displayName": "Requestor1",
      "employeeId": null,
      "faxNumber": null,
      "givenName": null,
      "imAddresses": [],
      "infoCatalogs": [],
      "isResourceAccount": null,
      "jobTitle": null,
      "legalAgeGroupClassification": null,
      "mail": null,
      "mailNickname": "Requestor1"
    }
  ]
}
```

## <a name="step-5-clean-up-resources"></a><span data-ttu-id="11bfa-249">Шаг 5: Очистка ресурсов</span><span class="sxs-lookup"><span data-stu-id="11bfa-249">Step 5: Clean up resources</span></span>

<span data-ttu-id="11bfa-250">На этом шаге вы удаляете внесенные вами изменения и удаляете пакет доступа к **маркетинговой кампании** .</span><span class="sxs-lookup"><span data-stu-id="11bfa-250">In this step, you remove the changes you made and delete the **Marketing Campaign** access package.</span></span>

### <a name="remove-an-access-package-assignment"></a><span data-ttu-id="11bfa-251">Удаление назначения пакета Access</span><span class="sxs-lookup"><span data-stu-id="11bfa-251">Remove an access package assignment</span></span>

<span data-ttu-id="11bfa-252">Перед удалением пакета Access необходимо удалить из него все назначения.</span><span class="sxs-lookup"><span data-stu-id="11bfa-252">You must remove any assignments to the access package before you can delete it.</span></span> <span data-ttu-id="11bfa-253">Используйте **идентификатор** запроса на назначение, который вы ранее записали, чтобы удалить его.</span><span class="sxs-lookup"><span data-stu-id="11bfa-253">Use the **id** of the assignment request that you previously recorded to delete it.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-254">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-254">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminRemove",
  "accessPackageAssignment":{
     "id": "a6bb6942-3ae1-4259-9908-0133aaee9377"
  }
}
```

#### <a name="response"></a><span data-ttu-id="11bfa-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-255">Response</span></span>

```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",
    "createdDateTime": null,
    "completedDate": null,
    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": null
}
```

### <a name="delete-the-access-package-assignment-policy"></a><span data-ttu-id="11bfa-256">Удаление политики назначения пакетов Access</span><span class="sxs-lookup"><span data-stu-id="11bfa-256">Delete the access package assignment policy</span></span>

<span data-ttu-id="11bfa-257">Используйте **идентификатор** ранее записанной политики назначения, чтобы удалить его.</span><span class="sxs-lookup"><span data-stu-id="11bfa-257">Use the **id** of the assignment policy that you previously recorded to delete it.</span></span> <span data-ttu-id="11bfa-258">Убедитесь, что сначала удаляются все назначения.</span><span class="sxs-lookup"><span data-stu-id="11bfa-258">Make sure all assignments are removed first.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-259">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-259">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/6c1f65ec-8c25-4a45-83c2-a1de2a6d0e9f
```

#### <a name="response"></a><span data-ttu-id="11bfa-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-260">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-access-package"></a><span data-ttu-id="11bfa-261">Удаление пакета Access</span><span class="sxs-lookup"><span data-stu-id="11bfa-261">Delete the access package</span></span>

<span data-ttu-id="11bfa-262">Используйте **идентификатор** пакета Access, который вы ранее записали, чтобы удалить его.</span><span class="sxs-lookup"><span data-stu-id="11bfa-262">Use the **id** of the access package that you previously recorded to delete it.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-263">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-263">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/cf54c6ca-d717-49bc-babe-d140d035dfdd
```

#### <a name="response"></a><span data-ttu-id="11bfa-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-264">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-user-account"></a><span data-ttu-id="11bfa-265">Удаление учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="11bfa-265">Delete the user account</span></span>

<span data-ttu-id="11bfa-266">Удалите учетную запись пользователя **Requestor1** .</span><span class="sxs-lookup"><span data-stu-id="11bfa-266">Delete the **Requestor1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-267">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-267">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/ce02eca8-752b-4ecf-ac29-aa9bccd87606
```

#### <a name="response"></a><span data-ttu-id="11bfa-268">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-268">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-group"></a><span data-ttu-id="11bfa-269">Добавлять и удалять участников группы.</span><span class="sxs-lookup"><span data-stu-id="11bfa-269">Delete the group</span></span>

<span data-ttu-id="11bfa-270">Удаление группы **маркетинговых ресурсов** .</span><span class="sxs-lookup"><span data-stu-id="11bfa-270">Delete the **Marketing resources** group.</span></span>

#### <a name="request"></a><span data-ttu-id="11bfa-271">Запрос</span><span class="sxs-lookup"><span data-stu-id="11bfa-271">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/groups/a468eaea-ed6c-4290-98d2-a96bb1cb4209
```

#### <a name="response"></a><span data-ttu-id="11bfa-272">Отклик</span><span class="sxs-lookup"><span data-stu-id="11bfa-272">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="11bfa-273">См. также</span><span class="sxs-lookup"><span data-stu-id="11bfa-273">See also</span></span>

<span data-ttu-id="11bfa-274">В этом руководстве показано, как использовать многие API для выполнения задач.</span><span class="sxs-lookup"><span data-stu-id="11bfa-274">In this tutorial, you used many APIs to accomplish tasks.</span></span> <span data-ttu-id="11bfa-275">Изучите Справочник по API для этих API, чтобы узнать больше о возможных действиях API.</span><span class="sxs-lookup"><span data-stu-id="11bfa-275">Explore the API reference for these APIs to learn more about what the APIs can do.</span></span>


- [<span data-ttu-id="11bfa-276">Работа с API управления обслуживанием Azure AD</span><span class="sxs-lookup"><span data-stu-id="11bfa-276">Working with the Azure AD entitlement management API</span></span>](https://docs.microsoft.com/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)
- [<span data-ttu-id="11bfa-277">акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="11bfa-277">accessPackageCatalog</span></span>](https://docs.microsoft.com/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)
- [<span data-ttu-id="11bfa-278">акцесспаккажересаурцерекуест</span><span class="sxs-lookup"><span data-stu-id="11bfa-278">accessPackageResourceRequest</span></span>](https://docs.microsoft.com/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta)
- [<span data-ttu-id="11bfa-279">акцесспаккаже</span><span class="sxs-lookup"><span data-stu-id="11bfa-279">accessPackage</span></span>](https://docs.microsoft.com/graph/api/resources/accesspackage?view=graph-rest-beta)
- [<span data-ttu-id="11bfa-280">акцесспаккажересаурцеролескопе</span><span class="sxs-lookup"><span data-stu-id="11bfa-280">accessPackageResourceRoleScope</span></span>](https://docs.microsoft.com/graph/api/resources/accesspackageresourcerolescope?view=graph-rest-beta)
- [<span data-ttu-id="11bfa-281">акцесспаккажеассигнментполици</span><span class="sxs-lookup"><span data-stu-id="11bfa-281">accessPackageAssignmentPolicy</span></span>](https://docs.microsoft.com/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)
- [<span data-ttu-id="11bfa-282">акцесспаккажеассигнментрекуест</span><span class="sxs-lookup"><span data-stu-id="11bfa-282">accessPackageAssignmentRequest</span></span>](https://docs.microsoft.com/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta)
- [<span data-ttu-id="11bfa-283">group</span><span class="sxs-lookup"><span data-stu-id="11bfa-283">group</span></span>](https://docs.microsoft.com/graph/api/resources/group?view=graph-rest-1.0)
- [<span data-ttu-id="11bfa-284">user</span><span class="sxs-lookup"><span data-stu-id="11bfa-284">user</span></span>](https://docs.microsoft.com/graph/api/resources/user?view=graph-rest-1.0)
