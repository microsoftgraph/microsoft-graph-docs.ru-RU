---
title: Руководство. Используйте API обзоров доступа для просмотра гостевого доступа к группам Microsoft 365
description: Используйте API отзывов доступа, чтобы просмотреть гостевой доступ к группам Microsoft 365
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: 216d6e345fcbb2919593f95b327a2b83037e4535
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921106"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a><span data-ttu-id="494f2-103">Руководство. Используйте API обзоров доступа для просмотра гостевого доступа к группам Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="494f2-103">Tutorial: Use the access reviews API to review guest access to your Microsoft 365 groups</span></span>

<span data-ttu-id="494f2-104">В этом руководстве вы будете использовать Graph Explorer для создания и чтения отзывов доступа, которые ориентированы на все группы Microsoft 365 с гостевых пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="494f2-104">In this tutorial, you will use Graph Explorer to create and read access reviews that targets all Microsoft 365 groups with guest users in the tenant.</span></span> <span data-ttu-id="494f2-105">Для этого сначала с помощью Azure AD B2B вы сможете приглашать и создавать гостевого пользователя, также именуемого внешним удостоверением, в клиенте.</span><span class="sxs-lookup"><span data-stu-id="494f2-105">To achieve this, you'll first use Azure AD B2B to invite and create a guest user, also referred to as an external identity, in your tenant.</span></span> <span data-ttu-id="494f2-106">Затем этот гостевой пользователь будет добавлен в группу Microsoft 365 перед созданием и чтением обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="494f2-106">Then, you'll add this guest user to your Microsoft 365 group prior to creating and reading the access review.</span></span>

>[!NOTE]
><span data-ttu-id="494f2-107">Объекты отклика, показанные в этом руководстве, могут быть сокращены для чтения.</span><span class="sxs-lookup"><span data-stu-id="494f2-107">The response objects shown in this tutorial might be shortened for readability.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="494f2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="494f2-108">Prerequisites</span></span>

<span data-ttu-id="494f2-109">Для завершения этого руководства необходимы следующие ресурсы и привилегии:</span><span class="sxs-lookup"><span data-stu-id="494f2-109">To complete this tutorial, you need the following resources and privileges:</span></span>

+ <span data-ttu-id="494f2-110">Рабочий клиент Azure AD с включенной лицензией Azure AD Premium P2 или EMS E5.</span><span class="sxs-lookup"><span data-stu-id="494f2-110">A working Azure AD tenant with an Azure AD Premium P2 or EMS E5 license enabled.</span></span> 
+ <span data-ttu-id="494f2-111">Учетная запись в другом клиенте Azure AD или социальном удостоверении, которую можно пригласить в качестве гостевого пользователя (B2B-пользователя).</span><span class="sxs-lookup"><span data-stu-id="494f2-111">An account in a different Azure AD tenant or a social identity that you can invite as a guest user (B2B user).</span></span>
+ <span data-ttu-id="494f2-112">Во входе [в Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) в качестве пользователя в роли глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="494f2-112">Sign in to [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) as a user in a global administrator role.</span></span> 
+ <span data-ttu-id="494f2-113">Следующие делегированные разрешения: `User.Invite.All` `AccessReview.ReadWrite.All` , , `Group.ReadWrite.All` `User.ReadWrite.All` .</span><span class="sxs-lookup"><span data-stu-id="494f2-113">The following delegated permissions: `User.Invite.All`, `AccessReview.ReadWrite.All`, `Group.ReadWrite.All`, `User.ReadWrite.All`.</span></span>

<span data-ttu-id="494f2-114">Согласие на необходимые разрешения в Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="494f2-114">To consent to the required permissions in Graph Explorer:</span></span>
1. <span data-ttu-id="494f2-115">Выберите значок параметров справа от сведений учетной записи пользователя, а затем выберите **Выберите разрешения.**</span><span class="sxs-lookup"><span data-stu-id="494f2-115">Select the settings icon to the right of the user account details, and then choose **Select permissions**.</span></span>
   
   <span data-ttu-id="494f2-116">![Выбор разрешений Microsoft Graph](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
   </span><span class="sxs-lookup"><span data-stu-id="494f2-116">![Select the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Select the Microsoft Graph permissions":::-->

2. <span data-ttu-id="494f2-117">Прокрутите список разрешений для этих разрешений:</span><span class="sxs-lookup"><span data-stu-id="494f2-117">Scroll through the list of permissions to these permissions:</span></span>
   + <span data-ttu-id="494f2-118">AccessReviews (3), расширяйте и выберите **AccessReviews.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="494f2-118">AccessReviews (3), expand and then select **AccessReviews.ReadWrite.All**.</span></span>
   + <span data-ttu-id="494f2-119">Группа (2), развиньте и выберите **Group.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="494f2-119">Group (2), expand and then select **Group.ReadWrite.All**.</span></span>
   + <span data-ttu-id="494f2-120">Пользователь (8), расширить и затем выбрать **User.Invite.All** и **User.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="494f2-120">User (8), expand and then select **User.Invite.All** and **User.ReadWrite.All**.</span></span>
   
   <span data-ttu-id="494f2-121">Нажмите **Согласие** и выберите **Принять**, чтобы согласиться принять разрешения.</span><span class="sxs-lookup"><span data-stu-id="494f2-121">Select **Consent**, and then select **Accept** to accept the consent of the permissions.</span></span> <span data-ttu-id="494f2-122">Вам не нужно предоставлять согласие от имени организации для этих разрешений.</span><span class="sxs-lookup"><span data-stu-id="494f2-122">You do not need to consent on behalf of your organization for these permissions.</span></span>
   
   <span data-ttu-id="494f2-123">![Согласие на разрешения Microsoft Graph](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png)
   </span><span class="sxs-lookup"><span data-stu-id="494f2-123">![Consent to the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png" alt-text="Consent to the Microsoft Graph permissions":::-->

## <a name="step-1-create-a-test-user-in-your-tenant"></a><span data-ttu-id="494f2-124">Шаг 1. Создание тестового пользователя в клиенте</span><span class="sxs-lookup"><span data-stu-id="494f2-124">Step 1: Create a test user in your tenant</span></span>

### <a name="request"></a><span data-ttu-id="494f2-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-125">Request</span></span>

```http
POST /users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a><span data-ttu-id="494f2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-126">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "c9a5aff7-9298-4d71-adab-0a222e0a05e4",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-invite-a-guest-user-into-your-tenant"></a><span data-ttu-id="494f2-127">Шаг 2. Приглашение гостевого пользователя в клиента</span><span class="sxs-lookup"><span data-stu-id="494f2-127">Step 2: Invite a guest user into your tenant</span></span>

<span data-ttu-id="494f2-128">Приглашение гостевого пользователя с адресом **электронной почты john@tailspintoys.com** клиенту.</span><span class="sxs-lookup"><span data-stu-id="494f2-128">Invite a guest user with the email address **john@tailspintoys.com** to your tenant.</span></span>

### <a name="request"></a><span data-ttu-id="494f2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-129">Request</span></span>

```http
POST https://graph.microsoft.com/beta/invitations
Content-Type: application/json

{
    "invitedUserDisplayName": "John Doe (Tailspin Toys)",
    "invitedUserEmailAddress": "john@tailspintoys.com",
    "sendInvitationMessage": false,
    "inviteRedirectUrl": "https://myapps.microsoft.com"
}
```

### <a name="response"></a><span data-ttu-id="494f2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-130">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#invitations/$entity",
    "invitedUser": {
        "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    }    
}
```

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a><span data-ttu-id="494f2-131">Шаг 3. Создание новой группы Microsoft 365 и добавление гостевого пользователя</span><span class="sxs-lookup"><span data-stu-id="494f2-131">Step 3: Create a new Microsoft 365 group and add the guest user</span></span>

<span data-ttu-id="494f2-132">На этом шаге:</span><span class="sxs-lookup"><span data-stu-id="494f2-132">In this step:</span></span>
1. <span data-ttu-id="494f2-133">Создайте новую группу Microsoft 365 с именем **Маркетинговая кампания Feelgood.**</span><span class="sxs-lookup"><span data-stu-id="494f2-133">Create a new Microsoft 365 group named **Feelgood marketing campaign**.</span></span>
2. <span data-ttu-id="494f2-134">Назначьте себя владельцем группы.</span><span class="sxs-lookup"><span data-stu-id="494f2-134">Assign yourself as the group owner.</span></span>
3. <span data-ttu-id="494f2-135">Добавьте john@tailspintoys.com в качестве участника группы.</span><span class="sxs-lookup"><span data-stu-id="494f2-135">Add john@tailspintoys.com as a group member.</span></span> <span data-ttu-id="494f2-136">Их доступ к группе является предметом рассмотрения вами, владельцем группы.</span><span class="sxs-lookup"><span data-stu-id="494f2-136">Their access to the group is the subject of review by you, the group owner.</span></span>

### <a name="request"></a><span data-ttu-id="494f2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-137">Request</span></span>
<span data-ttu-id="494f2-138">В этом вызове замените:</span><span class="sxs-lookup"><span data-stu-id="494f2-138">In this call, replace:</span></span>
+ <span data-ttu-id="494f2-139">`cdb555e3-b33e-4fd5-a427-17fadacbdfa7` с **вашим id**. Чтобы получить свой **id,** `GET` запустите `https://graph.microsoft.com/beta/me` .</span><span class="sxs-lookup"><span data-stu-id="494f2-139">`cdb555e3-b33e-4fd5-a427-17fadacbdfa7` with your **id**. To retrieve your **id**, run `GET` on `https://graph.microsoft.com/beta/me`.</span></span>
+ <span data-ttu-id="494f2-140">`baf1b0a0-1f9a-4a56-9884-6a30824f8d20` с **john@tailspintoys.com**'s **id** из ответа в шаге 2.</span><span class="sxs-lookup"><span data-stu-id="494f2-140">`baf1b0a0-1f9a-4a56-9884-6a30824f8d20` with **john@tailspintoys.com**'s **id** from the response in Step 2.</span></span>

```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
    "description": "Feelgood Marketing Campaign with external partners and vendors.",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ],
    "mailEnabled": true,
    "mailNickname": "FeelGoodCampaign",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    ]
}
```

### <a name="response"></a><span data-ttu-id="494f2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-141">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "59ab642a-2776-4e32-9b68-9ff7a47b7f6a",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ]
}
```

<span data-ttu-id="494f2-142">Теперь у вас есть группа Microsoft 365 с гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="494f2-142">You now have a Microsoft 365 group with a guest user.</span></span>

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a><span data-ttu-id="494f2-143">Шаг 4. Создание обзора доступа для всех групп Microsoft 365 с гостевых пользователей</span><span class="sxs-lookup"><span data-stu-id="494f2-143">Step 4: Create an access review for all Microsoft 365 groups with guest users</span></span>

<span data-ttu-id="494f2-144">При создании серии повторяющихся обзоров доступа для всех групп Microsoft 365 с гостевых пользователей вы запланировать периодический обзор доступа гостей к группе Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="494f2-144">When you create a recurring access review series for all Microsoft 365 groups with guest users, you schedule a periodic review of the guests' access to the Microsoft 365 group.</span></span> <span data-ttu-id="494f2-145">Сделайте это для **группы маркетинговой кампании Feelgood.**</span><span class="sxs-lookup"><span data-stu-id="494f2-145">Do this for the **Feelgood Marketing Campaign** group.</span></span>

<span data-ttu-id="494f2-146">В серии обзоров доступа используются следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="494f2-146">The access review series uses following settings:</span></span>
+ <span data-ttu-id="494f2-147">Это повторяющийся обзор доступа, который пересматривается ежеквартно.</span><span class="sxs-lookup"><span data-stu-id="494f2-147">It's a recurring access review and reviewed quarterly.</span></span>
+ <span data-ttu-id="494f2-148">Владельцы групп проверяют постоянный доступ гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="494f2-148">The group owners review the continued access of guest users.</span></span>
+ <span data-ttu-id="494f2-149">Область обзора ограничена группами Microsoft 365 только для **гостевых** пользователей.</span><span class="sxs-lookup"><span data-stu-id="494f2-149">The review scope is limited to Microsoft 365 groups with **Guest users** only.</span></span>
+ <span data-ttu-id="494f2-150">Обозреватель резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="494f2-150">A backup reviewer.</span></span> <span data-ttu-id="494f2-151">Это может быть пользователь с откатом или группа, которая может просмотреть доступ в случае, если у группы нет владельцев.</span><span class="sxs-lookup"><span data-stu-id="494f2-151">This can be a fallback user or a group that can review the access in case the group doesn't have any owners assigned.</span></span>
+ <span data-ttu-id="494f2-152">**autoApplyDecisionsEnabled** установлено `true` для .</span><span class="sxs-lookup"><span data-stu-id="494f2-152">**autoApplyDecisionsEnabled** is set to `true`.</span></span> <span data-ttu-id="494f2-153">В этом случае решения применяются автоматически, как только рецензент завершит обзор доступа или закончится продолжительность обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="494f2-153">In this case, decisions are applied automatically once the reviewer completes the access review or the access review duration ends.</span></span> <span data-ttu-id="494f2-154">Если он не включен, пользователь должен после завершения проверки применять решения вручную.</span><span class="sxs-lookup"><span data-stu-id="494f2-154">If not enabled, a user must, after the review completes, apply the decisions manually.</span></span>
+ <span data-ttu-id="494f2-155">Применить **действие removeAccessApplyAction** для отклонить гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="494f2-155">Apply **removeAccessApplyAction** action to denied guest users.</span></span> <span data-ttu-id="494f2-156">Это удаляет членство в группе отклоненного гостя.</span><span class="sxs-lookup"><span data-stu-id="494f2-156">This removes the membership in the group of the denied guest.</span></span> <span data-ttu-id="494f2-157">Гостевой пользователь по-прежнему может войти в клиент.</span><span class="sxs-lookup"><span data-stu-id="494f2-157">The guest user can still sign in to your tenant.</span></span>

### <a name="request"></a><span data-ttu-id="494f2-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-158">Request</span></span>
<span data-ttu-id="494f2-159">В этом вызове замените следующее:</span><span class="sxs-lookup"><span data-stu-id="494f2-159">In this call, replace the following:</span></span>

+ <span data-ttu-id="494f2-160">`c9a5aff7-9298-4d71-adab-0a222e0a05e4` с **ид пользователя,** назначенного в качестве резервного рецензента.</span><span class="sxs-lookup"><span data-stu-id="494f2-160">`c9a5aff7-9298-4d71-adab-0a222e0a05e4` with the **id** of the user you are designating as a backup reviewer.</span></span> <span data-ttu-id="494f2-161">Это **id из** ответа в шаге 1.</span><span class="sxs-lookup"><span data-stu-id="494f2-161">This is the **id** from the response in Step 1.</span></span>
+ <span data-ttu-id="494f2-162">Значение **startDate с** сегодняшней датой и **значением endDate** с датой один год с даты начала.</span><span class="sxs-lookup"><span data-stu-id="494f2-162">Value of **startDate** with today's date and value of **endDate** with a date one year from the start date.</span></span> 

```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "backupReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

### <a name="response"></a><span data-ttu-id="494f2-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-163">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
    "id": "c22ae540-b89a-4d24-bac0-4ef35e6591ea",
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "status": "NotStarted",
    "createdBy": {
        "id": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "backupReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

## <a name="step-5-list-instances-of-the-access-review"></a><span data-ttu-id="494f2-164">Шаг 5. Список экземпляров обзора доступа</span><span class="sxs-lookup"><span data-stu-id="494f2-164">Step 5: List instances of the access review</span></span>

<span data-ttu-id="494f2-165">В следующем запросе перечислены все экземпляры определения обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="494f2-165">The following query lists all instances of the access review definition.</span></span> <span data-ttu-id="494f2-166">Если клиент тестирования содержит другие группы Microsoft 365 с гостевых пользователей, этот запрос возвращает один экземпляр для каждой группы Microsoft 365 с гостевых пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="494f2-166">If your test tenant contains other Microsoft 365 groups with guest users, this request will return one instance for every Microsoft 365 group with guest users in the tenant.</span></span>

### <a name="request"></a><span data-ttu-id="494f2-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-167">Request</span></span>
<span data-ttu-id="494f2-168">В этом вызове `c22ae540-b89a-4d24-bac0-4ef35e6591ea` замените **id** определения обзора доступа, возвращенного в шаге 4.</span><span class="sxs-lookup"><span data-stu-id="494f2-168">In this call, replace `c22ae540-b89a-4d24-bac0-4ef35e6591ea` with the **id** of your access review definition returned in Step 4.</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a><span data-ttu-id="494f2-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-169">Response</span></span>
<span data-ttu-id="494f2-170">В этом ответе область включает группу с **id** (группа маркетинговой кампании `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` **Feelgood,** созданная в шаге 3), так как у нее есть гость.</span><span class="sxs-lookup"><span data-stu-id="494f2-170">In this response, the scope includes a group with **id** `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` (the **Feelgood marketing campaign** group created in Step 3) because it has a guest user.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances",
    "value": [
        {
            "id": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "startDateTime": "2021-02-10T17:00:36.96Z",
            "endDateTime": "2021-02-10T17:00:36.96Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```
<span data-ttu-id="494f2-171">В этом ответе экземпляр проверки доступа в настоящее время `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="494f2-171">In this response, the access review instance is currently `InProgress`.</span></span> <span data-ttu-id="494f2-172">Поскольку это ежеквартный обзор, каждые 3 месяца новый экземпляр обзора создается автоматически, и вы — рецензент — можете применять новые решения.</span><span class="sxs-lookup"><span data-stu-id="494f2-172">Because this is a quarterly review, every 3 months, a new review instance is created automatically and you—the reviewer—can apply new decisions.</span></span>

## <a name="step-6-get-decisions"></a><span data-ttu-id="494f2-173">Шаг 6. Принятие решений</span><span class="sxs-lookup"><span data-stu-id="494f2-173">Step 6: Get decisions</span></span>

<span data-ttu-id="494f2-174">Получите решения, принятые в случае проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="494f2-174">Get the decisions taken for the instance of an access review.</span></span>

### <a name="request"></a><span data-ttu-id="494f2-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-175">Request</span></span>
<span data-ttu-id="494f2-176">В этом вызове:</span><span class="sxs-lookup"><span data-stu-id="494f2-176">In this call:</span></span>
+ <span data-ttu-id="494f2-177">`c22ae540-b89a-4d24-bac0-4ef35e6591ea`Замените **id определения** обзора доступа, возвращенного в шаге 4.</span><span class="sxs-lookup"><span data-stu-id="494f2-177">Replace `c22ae540-b89a-4d24-bac0-4ef35e6591ea` with the **id** of your access review definition returned in Step 4.</span></span>
+ <span data-ttu-id="494f2-178">`6392b1a7-9c25-4844-83e5-34e23c88e16a`Замените **id экземпляра** обзора доступа, возвращенного в шаге 5.</span><span class="sxs-lookup"><span data-stu-id="494f2-178">Replace `6392b1a7-9c25-4844-83e5-34e23c88e16a` with the **id** of your access review instance returned in Step 5.</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
```

### <a name="response"></a><span data-ttu-id="494f2-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-179">Response</span></span>

<span data-ttu-id="494f2-180">В следующем ответе показано решение, принятое для экземпляра обзора.</span><span class="sxs-lookup"><span data-stu-id="494f2-180">The following response shows the decision taken for the instance of the review.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances('6392b1a7-9c25-4844-83e5-34e23c88e16a')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "0e76ee07-b4c6-469e-bc9d-e73fc9a8d660",
            "accessReviewId": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "reviewedDateTime": "2021-02-10T17:06:26.147Z",
            "decision": "Approve",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "AAD Access Reviews",
                "userPrincipalName": "AAD Access Reviews"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "userDisplayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "displayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            }
        }
    ]
}
```

<span data-ttu-id="494f2-181">Так как это ежекварточный обзор, и пока определение по-прежнему активно, то есть периодичная дата повторения не является прошлой датой, каждые 3 месяца, когда создается новый экземпляр обзора, вы, как рецензент, можете применять новые решения. </span><span class="sxs-lookup"><span data-stu-id="494f2-181">Because this is a quarterly review and as long as the definition is still active, that is, the recurrence **endDate** is not a past date, every 3 months when a new review instance is created, you as the reviewer can apply new decisions.</span></span>

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="494f2-182">Шаг 7. Очистка ресурсов</span><span class="sxs-lookup"><span data-stu-id="494f2-182">Step 7: Clean up resources</span></span>

<span data-ttu-id="494f2-183">Удалите ресурсы, созданные для этого руководства: группу маркетинговой кампании **Feelgood,** определение расписания обзоров доступа, гостевой пользователь и тестовый пользователь.</span><span class="sxs-lookup"><span data-stu-id="494f2-183">Delete the resources that you created for this tutorial—**Feelgood marketing campaign** group, the access review schedule definition, the guest user, and the test user.</span></span>

### <a name="delete-the-microsoft-365-group"></a><span data-ttu-id="494f2-184">Удаление группы Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="494f2-184">Delete the Microsoft 365 group</span></span>

#### <a name="request"></a><span data-ttu-id="494f2-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-185">Request</span></span>
<span data-ttu-id="494f2-186">В этом вызове замените id маркетинговой кампании `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` **Feelgood** microsoft 365. </span><span class="sxs-lookup"><span data-stu-id="494f2-186">In this call, replace `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` with the **id** of your **Feelgood marketing campaign** Microsoft 365 group.</span></span>

```http
DELETE https://graph.microsoft.com/beta/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a
```

#### <a name="response"></a><span data-ttu-id="494f2-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-187">Response</span></span>

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a><span data-ttu-id="494f2-188">Удаление определения обзора доступа</span><span class="sxs-lookup"><span data-stu-id="494f2-188">Delete the access review definition</span></span>

<span data-ttu-id="494f2-189">В этом вызове `c22ae540-b89a-4d24-bac0-4ef35e6591ea` замените **id** определения обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="494f2-189">In this call, replace `c22ae540-b89a-4d24-bac0-4ef35e6591ea` with the **id** of your access review definition.</span></span> <span data-ttu-id="494f2-190">Так как определение расписания проверки доступа является планом обзора доступа, удаление определения удаляет параметры, экземпляры и решения, связанные с обзором доступа.</span><span class="sxs-lookup"><span data-stu-id="494f2-190">Since the access review schedule definition is the blueprint for the access review, deleting the definition will remove the settings, instances, and decisions associated with the access review.</span></span>

#### <a name="request"></a><span data-ttu-id="494f2-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-191">Request</span></span>
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
```

#### <a name="response"></a><span data-ttu-id="494f2-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-192">Response</span></span>
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```
### <a name="remove-the-guest-user"></a><span data-ttu-id="494f2-193">Удаление гостевого пользователя</span><span class="sxs-lookup"><span data-stu-id="494f2-193">Remove the guest user</span></span>

<span data-ttu-id="494f2-194">В этом вызове `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` замените **id** гостевого пользователя john@tailspintoys.com.</span><span class="sxs-lookup"><span data-stu-id="494f2-194">In this call, replace `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` with the **id** of the guest user, john@tailspintoys.com.</span></span>

#### <a name="request"></a><span data-ttu-id="494f2-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-195">Request</span></span>
```http
DELETE https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20
```

#### <a name="response"></a><span data-ttu-id="494f2-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-196">Response</span></span>
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-test-user"></a><span data-ttu-id="494f2-197">Удаление тестового пользователя</span><span class="sxs-lookup"><span data-stu-id="494f2-197">Delete the test user</span></span>

#### <a name="request"></a><span data-ttu-id="494f2-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="494f2-198">Request</span></span>
<span data-ttu-id="494f2-199">В этом вызове `c9a5aff7-9298-4d71-adab-0a222e0a05e4` замените **id** тестового пользователя.</span><span class="sxs-lookup"><span data-stu-id="494f2-199">In this call, replace `c9a5aff7-9298-4d71-adab-0a222e0a05e4` with the **id** of your test user.</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4
```

#### <a name="response"></a><span data-ttu-id="494f2-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="494f2-200">Response</span></span>

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

<span data-ttu-id="494f2-201">Поздравляем!</span><span class="sxs-lookup"><span data-stu-id="494f2-201">Congratulations!</span></span> <span data-ttu-id="494f2-202">Вы создали обзор доступа для всех гостевых пользователей в группах Microsoft 365 в клиенте и запланирование ежеквартов для оценки и аттестации доступа гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="494f2-202">You have created an access review for all guest users in Microsoft 365 groups in your tenant, and scheduled quarterly for the evaluation and attestation of the guest users' access.</span></span> <span data-ttu-id="494f2-203">Владельцы групп будут пересматривать доступ во время этих циклов, выбирая утверждение или отказ в доступе.</span><span class="sxs-lookup"><span data-stu-id="494f2-203">The group owners will review access during these cycles, choosing either to approve or deny access.</span></span>

## <a name="see-also"></a><span data-ttu-id="494f2-204">См. также</span><span class="sxs-lookup"><span data-stu-id="494f2-204">See also</span></span>

+ [<span data-ttu-id="494f2-205">Обзор обзоров доступа и требования к лицензиям</span><span class="sxs-lookup"><span data-stu-id="494f2-205">Access Reviews overview and license requirements</span></span>](/azure/active-directory/governance/access-reviews-overview)
+ [<span data-ttu-id="494f2-206">Сценарии лицензии Access Reviews</span><span class="sxs-lookup"><span data-stu-id="494f2-206">Access Reviews license scenarios</span></span>](/azure/active-directory/governance/access-reviews-overview#example-license-scenarios)
+ [<span data-ttu-id="494f2-207">Создание обзора доступа групп & приложений</span><span class="sxs-lookup"><span data-stu-id="494f2-207">Create an access review of groups & applications</span></span>](/azure/active-directory/governance/create-access-review)
+ [<span data-ttu-id="494f2-208">Приглашение и добавление гостевых пользователей в организацию</span><span class="sxs-lookup"><span data-stu-id="494f2-208">Invite/add guest users to your organization</span></span>](/graph/api/resources/invitation?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="494f2-209">Ссылка на API обзоров доступа</span><span class="sxs-lookup"><span data-stu-id="494f2-209">Access Reviews API Reference</span></span>](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="494f2-210">Создание accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="494f2-210">Create accessReviewScheduleDefinition</span></span>](/graph/api/accessreviewscheduledefinition-create?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="494f2-211">List accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="494f2-211">List accessReviewInstance</span></span>](/graph/api/accessreviewinstance-list?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="494f2-212">List accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="494f2-212">List accessReviewInstanceDecisionItem</span></span>](/graph/api/accessreviewinstancedecisionitem-list?view=graph-rest-beta&preserve-view=true)

