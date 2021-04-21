---
title: Руководство. Используйте API обзоров доступа для просмотра доступа к группам безопасности
description: Используйте API обзоров доступа для просмотра доступа к группам безопасности
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: bc8796bee1297e125ad287d5151c709cf58fb222
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921091"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-your-security-groups"></a><span data-ttu-id="06d05-103">Руководство. Используйте API обзоров доступа для просмотра доступа к группам безопасности</span><span class="sxs-lookup"><span data-stu-id="06d05-103">Tutorial: Use the access reviews API to review access to your security groups</span></span>

<span data-ttu-id="06d05-104">В этом руководстве вы будете использовать Graph Explorer для просмотра доступа к группе безопасности в клиенте.</span><span class="sxs-lookup"><span data-stu-id="06d05-104">In this tutorial, you will use Graph Explorer to review access to a security group in your tenant.</span></span>

<span data-ttu-id="06d05-105">Вы можете использовать Graph Explorer или Postman для проверки звонков API отзывов доступа, прежде чем автоматизировать их в скрипт или приложение.</span><span class="sxs-lookup"><span data-stu-id="06d05-105">You can use Graph Explorer or Postman to try out and test your access reviews API calls before you automate them into a script or an app.</span></span> <span data-ttu-id="06d05-106">Это экономит время, помогая правильно определять и проверять запросы без повторнойкомпилации приложения.</span><span class="sxs-lookup"><span data-stu-id="06d05-106">This saves you time by helping you properly define and validate your queries without repeatedly recompiling your application.</span></span>

>[!NOTE]
><span data-ttu-id="06d05-107">Объекты отклика, показанные в этом руководстве, могут быть сокращены для чтения.</span><span class="sxs-lookup"><span data-stu-id="06d05-107">The response objects shown in this tutorial might be shortened for readability.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06d05-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="06d05-108">Prerequisites</span></span>

<span data-ttu-id="06d05-109">Для завершения этого руководства необходимы следующие ресурсы и привилегии:</span><span class="sxs-lookup"><span data-stu-id="06d05-109">To complete this tutorial, you need the following resources and privileges:</span></span>

+ <span data-ttu-id="06d05-110">Рабочий клиент Azure AD с включенной лицензией Azure AD Premium P2 или EMS E5.</span><span class="sxs-lookup"><span data-stu-id="06d05-110">A working Azure AD tenant with an Azure AD Premium P2 or EMS E5 license enabled.</span></span>
+ <span data-ttu-id="06d05-111">Войдите в [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) как пользователь в роли глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="06d05-111">Log in to [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) as a user in a global administrator role.</span></span>
  + <span data-ttu-id="06d05-112">[Необязательный] Запустите новое **инкогнито** или **сеанс браузера InPrivate** или запустите сеанс в анонимном браузере.</span><span class="sxs-lookup"><span data-stu-id="06d05-112">[Optional] Start a new **incognito** or **InPrivate browser** session or start a session in an anonymous browser.</span></span> <span data-ttu-id="06d05-113">Вы войдите позже в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="06d05-113">You will log in later in this tutorial.</span></span>
+ <span data-ttu-id="06d05-114">Следующие делегированные разрешения: `AccessReview.ReadWrite.All` , `Group.ReadWrite.All` .</span><span class="sxs-lookup"><span data-stu-id="06d05-114">The following delegated permissions: `AccessReview.ReadWrite.All`, `Group.ReadWrite.All`.</span></span>

<span data-ttu-id="06d05-115">Согласие на необходимые разрешения в Graph Explorer:</span><span class="sxs-lookup"><span data-stu-id="06d05-115">To consent to the required permissions in Graph Explorer:</span></span>
1. <span data-ttu-id="06d05-116">Выберите значок передач параметров справа от сведений учетной записи пользователя, а затем выберите **выберите разрешения.**</span><span class="sxs-lookup"><span data-stu-id="06d05-116">Select the settings gear icon to the right of the user account details, and then select **Select permissions**.</span></span>
   
   <span data-ttu-id="06d05-117">![Выбор разрешений Microsoft Graph](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
   </span><span class="sxs-lookup"><span data-stu-id="06d05-117">![Select the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Select the Microsoft Graph permissions":::-->

2. <span data-ttu-id="06d05-118">Прокрутите список разрешений для этих разрешений:</span><span class="sxs-lookup"><span data-stu-id="06d05-118">Scroll through the list of permissions to these permissions:</span></span>
   + <span data-ttu-id="06d05-119">AccessReviews (3), расширяйте и выберите **AccessReviews.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="06d05-119">AccessReviews (3), expand and then select **AccessReviews.ReadWrite.All**.</span></span>
   + <span data-ttu-id="06d05-120">Группа (2), развиньте и выберите **Group.ReadWrite.All**.</span><span class="sxs-lookup"><span data-stu-id="06d05-120">Group (2), expand and then select **Group.ReadWrite.All**.</span></span>
  
    <span data-ttu-id="06d05-121">Выберите **Согласие** и в всплывающее  окно выберите Согласие от имени организации, а затем выберите **Accept,** чтобы принять согласие разрешений.</span><span class="sxs-lookup"><span data-stu-id="06d05-121">Select **Consent**, and in the pop window, choose to **Consent on behalf of your organization** and then select **Accept** to accept the consent of the permissions.</span></span>
   
   <span data-ttu-id="06d05-122">![Согласие на разрешения Microsoft Graph](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png)
   </span><span class="sxs-lookup"><span data-stu-id="06d05-122">![Consent to the Microsoft Graph permissions](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png)
</span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png" alt-text="Consent to the Microsoft Graph permissions":::-->

## <a name="step-1-create-test-users-in-your-tenant"></a><span data-ttu-id="06d05-123">Шаг 1. Создание тестовых пользователей в клиенте</span><span class="sxs-lookup"><span data-stu-id="06d05-123">Step 1: Create test users in your tenant</span></span>

<span data-ttu-id="06d05-124">Создайте трех новых тестовых пользователей, каждый раз запуская запрос ниже, меняя свойства **displayName,** **mailNickname** и **userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="06d05-124">Create three new test users by running the request below three times, changing the **displayName**, **mailNickname**, and **userPrincipalName** properties each time.</span></span> <span data-ttu-id="06d05-125">Запись **их id** s.</span><span class="sxs-lookup"><span data-stu-id="06d05-125">Record their **id** s.</span></span>

### <a name="request"></a><span data-ttu-id="06d05-126">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d05-126">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="06d05-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d05-127">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "43b12b0c-ee2c-4257-96fe-505d823e06ab",
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-create-a-security-group-assign-owners-and-add-members"></a><span data-ttu-id="06d05-128">Шаг 2. Создание группы безопасности, назначение владельцев и добавление участников</span><span class="sxs-lookup"><span data-stu-id="06d05-128">Step 2: Create a security group, assign owners, and add members</span></span>

<span data-ttu-id="06d05-129">Создайте группу безопасности с именем **Building security group,** которая является целью обзоров доступа в этом руководстве.</span><span class="sxs-lookup"><span data-stu-id="06d05-129">Create a security group named **Building security group** that is the target of the access reviews in this tutorial.</span></span> <span data-ttu-id="06d05-130">Назначьте этой группе двух владельцев групп и двух участников.</span><span class="sxs-lookup"><span data-stu-id="06d05-130">Assign to this group two group owners and two members.</span></span> <span data-ttu-id="06d05-131">Эти члены будут подвергаться проверке со стороны владельцев групп.</span><span class="sxs-lookup"><span data-stu-id="06d05-131">These members will be the subject of review by the group owners.</span></span>

### <a name="request"></a><span data-ttu-id="06d05-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d05-132">Request</span></span>
<span data-ttu-id="06d05-133">В этом вызове замените:</span><span class="sxs-lookup"><span data-stu-id="06d05-133">In this call, replace:</span></span>
+ <span data-ttu-id="06d05-134">`010b2de0-0ed4-4ece-bfa2-22fff71d0497` и `b828cc0e-4240-46ed-bb25-888744487e2d` с **id** s двух владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="06d05-134">`010b2de0-0ed4-4ece-bfa2-22fff71d0497` and `b828cc0e-4240-46ed-bb25-888744487e2d` with the **id** s of your two group owners.</span></span>
  + <span data-ttu-id="06d05-135">Один из **id** s принадлежит одному из пользователей, созданных в шаге 1.</span><span class="sxs-lookup"><span data-stu-id="06d05-135">One of the **id** s belongs to one of the users you created in Step 1.</span></span>
  + <span data-ttu-id="06d05-136">Другой — ваш **id**. Чтобы получить свой **id,** `GET` запустите `https://graph.microsoft.com/beta/me` .</span><span class="sxs-lookup"><span data-stu-id="06d05-136">The other is your **id**. To retrieve your **id**, run `GET` on `https://graph.microsoft.com/beta/me`.</span></span>
+ <span data-ttu-id="06d05-137">`43b12b0c-ee2c-4257-96fe-505d823e06ab` и `859924d0-7115-422a-9ee8-ea8c0c014707` с **id** s из вас два члена группы.</span><span class="sxs-lookup"><span data-stu-id="06d05-137">`43b12b0c-ee2c-4257-96fe-505d823e06ab` and `859924d0-7115-422a-9ee8-ea8c0c014707` with the **id** s of you two group members.</span></span> <span data-ttu-id="06d05-138">Это два других члена, созданные в шаге 1.</span><span class="sxs-lookup"><span data-stu-id="06d05-138">These are the other two members you created in Step 1.</span></span>

```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
    "description": "Building security group",
    "displayName": "Building security group",
    "groupTypes": [],
    "mailEnabled": false,
    "mailNickname": "buildingsecurity",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/010b2de0-0ed4-4ece-bfa2-22fff71d0497",
        "https://graph.microsoft.com/beta/users/b828cc0e-4240-46ed-bb25-888744487e2d"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/43b12b0c-ee2c-4257-96fe-505d823e06ab",
        "https://graph.microsoft.com/beta/users/859924d0-7115-422a-9ee8-ea8c0c014707"
    ]
}
```

### <a name="response"></a><span data-ttu-id="06d05-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d05-139">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "825f1b5e-6fb2-4d9a-b393-d491101acc0c",
    "displayName": "Building security group",
    "groupTypes": []
}
```
<span data-ttu-id="06d05-140">В ответе зафиксировать **id** новой группы, чтобы использовать его позже в этом учебнике.</span><span class="sxs-lookup"><span data-stu-id="06d05-140">From the response, record the **id** of the new group to use it later in this tutorial.</span></span>

## <a name="step-3-create-an-access-review"></a><span data-ttu-id="06d05-141">Шаг 3. Создание обзора доступа</span><span class="sxs-lookup"><span data-stu-id="06d05-141">Step 3: Create an access review</span></span>

<span data-ttu-id="06d05-142">Создайте обзор доступа для членов группы безопасности с помощью следующих параметров:</span><span class="sxs-lookup"><span data-stu-id="06d05-142">Create an access review for members of the security group, using the following settings:</span></span>
+ <span data-ttu-id="06d05-143">Это обзор самостоятельного просмотра доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-143">It is a self-reviewing access review.</span></span> <span data-ttu-id="06d05-144">В этом случае проверяемая пользовательская группа самостоятельно засвидетельна необходимостью доступа к группе.</span><span class="sxs-lookup"><span data-stu-id="06d05-144">In this case, users under review will self-attest to their need for access to the group.</span></span>
+ <span data-ttu-id="06d05-145">Это разовая проверка доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-145">This is a one-time access review.</span></span> <span data-ttu-id="06d05-146">В этом случае после предоставления доступа пользователю не нужно повторно засвидетельстовка в течение периода проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-146">In this case, once access is granted, the user does not need to self-attest again within the access review period.</span></span>
+ <span data-ttu-id="06d05-147">Область обзора ограничена членами **группы безопасности Building.**</span><span class="sxs-lookup"><span data-stu-id="06d05-147">The review scope is limited to members of **Building security group**.</span></span>

### <a name="request"></a><span data-ttu-id="06d05-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d05-148">Request</span></span>
<span data-ttu-id="06d05-149">В этом вызове замените следующее:</span><span class="sxs-lookup"><span data-stu-id="06d05-149">In this call, replace the following:</span></span>
+ <span data-ttu-id="06d05-150">`825f1b5e-6fb2-4d9a-b393-d491101acc0c` с **id** группы **безопасности Здания**.</span><span class="sxs-lookup"><span data-stu-id="06d05-150">`825f1b5e-6fb2-4d9a-b393-d491101acc0c` with the **id** of **Building security group**.</span></span>
+ <span data-ttu-id="06d05-151">Значение **startDate с** сегодняшней датой и **значением endDate** с датой один год с даты начала.</span><span class="sxs-lookup"><span data-stu-id="06d05-151">Value of **startDate** with today's date and value of **endDate** with a date one year from the start date.</span></span>

<span data-ttu-id="06d05-152">Если не указать значение  свойства рецензентов, этот обзор доступа настраивается как самообсчет с участниками в качестве рецензентов.</span><span class="sxs-lookup"><span data-stu-id="06d05-152">By failing to specify the value of the **reviewers** property, this access review is configured as self-reviewing with the members as the reviewers.</span></span>

```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "One-time self-review for members of Building security group",
    "descriptionForAdmins": "One-time self-review for members of Building security group",
    "descriptionForReviewers": "One-time self-review for members of Building security group",
    "scope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-09",
                "endDate": "2022-12-31"
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

### <a name="response"></a><span data-ttu-id="06d05-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d05-153">Response</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
    "id": "d7286a17-3a01-406a-b872-986b6b40317c",
    "displayName": "One-time self-review for members of Building security group",
    "status": "NotStarted",
    "createdBy": {
        "id": "b828cc0e-4240-46ed-bb25-888744487e2d",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "backupReviewers": [],
    "settings": {
        "defaultDecisionEnabled": false,
        "defaultDecision": "Deny",
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-09",
                "endDate": "2022-12-31"
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

## <a name="step-4-list-instances-of-the-access-review"></a><span data-ttu-id="06d05-154">Шаг 4. Список экземпляров обзора доступа</span><span class="sxs-lookup"><span data-stu-id="06d05-154">Step 4: List instances of the access review</span></span>

<span data-ttu-id="06d05-155">В следующем запросе перечислены все экземпляры определения обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-155">The following query lists all instances of the access review definition.</span></span> <span data-ttu-id="06d05-156">Так как в шаге 3 был создан разовая проверка доступа, запрос возвращает только один экземпляр, **id** которого является таким же, как и **id определения доступа.**</span><span class="sxs-lookup"><span data-stu-id="06d05-156">Because you created a one-time access review in Step 3, the request returns only one instance whose **id** is the same as the access definition’s **id**.</span></span>

### <a name="request"></a><span data-ttu-id="06d05-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d05-157">Request</span></span>
<span data-ttu-id="06d05-158">В этом вызове `d7286a17-3a01-406a-b872-986b6b40317c` замените **id** определения обзора доступа, возвращенного в шаге 3.</span><span class="sxs-lookup"><span data-stu-id="06d05-158">In this call, replace `d7286a17-3a01-406a-b872-986b6b40317c` with the **id** of your access review definition returned in Step 3.</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/d7286a17-3a01-406a-b872-986b6b40317c/instances
```

### <a name="response"></a><span data-ttu-id="06d05-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d05-159">Response</span></span>

<span data-ttu-id="06d05-160">В этом ответе **состояние экземпляра** проверки доступа в том, что `InProgress` **startDateTime** прошло, **а endDateTime** — в будущем.</span><span class="sxs-lookup"><span data-stu-id="06d05-160">In this response, the **status** of the access review instance is `InProgress` because **startDateTime** is past and **endDateTime** is in the future.</span></span> <span data-ttu-id="06d05-161">Если **startDateTime** будет в будущем, состояние будет `NotStarted` .</span><span class="sxs-lookup"><span data-stu-id="06d05-161">If **startDateTime** is in the future, the status will be `NotStarted`.</span></span> <span data-ttu-id="06d05-162">С другой стороны, если **endDateTime** в прошлом, состояние будет `Completed` .</span><span class="sxs-lookup"><span data-stu-id="06d05-162">On the other hand, if **endDateTime** is in the past, the status will be `Completed`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('d7286a17-3a01-406a-b872-986b6b40317c')/instances",
    "value": [
        {
            "id": "d7286a17-3a01-406a-b872-986b6b40317c",
            "startDateTime": "2021-02-10T15:09:40.153Z",
            "endDateTime": "2022-12-31T08:00:00Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```

## <a name="step-5-get-decisions"></a><span data-ttu-id="06d05-163">Шаг 5. Принятие решений</span><span class="sxs-lookup"><span data-stu-id="06d05-163">Step 5: Get decisions</span></span>

<span data-ttu-id="06d05-164">Вас интересуют решения, принятые в экземпляре обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-164">You are interested in the decisions taken for the instance of the access review.</span></span>

### <a name="request"></a><span data-ttu-id="06d05-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d05-165">Request</span></span>
<span data-ttu-id="06d05-166">В этом вызове `d7286a17-3a01-406a-b872-986b6b40317c` замените **id** определения обзора доступа, возвращенного в шаге 3.</span><span class="sxs-lookup"><span data-stu-id="06d05-166">In this call, replace `d7286a17-3a01-406a-b872-986b6b40317c` with the **id** of your access review definition returned in Step 3.</span></span>

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/d7286a17-3a01-406a-b872-986b6b40317c/instances/d7286a17-3a01-406a-b872-986b6b40317c/decisions
```

### <a name="response"></a><span data-ttu-id="06d05-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d05-167">Response</span></span>

<span data-ttu-id="06d05-168">В следующем ответе показано решение, принятое для экземпляра обзора.</span><span class="sxs-lookup"><span data-stu-id="06d05-168">The following response shows the decision taken for the instance of the review.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('d7286a17-3a01-406a-b872-986b6b40317c')/instances('d7286a17-3a01-406a-b872-986b6b40317c')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "1c74f500-9082-4dfe-80ac-784a6edb71d7",
            "accessReviewId": "d7286a17-3a01-406a-b872-986b6b40317c",
            "decision": "NotReviewed",
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "43b12b0c-ee2c-4257-96fe-505d823e06ab",
                "userDisplayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "43b12b0c-ee2c-4257-96fe-505d823e06ab",
                "displayName": "Alex Wilber",
                "userPrincipalName": "AlexW@contoso.com"
            }
        },
        {
            "id": "7744be81-7d17-40c9-8fd3-c9072b1ccace",
            "accessReviewId": "d7286a17-3a01-406a-b872-986b6b40317c",
            "decision": "NotReviewed",
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "859924d0-7115-422a-9ee8-ea8c0c014707",
                "userDisplayName": "Allan Deyoung",
                "userPrincipalName": "AllanD@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "859924d0-7115-422a-9ee8-ea8c0c014707",
                "displayName": "Allan Deyoung",
                "userPrincipalName": "AllanD@contoso.com"
            }
        }
    ]
}
```

<span data-ttu-id="06d05-169">По вызову свойство **decision** имеет значение `NotReviewed` .</span><span class="sxs-lookup"><span data-stu-id="06d05-169">From the call, the **decision** property has the value of `NotReviewed`.</span></span> <span data-ttu-id="06d05-170">Это потому, что ни один из двух участников не завершил самоаттестацию.</span><span class="sxs-lookup"><span data-stu-id="06d05-170">This is because none of the two members has completed their self-attestation.</span></span> <span data-ttu-id="06d05-171">Следуйте шагу 6, чтобы узнать, как каждый член может самостоятельно подтвердить свою потребность в просмотре доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-171">Follow step 6 to learn how each member can self-attest to their need for access review.</span></span>

## <a name="step-6-self-review-your-pending-access"></a><span data-ttu-id="06d05-172">Шаг 6. Самостоятельное рассмотрение ожидающих доступа</span><span class="sxs-lookup"><span data-stu-id="06d05-172">Step 6: Self-review your pending access</span></span>

<span data-ttu-id="06d05-173">На шаге 3 вы настраивали обзор доступа в качестве самостоятельного просмотра.</span><span class="sxs-lookup"><span data-stu-id="06d05-173">In Step 3, you configured the access review as a self-reviewing.</span></span> <span data-ttu-id="06d05-174">Это означает, что оба члена **группы безопасности здания** должны самостоятельно подтвердить свою необходимость сохранения доступа к группе.</span><span class="sxs-lookup"><span data-stu-id="06d05-174">This means that both members of **Building security group** must self-attest to their need to maintain access to the group.</span></span> <span data-ttu-id="06d05-175">Вы выполните этот шаг в качестве одного из двух членов группы безопасности здания.</span><span class="sxs-lookup"><span data-stu-id="06d05-175">You will complete this step as one of the two members of Building security group.</span></span>

<span data-ttu-id="06d05-176">In this step, you will:</span><span class="sxs-lookup"><span data-stu-id="06d05-176">In this step, you will:</span></span>
1. <span data-ttu-id="06d05-177">Список ожидающих экземпляров проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-177">List your pending access review instances.</span></span>
2. <span data-ttu-id="06d05-178">Завершите процесс самоаттестации проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-178">Complete the access review self-attestation process.</span></span>

<span data-ttu-id="06d05-179">Запустите новый сеанс браузера в режиме **инкогнито** или **в режиме просмотра InPrivate** или с помощью анонимного браузера и войдите в систему в качестве одного из двух членов группы безопасности **Building.**</span><span class="sxs-lookup"><span data-stu-id="06d05-179">Start a new browser session in **incognito** or **InPrivate browsing** mode, or via an anonymous browser, and log in as one of the two members of **Building security group**.</span></span> <span data-ttu-id="06d05-180">Таким образом, вы не перебиваете текущий сеанс в качестве пользователя в роли глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="06d05-180">By doing so, you will not interrupt your current session as a user in the global administrator role.</span></span> <span data-ttu-id="06d05-181">Кроме того, можно прервать текущий сеанс, выйдя из Graph Explorer и войдя в систему в качестве одного из двух участников группы.</span><span class="sxs-lookup"><span data-stu-id="06d05-181">Alternatively, you can interrupt your current session by logging out of Graph Explorer and logging back in as one of the two group members.</span></span>

### <a name="list-your-pending-access-review-instances"></a><span data-ttu-id="06d05-182">Список ожидающих экземпляров проверки доступа</span><span class="sxs-lookup"><span data-stu-id="06d05-182">List your pending access review instances</span></span>

<span data-ttu-id="06d05-183">В сеансе браузера инкогнито и в Graph Explorer запустите следующий запрос, чтобы перечислить ожидающий экземпляры обзора доступа:</span><span class="sxs-lookup"><span data-stu-id="06d05-183">In the incognito browser session and in Graph Explorer, run the following query to list your pending access review instances:</span></span>

#### <a name="request"></a><span data-ttu-id="06d05-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d05-184">Request</span></span>

```http
GET /me/pendingAccessReviewInstances
```

#### <a name="response"></a><span data-ttu-id="06d05-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d05-185">Response</span></span>
<span data-ttu-id="06d05-186">В ответе ниже пользователь Alex Wilber из **id** имеет 1 ожидающих просмотра доступа к `43b12b0c-ee2c-4257-96fe-505d823e06ab` самостоятельной проверке.</span><span class="sxs-lookup"><span data-stu-id="06d05-186">From the response below, user Alex Wilber of **id** `43b12b0c-ee2c-4257-96fe-505d823e06ab` has 1 pending access review to self-attest to.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('43b12b0c-ee2c-4257-96fe-505d823e06ab')/pendingAccessReviewInstances",
    "@odata.count": 1,
    "value": [
        {
            "id": "d7286a17-3a01-406a-b872-986b6b40317c",
            "startDateTime": "2021-02-10T15:09:40.153Z",
            "endDateTime": "2022-12-31T08:00:00Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c/transitiveMembers",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```
<span data-ttu-id="06d05-187">Использование вызова `/me/pendingAccessReviewInstances` в пользовательском контексте имеет ряд преимуществ:</span><span class="sxs-lookup"><span data-stu-id="06d05-187">Using the call `/me/pendingAccessReviewInstances` in a user context has a number of advantages:</span></span>
+ <span data-ttu-id="06d05-188">Не требуется руководитель службы.</span><span class="sxs-lookup"><span data-stu-id="06d05-188">No service principal is required.</span></span> <span data-ttu-id="06d05-189">Пользователь может звонить и читать ожидающих действий по обзору доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-189">A user can call and read their pending access review actions.</span></span>
+ <span data-ttu-id="06d05-190">Можно использовать виджеты или плагины на странице Интрасети или бот или daemon, которые работают в качестве фоновой службы.</span><span class="sxs-lookup"><span data-stu-id="06d05-190">Can be used by widgets or plugins on an Intranet page, or a bot or daemon that run as a background service.</span></span> <span data-ttu-id="06d05-191">Они могут уведомлять вас о новых отзывах доступа или обновлениях для доступа к отзывам.</span><span class="sxs-lookup"><span data-stu-id="06d05-191">These can notify you of new access reviews or of updates to access reviews.</span></span> 

### <a name="complete-the-access-review-self-attestation"></a><span data-ttu-id="06d05-192">Завершение самоаттестации проверки доступа</span><span class="sxs-lookup"><span data-stu-id="06d05-192">Complete the access review self-attestation</span></span>

<span data-ttu-id="06d05-193">В том же сеансе инкогнито браузера войдите, чтобы https://myaccess.microsoft.com/ завершить самоаттестацию.</span><span class="sxs-lookup"><span data-stu-id="06d05-193">In the same incognito browser session, log in to https://myaccess.microsoft.com/ to complete the self-attestation.</span></span> <span data-ttu-id="06d05-194">В правой панели навигации выберите **отзывы о доступе** и выберите обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-194">From the right navigation bar, select **access reviews** and choose your access review.</span></span> <span data-ttu-id="06d05-195">Выберите **Да,** что вам по-прежнему необходим доступ к **группе безопасности здания,** введите причину, а затем нажмите **отправить**.</span><span class="sxs-lookup"><span data-stu-id="06d05-195">Select **Yes**, that you still need access to **Building security group**, enter a reason, then click **Submit**.</span></span>

   <span data-ttu-id="06d05-196">![Самооценка доступа к обзору](../images/../concepts/images/tutorial-accessreviews-api/selfattest.png)
   </span><span class="sxs-lookup"><span data-stu-id="06d05-196">![Self-attest to access review](../images/../concepts/images/tutorial-accessreviews-api/selfattest.png)
   </span></span><!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/selfattest.png" alt-text="Self-attest to access review":::-->

<span data-ttu-id="06d05-197">Теперь вы можете выйти из сеанса браузера инкогнито и выйти из него.</span><span class="sxs-lookup"><span data-stu-id="06d05-197">You can now logout and exit the incognito browser session.</span></span>

<span data-ttu-id="06d05-198">Возвращаясь к основному сеансу браузера, в котором вы все еще входите  в качестве пользователя глобального администратора, повторите шаг 4, чтобы увидеть, что свойство решения для участника, завершившего шаг 5, теперь `Approve` .</span><span class="sxs-lookup"><span data-stu-id="06d05-198">Back in the main browser session where you are still logged in as the global administrator user, repeat Step 4 to see that the **decision** property for the member who completed step 5 is now `Approve`.</span></span>

<span data-ttu-id="06d05-199">Поздравляем!</span><span class="sxs-lookup"><span data-stu-id="06d05-199">Congratulations!</span></span> <span data-ttu-id="06d05-200">Вы создали обзор доступа и самостоятельно засвидетельстили необходимость доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-200">You have created an access review and self-attested to the need for access.</span></span> <span data-ttu-id="06d05-201">Это можно сделать только один раз и сохранить доступ до истечения срока действия определения проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-201">You only do this once, and maintain access until when the access review definition expires.</span></span>

## <a name="step-7-clean-up-resources"></a><span data-ttu-id="06d05-202">Шаг 7. Очистка ресурсов</span><span class="sxs-lookup"><span data-stu-id="06d05-202">Step 7: Clean up resources</span></span>

<span data-ttu-id="06d05-203">Удалите ресурсы, созданные для этого **руководства:** создание группы безопасности, определение расписания проверки доступа и три тестовых пользователя.</span><span class="sxs-lookup"><span data-stu-id="06d05-203">Delete the resources that you created for this tutorial—**Building security group**, the access review schedule definition, and the three test users..</span></span>

### <a name="delete-the-security-group"></a><span data-ttu-id="06d05-204">Удаление группы безопасности</span><span class="sxs-lookup"><span data-stu-id="06d05-204">Delete the security group</span></span>

#### <a name="request"></a><span data-ttu-id="06d05-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d05-205">Request</span></span>
<span data-ttu-id="06d05-206">В этом вызове `825f1b5e-6fb2-4d9a-b393-d491101acc0c` замените **id** группы **безопасности Building.**</span><span class="sxs-lookup"><span data-stu-id="06d05-206">In this call, replace `825f1b5e-6fb2-4d9a-b393-d491101acc0c` with the **id** of **Building security group**.</span></span>

```http
DELETE https://graph.microsoft.com/beta/groups/825f1b5e-6fb2-4d9a-b393-d491101acc0c
```

#### <a name="response"></a><span data-ttu-id="06d05-207">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d05-207">Response</span></span>

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a><span data-ttu-id="06d05-208">Удаление определения обзора доступа</span><span class="sxs-lookup"><span data-stu-id="06d05-208">Delete the access review definition</span></span>

<span data-ttu-id="06d05-209">В этом вызове `d7286a17-3a01-406a-b872-986b6b40317c` замените **id** определения обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-209">In this call, replace `d7286a17-3a01-406a-b872-986b6b40317c` with the **id** of your access review definition.</span></span> <span data-ttu-id="06d05-210">Так как определение расписания проверки доступа является планом обзора доступа, удаление определения удаляет параметры, экземпляры и решения, связанные с обзором доступа.</span><span class="sxs-lookup"><span data-stu-id="06d05-210">Since the access review schedule definition is the blueprint for the access review, deleting the definition will remove the settings, instances, and decisions associated with the access review.</span></span>

#### <a name="request"></a><span data-ttu-id="06d05-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d05-211">Request</span></span>
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/d7286a17-3a01-406a-b872-986b6b40317c
```

#### <a name="response"></a><span data-ttu-id="06d05-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d05-212">Response</span></span>
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-three-test-users"></a><span data-ttu-id="06d05-213">Удаление трех тестовых пользователей</span><span class="sxs-lookup"><span data-stu-id="06d05-213">Delete the three test users</span></span>

#### <a name="request"></a><span data-ttu-id="06d05-214">Запрос</span><span class="sxs-lookup"><span data-stu-id="06d05-214">Request</span></span>
<span data-ttu-id="06d05-215">В этом вызове `43b12b0c-ee2c-4257-96fe-505d823e06ab` замените **id** тестового пользователя.</span><span class="sxs-lookup"><span data-stu-id="06d05-215">In this call, replace `43b12b0c-ee2c-4257-96fe-505d823e06ab` with the **id** of your test user.</span></span> <span data-ttu-id="06d05-216">Повторите это дважды с **помощью id** s двух других пользователей, чтобы удалить их.</span><span class="sxs-lookup"><span data-stu-id="06d05-216">Repeat this twice with the **id** s of the other two users to delete them.</span></span>

```http
DELETE https://graph.microsoft.com/beta/users/43b12b0c-ee2c-4257-96fe-505d823e06ab
```

#### <a name="response"></a><span data-ttu-id="06d05-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="06d05-217">Response</span></span>

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```


## <a name="see-also"></a><span data-ttu-id="06d05-218">См. также</span><span class="sxs-lookup"><span data-stu-id="06d05-218">See also</span></span>

+ [<span data-ttu-id="06d05-219">обзор обзоров доступа и требования к лицензиям</span><span class="sxs-lookup"><span data-stu-id="06d05-219">access reviews overview and license requirements</span></span>](/azure/active-directory/governance/access-reviews-overview)
+ [<span data-ttu-id="06d05-220">отзывы о сценариях лицензии</span><span class="sxs-lookup"><span data-stu-id="06d05-220">access reviews license scenarios</span></span>](/azure/active-directory/governance/access-reviews-overview#example-license-scenarios)
+ [<span data-ttu-id="06d05-221">Создание обзора доступа групп & приложений</span><span class="sxs-lookup"><span data-stu-id="06d05-221">Create an access review of groups & applications</span></span>](/azure/active-directory/governance/create-access-review)
+ [<span data-ttu-id="06d05-222">Ссылка на API отзывов о доступе</span><span class="sxs-lookup"><span data-stu-id="06d05-222">access reviews API Reference</span></span>](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="06d05-223">Создание accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="06d05-223">Create accessReviewScheduleDefinition</span></span>](/graph/api/accessreviewscheduledefinition-create?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="06d05-224">List accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="06d05-224">List accessReviewInstance</span></span>](/graph/api/accessreviewinstance-list?view=graph-rest-beta&preserve-view=true)
+ [<span data-ttu-id="06d05-225">List accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="06d05-225">List accessReviewInstanceDecisionItem</span></span>](/graph/api/accessreviewinstancedecisionitem-list?view=graph-rest-beta&preserve-view=true)

