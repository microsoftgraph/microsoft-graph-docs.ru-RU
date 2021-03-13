---
title: Руководство. Управление доступом к ресурсам в управлении правами Active Directory с помощью API Microsoft Graph
description: Узнайте, как управлять доступом к ресурсам в управлении правами Active Directory (Azure AD) с помощью API Microsoft Graph.
author: davidmu1
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: b27bda23d32033205c21199d27d34dd360fa380d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760983"
---
# <a name="tutorial-manage-access-to-resources-in-active-directory-entitlement-management-using-microsoft-graph-apis"></a><span data-ttu-id="bc4e0-103">Руководство. Управление доступом к ресурсам в управлении правами Active Directory с помощью API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bc4e0-103">Tutorial: Manage access to resources in Active Directory entitlement management using Microsoft Graph APIs</span></span>

<span data-ttu-id="bc4e0-104">Управление доступом ко всем ресурсам, которые необходимы сотрудникам, таким как группы, приложения и сайты, является важной функцией для организаций.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-104">Managing access to all the resources that employees need, such as groups, applications, and sites, is an important function for organizations.</span></span> <span data-ttu-id="bc4e0-105">Вы хотите предоставить сотрудникам необходимый уровень доступа, чтобы они могли быть продуктивными, и удалить их доступ, когда он больше не нужен.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-105">You want to grant employees the right level of access they need to be productive and remove their access when it is no longer needed.</span></span> <span data-ttu-id="bc4e0-106">[Управление правами Azure Active Directory (Azure AD)](/azure/active-directory/governance/entitlement-management-overview) с помощью API Microsoft Graph позволяет управлять этим типом доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-106">[Azure Active Directory (Azure AD) entitlement management](/azure/active-directory/governance/entitlement-management-overview) using Microsoft Graph APIs enables you to manage this type of access.</span></span>

<span data-ttu-id="bc4e0-107">В этом руководстве вам было предложено разработать код для создания пакета ресурсов для маркетинговой кампании, которую внутренние пользователи могут запрашивать самостоятельно.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-107">In this tutorial, you've been asked to develop code to create a package of resources for a marketing campaign that internal users can self-service request.</span></span> <span data-ttu-id="bc4e0-108">Запросы не требуют утверждения, а срок доступа пользователя истекает через 30 дней.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-108">Requests do not require approval and user's access expires after 30 days.</span></span> <span data-ttu-id="bc4e0-109">Для этого руководства ресурсы маркетинговой кампании являются только членством в одной группе, но это может быть коллекция групп, приложений или сайтов SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-109">For this tutorial, the marketing campaign resources are just membership in a single group, but it could be a collection of groups, applications, or SharePoint Online sites.</span></span>

><span data-ttu-id="bc4e0-110">**Примечание:** Объекты отклика, показанные в этом руководстве, могут быть сокращены для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-110">**Note:** The response objects shown in this tutorial might be shortened for readability.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="bc4e0-111">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bc4e0-111">Prerequisites</span></span>

<span data-ttu-id="bc4e0-112">Чтобы успешно завершить этот учебник, убедитесь, что у вас есть необходимые предпосылки:</span><span class="sxs-lookup"><span data-stu-id="bc4e0-112">To successfully complete this tutorial, make sure that you have the required prerequisites:</span></span>
- <span data-ttu-id="bc4e0-113">Управление правами Azure AD требует определенных лицензий.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-113">Azure AD entitlement management requires specific licenses.</span></span> <span data-ttu-id="bc4e0-114">Дополнительные сведения см. в [дополнительных сведениях о требованиях к лицензии.](/azure/active-directory/governance/entitlement-management-overview#license-requirements)</span><span class="sxs-lookup"><span data-stu-id="bc4e0-114">For more information, see [License requirements](/azure/active-directory/governance/entitlement-management-overview#license-requirements).</span></span> <span data-ttu-id="bc4e0-115">В вашем клиенте требуются следующие лицензии:</span><span class="sxs-lookup"><span data-stu-id="bc4e0-115">The following licenses are required in your tenant:</span></span>
    - <span data-ttu-id="bc4e0-116">Azure AD Premium P2</span><span class="sxs-lookup"><span data-stu-id="bc4e0-116">Azure AD Premium P2</span></span>
    - <span data-ttu-id="bc4e0-117">Лицензия на корпоративную мобильность и безопасность (EMS) E5</span><span class="sxs-lookup"><span data-stu-id="bc4e0-117">Enterprise Mobility + Security (EMS) E5 license</span></span>
- <span data-ttu-id="bc4e0-118">В этом руководстве предполагается, что вы используете песочницу Microsoft Graph, но вы можете использовать Postman или создать собственное клиентское приложение, чтобы вызывать Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-118">This tutorial assumes that you are using Microsoft Graph Explorer, but you can use Postman, or create your own client app to call Microsoft Graph.</span></span> <span data-ttu-id="bc4e0-119">Чтобы вызвать API Microsoft Graph в этом руководстве, используйте учетную запись с ролью глобального администратора и соответствующими разрешениями.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-119">To call the Microsoft Graph APIs in this tutorial, you need to use an account with the global administrator role and the appropriate permissions.</span></span> <span data-ttu-id="bc4e0-120">Для этого руководства необходимы `User.ReadWrite.All` разрешения `Group.ReadWrite.All` , и `EntitlementManagement.ReadWrite.All` делегированная.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-120">For this tutorial, the `User.ReadWrite.All`, `Group.ReadWrite.All`, and `EntitlementManagement.ReadWrite.All` delegated permissions are needed.</span></span> <span data-ttu-id="bc4e0-121">Чтобы настроить разрешения в песочнице Microsoft Graph, выполните следующие действия.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-121">Complete the following steps to set permissions in Microsoft Graph Explorer:</span></span>
    1. <span data-ttu-id="bc4e0-122">Запустите [песочницу Microsoft Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="bc4e0-122">Start [Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
    2. <span data-ttu-id="bc4e0-123">Выберите вариант **Вход с помощью учетной записи Майкрософт** и войдите, используя учетную запись глобального администратора Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-123">Select **Sign-In with Microsoft** and sign in using an Azure AD global administrator account.</span></span> <span data-ttu-id="bc4e0-124">После успешного входа вы увидите данные учетной записи пользователя на панели слева.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-124">After you successfully sign in, you can see the user account details in the left-hand pane.</span></span>
    3. <span data-ttu-id="bc4e0-125">Щелкните значок параметров справа от сведений об учетной записи пользователя и нажмите **Выбор разрешений**.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-125">Select the settings icon to the right of the user account details, and then select **Select permissions**.</span></span>

        ![Выбор разрешений Microsoft Graph](./images/tutorial-access-package-api/set-permissions.png)
        
    4. <span data-ttu-id="bc4e0-127">Прокрутите список разрешений до разрешений, расширите `Group` **Группу (2),** выберите **разрешение Group.ReadWrite.All.**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-127">Scroll through the list of permissions to the `Group` permissions, expand **Group (2)**, select the **Group.ReadWrite.All** permission.</span></span> <span data-ttu-id="bc4e0-128">Прокрутите далее список разрешений до разрешений, расширите пользователь `User` **(8)** и выберите **разрешение User.ReadWrite.All.**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-128">Scroll further down the list of permissions to the `User` permissions, expand **User (8)**, and select the **User.ReadWrite.All** permission.</span></span>

        ![Поиск разрешений пользователя, группы и прав на получение прав](./images/tutorial-access-package-api/set-user-permission.png)
    
    5. <span data-ttu-id="bc4e0-130">Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-130">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="bc4e0-131">Вам не нужно предоставлять согласие от имени организации для этих разрешений.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-131">You do not need to consent on behalf of your organization for these permissions.</span></span>
    6. <span data-ttu-id="bc4e0-132">Поиск `EntitlementManagement` разрешений, расширение **EntitlementManagement (2),** выберите **разрешение Entitlement.ReadWrite.All,** а затем выберите **Согласие**.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-132">Search for the `EntitlementManagement` permissions, expand **EntitlementManagement (2)**, select the **Entitlement.ReadWrite.All** permission, and then select **Consent**.</span></span> <span data-ttu-id="bc4e0-133">Так как это разрешение требует согласия администратора и необходимо учетной записи пользователя, которую вы создаете в этом учебнике, необходимо выбрать Согласие от имени **вашей организации.**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-133">Because this permission requires admin consent and is needed by a user account that you create in this tutorial, you must select **Consent on behalf of your organization**.</span></span>

        ![Согласие на организацию](./images/tutorial-access-package-api/consent-for-organization.png)

    7. <span data-ttu-id="bc4e0-135">Выберите **Accept,** чтобы принять согласие на разрешения.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-135">Select **Accept** to accept the consent of the permissions.</span></span>

## <a name="step-1-create-a-user-account-and-a-group"></a><span data-ttu-id="bc4e0-136">Шаг 1. Создание учетной записи пользователя и группы</span><span class="sxs-lookup"><span data-stu-id="bc4e0-136">Step 1: Create a user account and a group</span></span>

<span data-ttu-id="bc4e0-137">На этом этапе в  каталоге создается группа маркетинговых ресурсов, которая является целевым ресурсом для управления правами.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-137">In this step, you create a group named **Marketing resources** in the directory that is the target resource for entitlement management.</span></span> <span data-ttu-id="bc4e0-138">Вы также создаете учетную запись пользователя, настроенную как внутренний запросчик.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-138">You also create a user account that is set up as an internal requestor.</span></span>

### <a name="create-a-user-account"></a><span data-ttu-id="bc4e0-139">Создание учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="bc4e0-139">Create a user account</span></span>

<span data-ttu-id="bc4e0-140">В этом руководстве создается учетная запись пользователя, которая используется для запроса доступа к ресурсам пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-140">For this tutorial, you create a user account that is used to request access to the resources in the access package.</span></span> <span data-ttu-id="bc4e0-141">Когда вы делаете эти вызовы, `contoso.onmicrosoft.com` измените доменное имя клиента.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-141">When you make these calls, change `contoso.onmicrosoft.com` to the domain name of your tenant.</span></span> <span data-ttu-id="bc4e0-142">Информацию о клиенте можно найти на странице обзора в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-142">You can find tenant information on the Azure Active Directory overview page.</span></span> <span data-ttu-id="bc4e0-143">Зафиксировать значение **свойства id,** которое возвращается для использования позже в учебнике.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-143">Record the value of the **id** property that is returned to be used later in the tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-144">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="bc4e0-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-145">Response</span></span>

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

### <a name="create-a-group"></a><span data-ttu-id="bc4e0-146">Создание группы</span><span class="sxs-lookup"><span data-stu-id="bc4e0-146">Create a group</span></span>

<span data-ttu-id="bc4e0-147">В этом руководстве создается группа маркетинговых **ресурсов,** которая является целевым ресурсом для управления правами.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-147">In this tutorial, you create a group named **Marketing resources** that is the target resource for entitlement management.</span></span> <span data-ttu-id="bc4e0-148">Можно использовать существующую группу, если она уже есть.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-148">You can use an existing group if you already have one.</span></span> <span data-ttu-id="bc4e0-149">Запись значения свойства **id,** которое возвращается для использования позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-149">Record the value of the **id** property that is returned to use later in this tutorial.</span></span> 

#### <a name="request"></a><span data-ttu-id="bc4e0-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-150">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="bc4e0-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-151">Response</span></span>

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

## <a name="step-2-add-resources-to-a-catalog-and-create-an-access-package"></a><span data-ttu-id="bc4e0-152">Шаг 2. Добавление ресурсов в каталог и создание пакета доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-152">Step 2: Add resources to a catalog and create an access package</span></span>

<span data-ttu-id="bc4e0-153">Пакет *доступа —* это набор ресурсов, необходимых команде или проекту и управляемых политиками.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-153">An *access package* is a bundle of resources that a team or project needs and is governed with policies.</span></span> <span data-ttu-id="bc4e0-154">Пакеты доступа определяются в контейнерах, называемых каталогами.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-154">Access packages are defined in containers called catalogs.</span></span> <span data-ttu-id="bc4e0-155">Каталоги могут ссылаться на ресурсы, такие как группы, приложения и сайты, которые используются в пакете доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-155">Catalogs can reference resources, such as groups, apps and sites, that are used in the access package.</span></span> <span data-ttu-id="bc4e0-156">На этом этапе создается пакет доступа **к маркетинговой** кампании в общем каталоге.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-156">In this step, you create a **Marketing Campaign** access package in the General catalog.</span></span> <span data-ttu-id="bc4e0-157">Если у вас другой каталог, используйте его имя в следующем разделе.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-157">If you have a different catalog, use its name in the next section.</span></span>

### <a name="get-the-catalog-identifier"></a><span data-ttu-id="bc4e0-158">Получить идентификатор каталога</span><span class="sxs-lookup"><span data-stu-id="bc4e0-158">Get the catalog identifier</span></span>

<span data-ttu-id="bc4e0-159">Чтобы добавить ресурсы в каталог, сначала необходимо получить его идентификатор.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-159">To add resources to the catalog, you must first get the identifier of it.</span></span> <span data-ttu-id="bc4e0-160">Если вы используете общий каталог, запустите следующий запрос, чтобы получить его идентификатор.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-160">If you are using the General catalog, run the following request to get its identifier.</span></span> <span data-ttu-id="bc4e0-161">Если используется другой калалог, измените значение фильтра в запросе на имя каталога.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-161">If you are using a different calalog, change the filter value in the request to the name of your catalog.</span></span> <span data-ttu-id="bc4e0-162">Запись значения свойства **id,** которое возвращается для использования позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-162">Record the value of the **id** property that is returned to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-163">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs?$filter=(displayName eq 'General')
```

#### <a name="response"></a><span data-ttu-id="bc4e0-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-164">Response</span></span>

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

<span data-ttu-id="bc4e0-165">Ответ должен содержать только каталог, имя которого вы предоставили в запросе.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-165">The response should only contain the catalog whose name you provided in the request.</span></span> <span data-ttu-id="bc4e0-166">Если не возвращаются значения, проверьте правильность имени каталога перед началом работы.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-166">If there are no values returned, check that the name of the catalog is correct before you proceed.</span></span>

### <a name="add-the-group-to-the-catalog"></a><span data-ttu-id="bc4e0-167">Добавление группы в каталог</span><span class="sxs-lookup"><span data-stu-id="bc4e0-167">Add the group to the catalog</span></span>

<span data-ttu-id="bc4e0-168">Чтобы добавить созданную группу в каталог, укайте следующие значения свойств:</span><span class="sxs-lookup"><span data-stu-id="bc4e0-168">To add the group that you created to the catalog, provide the following property values:</span></span>
- <span data-ttu-id="bc4e0-169">**catalogId** — **id** используемого каталога</span><span class="sxs-lookup"><span data-stu-id="bc4e0-169">**catalogId** - the **id** of the catalog that you are using</span></span>
- <span data-ttu-id="bc4e0-170">**displayName** — имя группы</span><span class="sxs-lookup"><span data-stu-id="bc4e0-170">**displayName** - the name of the group</span></span>
- <span data-ttu-id="bc4e0-171">**описание** — описание группы</span><span class="sxs-lookup"><span data-stu-id="bc4e0-171">**description** - the description of the group</span></span>
- <span data-ttu-id="bc4e0-172">**originId** — **id** созданной группы</span><span class="sxs-lookup"><span data-stu-id="bc4e0-172">**originId** - the **id** of the group that you created</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-173">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="bc4e0-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-174">Response</span></span>

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

### <a name="get-catalog-resources"></a><span data-ttu-id="bc4e0-175">Получить ресурсы каталога</span><span class="sxs-lookup"><span data-stu-id="bc4e0-175">Get catalog resources</span></span>

<span data-ttu-id="bc4e0-176">В последующих действиях в этом руководстве вам потребуется **id,** который был назначен групповому ресурсу в каталоге.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-176">In later steps in this tutorial, you need the **id** that was assigned to the group resource in the catalog.</span></span> <span data-ttu-id="bc4e0-177">Этот идентификатор, который представляет группу как ресурс в каталоге, отличается от идентификатора самой группы в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-177">This identifier, which represents the group as a resource in the catalog, is different than the identifier of the group itself in Microsoft Graph.</span></span> <span data-ttu-id="bc4e0-178">Это потому, что в каталоге могут быть ресурсы, которые не представлены в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-178">This is because a catalog can have resources which aren't represented in Microsoft Graph.</span></span>

<span data-ttu-id="bc4e0-179">В запросе укате **id** используемого каталога.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-179">In the request, provide the **id** of the catalog that you are using.</span></span> <span data-ttu-id="bc4e0-180">Запись значения свойства **id** для ресурса каталога группы.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-180">Record the value of the **id** property for the group catalog resource.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-181">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResources?$filter=(displayName eq 'Marketing resources')
```

#### <a name="response"></a><span data-ttu-id="bc4e0-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-182">Response</span></span>

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

### <a name="get-resources-roles"></a><span data-ttu-id="bc4e0-183">Получить роли ресурсов</span><span class="sxs-lookup"><span data-stu-id="bc4e0-183">Get resources roles</span></span>

<span data-ttu-id="bc4e0-184">Пакет доступа назначает пользователям роли ресурса.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-184">The access package assigns users to the roles of a resource.</span></span> <span data-ttu-id="bc4e0-185">Типичная роль группы — это роль участника.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-185">The typical role of a group is the member role.</span></span> <span data-ttu-id="bc4e0-186">Другие ресурсы, такие как сайты и приложения SharePoint Online, могут иметь много ролей.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-186">Other resources, such as SharePoint Online sites and applications, might have many roles.</span></span> <span data-ttu-id="bc4e0-187">Типичная роль группы, используемой в пакете доступа, — это роль участника.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-187">The typical role of a group used in an access package is the member role.</span></span> <span data-ttu-id="bc4e0-188">Роль участника потребуется при добавлении роли ресурса в пакет доступа позже в этом учебнике.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-188">You'll need the member role when you add a resource role to the access package later in this tutorial.</span></span> 

<span data-ttu-id="bc4e0-189">В запросе используйте **id** каталога и **id** группового ресурса в каталоге, который вы записали, чтобы получить **originId** роли ресурса Member.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-189">In the request, use the **id** of the catalog and the **id** of the group resource in the catalog that you recorded to get the **originId** of the Member resource role.</span></span> <span data-ttu-id="bc4e0-190">Зафиксировать значение **свойства originId,** используемого позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-190">Record the value of the **originId** property to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-191">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/cec5d6ab-c75d-47c0-9c1c-92e89f66e384/accessPackageResourceRoles?$filter=(originSystem+eq+%27AadGroup%27+and+accessPackageResource/id+eq+%274a1e21c5-8a76-4578-acb1-641160e076e8%27+and+displayName+eq+%27Member%27)&$expand=accessPackageResource
```

#### <a name="response"></a><span data-ttu-id="bc4e0-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-192">Response</span></span>

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

<span data-ttu-id="bc4e0-193">В случае успешной работы возвращается одно значение, которое представляет роль участника этой группы.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-193">If successful, a single value is returned, which represents the Member role of that group.</span></span> <span data-ttu-id="bc4e0-194">Если роли не возвращаются, проверьте значения **id** каталога и ресурса пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-194">If no roles are returned, check the **id** values of the catalog and the access package resource.</span></span>

### <a name="create-the-access-package"></a><span data-ttu-id="bc4e0-195">Создание пакета доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-195">Create the access package</span></span>

<span data-ttu-id="bc4e0-196">На этом этапе у вас есть каталог с групповым ресурсом, и вы знаете, что в пакете доступа используется роль ресурса участника группы.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-196">At this point, you have a catalog with a group resource, and you know that you'll use the resource role of group member in the access package.</span></span> <span data-ttu-id="bc4e0-197">Следующий шаг — создание пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-197">The next step is to create the access package.</span></span> <span data-ttu-id="bc4e0-198">После получения пакета доступа можно добавить в него роль ресурса и создать политику, которая позволяет пользователям запрашивать доступ к этой роли ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-198">After you have the access package, you can add the resource role to it, and create a policy for how users can request access to that resource role.</span></span> <span data-ttu-id="bc4e0-199">Для создания пакета доступа используется **id** каталога, записанный ранее.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-199">You use the **id** of the catalog that you recorded earlier to create the access package.</span></span> <span data-ttu-id="bc4e0-200">Запись **id пакета** доступа, который можно использовать позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-200">Record the **id** of the access package to use later in this tutorial.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-201">Request</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "cec5d6ab-c75d-47c0-9c1c-92e89f66e384",
  "displayName": "Marketing Campaign",
  "description": "Access to resources for the campaign"
}
```

#### <a name="response"></a><span data-ttu-id="bc4e0-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-202">Response</span></span>

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

### <a name="add-a-resource-role-to-the-access-package"></a><span data-ttu-id="bc4e0-203">Добавление роли ресурса в пакет доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-203">Add a resource role to the access package</span></span>

<span data-ttu-id="bc4e0-204">Добавьте роль Участника группового ресурса в пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-204">Add the Member role of the group resource to the access package.</span></span> <span data-ttu-id="bc4e0-205">В запросе укад. **id** пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-205">In the request, provide the **id** of the access package.</span></span> <span data-ttu-id="bc4e0-206">В теле запроса укажи **id** ресурса группового каталога для accessPackageResource и укажи **originId** роли Member, которую вы ранее записывали.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-206">In the request body provide the **id** of the group catalog resource for accessPackageResource, and provide the **originId** of the Member role that you previously recorded.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-207">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="bc4e0-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-208">Response</span></span>

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

<span data-ttu-id="bc4e0-209">Пакет доступа теперь имеет одну роль ресурса, которая является членством в группе.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-209">The access package now has one resource role, which is group membership.</span></span> <span data-ttu-id="bc4e0-210">Роль назначена любому пользователю, у которого есть пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-210">The role is assigned to any user who has the access package.</span></span>

### <a name="create-an-access-package-policy"></a><span data-ttu-id="bc4e0-211">Создание политики пакета доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-211">Create an access package policy</span></span>

<span data-ttu-id="bc4e0-212">Теперь, когда вы создали пакет доступа и добавили ресурсы и роли, вы можете решить, кто может получить к нему доступ, создав политику пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-212">Now that you created the access package and added resources and roles, you can decide who can access it by creating an access package policy.</span></span> <span data-ttu-id="bc4e0-213">В этом руководстве вы включаете созданную учетную запись **Requestor1** для запроса доступа к ресурсам пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-213">In this tutorial, you enable the **Requestor1** account that you created to request access to the resources in the access package.</span></span> <span data-ttu-id="bc4e0-214">Для этой задачи нужны эти значения:</span><span class="sxs-lookup"><span data-stu-id="bc4e0-214">For this task, you need these values:</span></span>
- <span data-ttu-id="bc4e0-215">**id** пакета доступа для значения **свойства accessPackageId**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-215">**id** of the access package for the value of the **accessPackageId** property</span></span>
- <span data-ttu-id="bc4e0-216">**id** **учетной записи пользователя Requestor1** для значения свойства **id** в **allowedRequestors**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-216">**id** of the **Requestor1** user account for the value of the **id** property in **allowedRequestors**</span></span>
 
<span data-ttu-id="bc4e0-217">Значение свойства **durationInDays** позволяет учетной записи **Requestor1** получать доступ к ресурсам в пакете доступа на срок до 30 дней.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-217">The value of the **durationInDays** property enables the **Requestor1** account to access the resources in the access package for up to 30 days.</span></span> <span data-ttu-id="bc4e0-218">Запись значения свойства **id,** которое возвращается для использования позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-218">Record the value of the **id** property that is returned to use later in this tutorial.</span></span> 

#### <a name="request"></a><span data-ttu-id="bc4e0-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-219">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="bc4e0-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-220">Response</span></span>

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

## <a name="step-3-request-access"></a><span data-ttu-id="bc4e0-221">Шаг 3. Запрос доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-221">Step 3: Request access</span></span>

<span data-ttu-id="bc4e0-222">На этом этапе учетная запись **пользователя Requestor1** запрашивает доступ к ресурсам пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-222">In this step, the **Requestor1** user account requests access to the resources in the access package.</span></span>

<span data-ttu-id="bc4e0-223">Чтобы запросить доступ к ресурсам в пакете доступа, необходимо упросить эти значения:</span><span class="sxs-lookup"><span data-stu-id="bc4e0-223">To request access to resources in the access package, you need to provide these values:</span></span>
- <span data-ttu-id="bc4e0-224">**id** **учетной записи пользователя Requestor1,** созданной для значения **свойства targetId**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-224">**id** of the **Requestor1** user account that you created for the value of the **targetId** property</span></span>
- <span data-ttu-id="bc4e0-225">**id** политики назначения для значения **свойства assignmentPolicyId**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-225">**id** of the assignment policy for the value of the **assignmentPolicyId** property</span></span>
- <span data-ttu-id="bc4e0-226">**id** пакета доступа для значения **свойства accessPackageId**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-226">**id** of the access package for the value of **accessPackageId** property</span></span>

<span data-ttu-id="bc4e0-227">В ответе вы можете увидеть состояние Принято **и** состояние **Отправка**.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-227">In the response you can see the status of **Accepted** and a state of **Submitted**.</span></span> <span data-ttu-id="bc4e0-228">Зафиксировать значение возвращаемого свойства **id,** чтобы получить состояние запроса позже.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-228">Record the value of the **id** property that is returned to get the status of the request later.</span></span>

<span data-ttu-id="bc4e0-229">Если вы еще этого не сделали, выпишитесь из учетной записи администратора, используемой в Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-229">If you haven't done so already, sign out of the administrator account that you were using in Microsoft Graph Explorer.</span></span> <span data-ttu-id="bc4e0-230">Вопишите в **созданную учетную запись пользователя Requestor1.**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-230">Sign in to the **Requestor1** user account that you created.</span></span> <span data-ttu-id="bc4e0-231">При первом входе вам будет предложено изменить пароль.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-231">You will be asked to change the password if it is the first time you are signing in.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-232">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="bc4e0-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-233">Response</span></span>

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

## <a name="step-4-validate-that-access-has-been-assigned"></a><span data-ttu-id="bc4e0-234">Шаг 4. Проверка назначенного доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-234">Step 4: Validate that access has been assigned</span></span>

<span data-ttu-id="bc4e0-235">На этом шаге вы подтверждаете, что учетной записи **пользователя Requestor1** был назначен пакет доступа и что теперь они являются членом группы **маркетинговых ресурсов.**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-235">In this step, you confirm that the **Requestor1** user account was assigned the access package and that they are now a member of the **Marketing resources** group.</span></span>

<span data-ttu-id="bc4e0-236">Выпишитесь из учетной записи Requestor1 и впишитесь в учетную запись администратора, чтобы узнать состояние запроса.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-236">Sign out of the Requestor1 account and sign back in to the administrator account to see the status of the request.</span></span>

### <a name="get-the-status-of-the-request"></a><span data-ttu-id="bc4e0-237">Получить состояние запроса</span><span class="sxs-lookup"><span data-stu-id="bc4e0-237">Get the status of the request</span></span>

<span data-ttu-id="bc4e0-238">Чтобы получить текущее состояние, используйте значение свойства **id** запроса.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-238">Use the value of the **id** property of the request to get the current status of it.</span></span> <span data-ttu-id="bc4e0-239">В ответе можно увидеть, как состояние изменено на **Fulfilled,** а состояние изменено на **Delivered**.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-239">In the response, you can see the status changed to **Fulfilled** and the state changed to **Delivered**.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-240">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/a6bb6942-3ae1-4259-9908-0133aaee9377
```

#### <a name="response"></a><span data-ttu-id="bc4e0-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-241">Response</span></span>

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

### <a name="get-access-package-assignments"></a><span data-ttu-id="bc4e0-242">Назначение пакета доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-242">Get access package assignments</span></span>

<span data-ttu-id="bc4e0-243">Вы также можете использовать **id** созданной политики пакетов доступа, чтобы увидеть, что ресурсы назначены учетной записи **пользователя Requestor1.**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-243">You can also use the **id** of the access package policy that you created to see that resources have been assigned to the **Requestor1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-244">Request</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=accessPackageAssignmentPolicy/Id eq 'db440482-1210-4a60-9b55-3ac7a72f63ba'
```

#### <a name="response"></a><span data-ttu-id="bc4e0-245">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-245">Response</span></span>

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

### <a name="get-the-members-of-the-group"></a><span data-ttu-id="bc4e0-246">Получить участников группы</span><span class="sxs-lookup"><span data-stu-id="bc4e0-246">Get the members of the group</span></span>

<span data-ttu-id="bc4e0-247">После предоставления запроса можно использовать **id,** записанный для  группы маркетинговых ресурсов, чтобы увидеть, что учетная запись пользователя **Requestor1** была добавлена в нее.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-247">After the request has been granted, you can use the **id** that you recorded for the **Marketing resources** group to see that the **Requestor1** user account has been added to it.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-248">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/groups/e93e24d1-2b65-4a6c-a1dd-654a12225487/members
```

#### <a name="response"></a><span data-ttu-id="bc4e0-249">Отклик:</span><span class="sxs-lookup"><span data-stu-id="bc4e0-249">Response:</span></span>

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

## <a name="step-5-clean-up-resources"></a><span data-ttu-id="bc4e0-250">Шаг 5. Очистка ресурсов</span><span class="sxs-lookup"><span data-stu-id="bc4e0-250">Step 5: Clean up resources</span></span>

<span data-ttu-id="bc4e0-251">На этом шаге удалите внесенные изменения и удалите пакет доступа **к маркетинговой** кампании.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-251">In this step, you remove the changes you made and delete the **Marketing Campaign** access package.</span></span>

### <a name="remove-an-access-package-assignment"></a><span data-ttu-id="bc4e0-252">Удаление назначения пакета доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-252">Remove an access package assignment</span></span>

<span data-ttu-id="bc4e0-253">Прежде чем удалить его, необходимо удалить все назначения в пакет доступа.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-253">You must remove any assignments to the access package before you can delete it.</span></span> <span data-ttu-id="bc4e0-254">Чтобы удалить его, используйте **id** запроса на назначение, записанного ранее.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-254">Use the **id** of the assignment request that you previously recorded to delete it.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-255">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-255">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="bc4e0-256">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-256">Response</span></span>

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

### <a name="delete-the-access-package-assignment-policy"></a><span data-ttu-id="bc4e0-257">Удаление политики назначения пакета доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-257">Delete the access package assignment policy</span></span>

<span data-ttu-id="bc4e0-258">Чтобы удалить его, используйте **id** политики назначения, записанную ранее.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-258">Use the **id** of the assignment policy that you previously recorded to delete it.</span></span> <span data-ttu-id="bc4e0-259">Сначала убедитесь, что все назначения удаляются.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-259">Make sure all assignments are removed first.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-260">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-260">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/6c1f65ec-8c25-4a45-83c2-a1de2a6d0e9f
```

#### <a name="response"></a><span data-ttu-id="bc4e0-261">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-261">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-access-package"></a><span data-ttu-id="bc4e0-262">Удаление пакета доступа</span><span class="sxs-lookup"><span data-stu-id="bc4e0-262">Delete the access package</span></span>

<span data-ttu-id="bc4e0-263">Чтобы удалить его, используйте **id** пакета доступа, который был записан ранее.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-263">Use the **id** of the access package that you previously recorded to delete it.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-264">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-264">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/cf54c6ca-d717-49bc-babe-d140d035dfdd
```

#### <a name="response"></a><span data-ttu-id="bc4e0-265">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-265">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-user-account"></a><span data-ttu-id="bc4e0-266">Удаление учетной записи пользователя</span><span class="sxs-lookup"><span data-stu-id="bc4e0-266">Delete the user account</span></span>

<span data-ttu-id="bc4e0-267">Удаление **учетной записи пользователя Requestor1.**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-267">Delete the **Requestor1** user account.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-268">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-268">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/users/ce02eca8-752b-4ecf-ac29-aa9bccd87606
```

#### <a name="response"></a><span data-ttu-id="bc4e0-269">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-269">Response</span></span>

```http
No Content - 204
```

### <a name="delete-the-group"></a><span data-ttu-id="bc4e0-270">Добавлять и удалять участников группы.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-270">Delete the group</span></span>

<span data-ttu-id="bc4e0-271">Удаление **группы маркетинговых ресурсов.**</span><span class="sxs-lookup"><span data-stu-id="bc4e0-271">Delete the **Marketing resources** group.</span></span>

#### <a name="request"></a><span data-ttu-id="bc4e0-272">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc4e0-272">Request</span></span>

```http
DELETE https://graph.microsoft.com/v1.0/groups/a468eaea-ed6c-4290-98d2-a96bb1cb4209
```

#### <a name="response"></a><span data-ttu-id="bc4e0-273">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc4e0-273">Response</span></span>

```http
No Content - 204
```

## <a name="see-also"></a><span data-ttu-id="bc4e0-274">См. также</span><span class="sxs-lookup"><span data-stu-id="bc4e0-274">See also</span></span>

<span data-ttu-id="bc4e0-275">В этом руководстве вы использовали множество API для выполнения задач.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-275">In this tutorial, you used many APIs to accomplish tasks.</span></span> <span data-ttu-id="bc4e0-276">Ознакомьтесь со ссылкой на API для этих API, чтобы узнать больше о том, что могут делать API.</span><span class="sxs-lookup"><span data-stu-id="bc4e0-276">Explore the API reference for these APIs to learn more about what the APIs can do.</span></span>


- [<span data-ttu-id="bc4e0-277">Работа с API управления правами Azure AD</span><span class="sxs-lookup"><span data-stu-id="bc4e0-277">Working with the Azure AD entitlement management API</span></span>](/graph/api/resources/entitlementmanagement-root?view=graph-rest-beta)
- [<span data-ttu-id="bc4e0-278">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="bc4e0-278">accessPackageCatalog</span></span>](/graph/api/resources/accesspackagecatalog?view=graph-rest-beta)
- [<span data-ttu-id="bc4e0-279">accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="bc4e0-279">accessPackageResourceRequest</span></span>](/graph/api/resources/accesspackageresourcerequest?view=graph-rest-beta)
- [<span data-ttu-id="bc4e0-280">accessPackage</span><span class="sxs-lookup"><span data-stu-id="bc4e0-280">accessPackage</span></span>](/graph/api/resources/accesspackage?view=graph-rest-beta)
- [<span data-ttu-id="bc4e0-281">accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="bc4e0-281">accessPackageResourceRoleScope</span></span>](/graph/api/resources/accesspackageresourcerolescope?view=graph-rest-beta)
- [<span data-ttu-id="bc4e0-282">accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="bc4e0-282">accessPackageAssignmentPolicy</span></span>](/graph/api/resources/accesspackageassignmentpolicy?view=graph-rest-beta)
- [<span data-ttu-id="bc4e0-283">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="bc4e0-283">accessPackageAssignmentRequest</span></span>](/graph/api/resources/accesspackageassignmentrequest?view=graph-rest-beta)
- [<span data-ttu-id="bc4e0-284">group</span><span class="sxs-lookup"><span data-stu-id="bc4e0-284">group</span></span>](/graph/api/resources/group?view=graph-rest-1.0)
- [<span data-ttu-id="bc4e0-285">user</span><span class="sxs-lookup"><span data-stu-id="bc4e0-285">user</span></span>](/graph/api/resources/user?view=graph-rest-1.0)