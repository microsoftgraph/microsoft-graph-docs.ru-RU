---
title: Создание accessReviewScheduleDefinition
description: Создайте новый объект accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: eb63f5720ce9ee7fc21cef2a93ca5a75b742465d
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030483"
---
# <a name="create-accessreviewscheduledefinition"></a><span data-ttu-id="eab2b-103">Создание accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="eab2b-103">Create accessReviewScheduleDefinition</span></span>

<span data-ttu-id="eab2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eab2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eab2b-105">Создайте новый [объект accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eab2b-105">Create a new [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eab2b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eab2b-106">Permissions</span></span>

<span data-ttu-id="eab2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eab2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eab2b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eab2b-109">Permission type</span></span>                        | <span data-ttu-id="eab2b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eab2b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eab2b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eab2b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="eab2b-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eab2b-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="eab2b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eab2b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eab2b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eab2b-114">Not supported.</span></span>|
|<span data-ttu-id="eab2b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="eab2b-115">Application</span></span>                            | <span data-ttu-id="eab2b-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eab2b-116">AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="eab2b-117">При входе пользователь должен также быть в роли каталога, что позволяет им создавать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="eab2b-117">The signed-in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="eab2b-118">Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="eab2b-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="eab2b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eab2b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="eab2b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eab2b-120">Request headers</span></span>
| <span data-ttu-id="eab2b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="eab2b-121">Name</span></span>         | <span data-ttu-id="eab2b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="eab2b-122">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="eab2b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eab2b-123">Authorization</span></span>|<span data-ttu-id="eab2b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eab2b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="eab2b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eab2b-126">Content-type</span></span> | <span data-ttu-id="eab2b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eab2b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eab2b-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eab2b-129">Request body</span></span>
<span data-ttu-id="eab2b-130">В теле запроса поставляем представление JSON объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eab2b-130">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="eab2b-131">В следующей таблице показаны свойства, принятые для создания accessReview.</span><span class="sxs-lookup"><span data-stu-id="eab2b-131">The following table shows the properties accepted to create an accessReview.</span></span>

| <span data-ttu-id="eab2b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="eab2b-132">Property</span></span> | <span data-ttu-id="eab2b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="eab2b-133">Type</span></span> | <span data-ttu-id="eab2b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="eab2b-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eab2b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="eab2b-135">displayName</span></span> | <span data-ttu-id="eab2b-136">String</span><span class="sxs-lookup"><span data-stu-id="eab2b-136">String</span></span> | <span data-ttu-id="eab2b-137">Имя серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="eab2b-137">Name of access review series.</span></span> <span data-ttu-id="eab2b-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eab2b-138">Required.</span></span>|
| <span data-ttu-id="eab2b-139">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="eab2b-139">descriptionForAdmins</span></span> | <span data-ttu-id="eab2b-140">Строка</span><span class="sxs-lookup"><span data-stu-id="eab2b-140">string</span></span> | <span data-ttu-id="eab2b-141">Контекст обзора, предоставленного администраторам.</span><span class="sxs-lookup"><span data-stu-id="eab2b-141">Context of the review provided to admins.</span></span> <span data-ttu-id="eab2b-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eab2b-142">Required.</span></span> |
  <span data-ttu-id="eab2b-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="eab2b-143">descriptionForReviewers</span></span> | <span data-ttu-id="eab2b-144">Строка</span><span class="sxs-lookup"><span data-stu-id="eab2b-144">string</span></span> | <span data-ttu-id="eab2b-145">Контекст обзора, предоставленного рецензентам.</span><span class="sxs-lookup"><span data-stu-id="eab2b-145">Context of the review provided to reviewers.</span></span> <span data-ttu-id="eab2b-146">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eab2b-146">Required.</span></span> |
| <span data-ttu-id="eab2b-147">область</span><span class="sxs-lookup"><span data-stu-id="eab2b-147">scope</span></span> | [<span data-ttu-id="eab2b-148">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="eab2b-148">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="eab2b-149">Определяет область пользователей, рассмотренных в группе.</span><span class="sxs-lookup"><span data-stu-id="eab2b-149">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="eab2b-150">Просмотрите [accessReviewScope и](../resources/accessreviewscheduledefinition.md) узнайте, как настроить область определения обзора [доступа.](/graph/accessreviews-scope-concept)</span><span class="sxs-lookup"><span data-stu-id="eab2b-150">See  [accessReviewScope](../resources/accessreviewscheduledefinition.md) and also learn how to [configure the scope of your access review definition](/graph/accessreviews-scope-concept).</span></span> <span data-ttu-id="eab2b-151">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eab2b-151">Required.</span></span>| 
| <span data-ttu-id="eab2b-152">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="eab2b-152">instanceEnumerationScope</span></span> | [<span data-ttu-id="eab2b-153">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="eab2b-153">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="eab2b-154">В случае проверки всех групп определяется область, в которой будут рассмотрены группы.</span><span class="sxs-lookup"><span data-stu-id="eab2b-154">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="eab2b-155">Просмотрите [accessReviewScope и](../resources/accessreviewscheduledefinition.md) узнайте, как настроить область определения обзора [доступа.](/graph/accessreviews-scope-concept)</span><span class="sxs-lookup"><span data-stu-id="eab2b-155">See [accessReviewScope](../resources/accessreviewscheduledefinition.md) and also learn how to [configure the scope of your access review definition](/graph/accessreviews-scope-concept).</span></span>| 
| <span data-ttu-id="eab2b-156">settings</span><span class="sxs-lookup"><span data-stu-id="eab2b-156">settings</span></span> | [<span data-ttu-id="eab2b-157">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="eab2b-157">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="eab2b-158">Параметры для серии обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="eab2b-158">The settings for an access review series.</span></span> <span data-ttu-id="eab2b-159">Здесь определяется повторяемость.</span><span class="sxs-lookup"><span data-stu-id="eab2b-159">Recurrence is determined here.</span></span> <span data-ttu-id="eab2b-160">См. [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="eab2b-160">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="eab2b-161">рецензенты</span><span class="sxs-lookup"><span data-stu-id="eab2b-161">reviewers</span></span> | <span data-ttu-id="eab2b-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="eab2b-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span> | <span data-ttu-id="eab2b-163">Определяет, кто такие рецензенты.</span><span class="sxs-lookup"><span data-stu-id="eab2b-163">Defines who the reviewers are.</span></span> <span data-ttu-id="eab2b-164">Если нет указаны, обзор является самообнаверяемой (пользователи рассмотрели обзор собственного доступа).</span><span class="sxs-lookup"><span data-stu-id="eab2b-164">If none are specified, the review is a self-review (users reviewed review their own access).</span></span>  <span data-ttu-id="eab2b-165">Примеры вариантов назначения рецензентов см. в примере Назначение рецензентов определению обзора доступа с помощью [API microsoft Graph.](/graph/accessreviews-reviewers-concept)</span><span class="sxs-lookup"><span data-stu-id="eab2b-165">For examples of options for assigning reviewers, see [Assign reviewers to your access review definition using the Microsoft Graph API](/graph/accessreviews-reviewers-concept).</span></span> |
|<span data-ttu-id="eab2b-166">fallbackReviewers</span><span class="sxs-lookup"><span data-stu-id="eab2b-166">fallbackReviewers</span></span>|<span data-ttu-id="eab2b-167">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="eab2b-167">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="eab2b-168">При условии, если основные рецензенты не существуют, рецензентам откатов будет предложено завершить проверку.</span><span class="sxs-lookup"><span data-stu-id="eab2b-168">If provided, the fallback reviewers are asked to complete a review if the primary reviewers do not exist.</span></span> <span data-ttu-id="eab2b-169">Например, если менеджеры выбраны в качестве и у проверяемого директора нет менеджера в Azure AD, проверятелям откатов будет предложено просмотреть `reviewers` этот принцип.</span><span class="sxs-lookup"><span data-stu-id="eab2b-169">For example, if managers are selected as `reviewers` and a principal under review does not have a manager in Azure AD, the fallback reviewers are asked to review that principal.</span></span>|
| <span data-ttu-id="eab2b-170">additionalNotificationRecipients</span><span class="sxs-lookup"><span data-stu-id="eab2b-170">additionalNotificationRecipients</span></span>   |<span data-ttu-id="eab2b-171">[accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md) collection</span><span class="sxs-lookup"><span data-stu-id="eab2b-171">[accessReviewNotificationRecipientItem](../resources/accessReviewNotificationRecipientItem.md) collection</span></span>| <span data-ttu-id="eab2b-172">Определяет список дополнительных пользователей или членов группы, которые будут уведомлены о ходе проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="eab2b-172">Defines the list of additional users or group members to be notified of the access review progress.</span></span> |
| <span data-ttu-id="eab2b-173">backupReviewers (обесценив)</span><span class="sxs-lookup"><span data-stu-id="eab2b-173">backupReviewers (deprecated)</span></span> |<span data-ttu-id="eab2b-174">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span><span class="sxs-lookup"><span data-stu-id="eab2b-174">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="eab2b-175">Это свойство было заменено **fallbackReviewers**.</span><span class="sxs-lookup"><span data-stu-id="eab2b-175">This property has been replaced by **fallbackReviewers**.</span></span> <span data-ttu-id="eab2b-176">Однако указание резервных **копийReviewers** или **fallbackReviewers** автоматически заполняет те же значения для другого свойства.</span><span class="sxs-lookup"><span data-stu-id="eab2b-176">However, specifying either **backupReviewers** or **fallbackReviewers** automatically populates the same values to the other property.</span></span> |

## <a name="response"></a><span data-ttu-id="eab2b-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="eab2b-177">Response</span></span>
<span data-ttu-id="eab2b-178">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="eab2b-178">If successful, this method returns a `201 Created` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eab2b-179">Примеры</span><span class="sxs-lookup"><span data-stu-id="eab2b-179">Examples</span></span>

### <a name="example-1-create-an-access-review-on-a-group"></a><span data-ttu-id="eab2b-180">Пример 1. Создание обзора доступа для группы</span><span class="sxs-lookup"><span data-stu-id="eab2b-180">Example 1: Create an access review on a group</span></span>

<span data-ttu-id="eab2b-181">Это пример создания обзора доступа со следующими настройками:</span><span class="sxs-lookup"><span data-stu-id="eab2b-181">This is an example of creating an access review with the following settings:</span></span>
+ <span data-ttu-id="eab2b-182">В обзоре рассматриваются все члены группы, у которых есть **групповой id.** `02f3bafb-448c-487c-88c2-5fd65ce49a41`</span><span class="sxs-lookup"><span data-stu-id="eab2b-182">The review reviews all members of a group, whose group **id** is `02f3bafb-448c-487c-88c2-5fd65ce49a41`.</span></span>
+ <span data-ttu-id="eab2b-183">Конкретный пользователь, у которого есть **пользовательский ид,** `398164b1-5196-49dd-ada2-364b49f99b27` является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="eab2b-183">A specific user, whose user **id** is `398164b1-5196-49dd-ada2-364b49f99b27` is the reviewer.</span></span>
+ <span data-ttu-id="eab2b-184">Он повторяется еженедельно и продолжается бесконечно.</span><span class="sxs-lookup"><span data-stu-id="eab2b-184">It recurs weekly and continues indefinitely.</span></span>

#### <a name="request"></a><span data-ttu-id="eab2b-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="eab2b-185">Request</span></span>
<span data-ttu-id="eab2b-186">В теле запроса поставляем представление JSON объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eab2b-186">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="eab2b-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="eab2b-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Test create",
  "descriptionForAdmins": "New scheduled access review",
  "descriptionForReviewers": "If you have any questions, contact jerry@contoso.com",
  "scope": {
    "query": "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/398164b1-5196-49dd-ada2-364b49f99b27",
      "queryType": "MicrosoftGraph"
    }
  ],  
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-08T12:02:30.667Z"
      }
    }
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="eab2b-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eab2b-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="eab2b-189">C#</span><span class="sxs-lookup"><span data-stu-id="eab2b-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eab2b-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eab2b-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eab2b-191">Java</span><span class="sxs-lookup"><span data-stu-id="eab2b-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eab2b-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="eab2b-192">Response</span></span>
><span data-ttu-id="eab2b-193">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eab2b-193">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "29f2d16e-9ca6-4052-bbfe-802c48944448",
  "displayName": "Test create",
  "createdDateTime": "0001-01-01T00:00:00Z",
  "lastModifiedDateTime": "0001-01-01T00:00:00Z",
  "status": "NotStarted",
  "descriptionForAdmins": "Test create",
  "descriptionForReviewers": "Test create",
  "instanceEnumerationScope": null,
  "createdBy": {
    "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
    "displayName": "MOD Administrator",
    "userPrincipalName": "admin@contoso.com"
  },
  "scope": {
    "query": "/groups/b74444cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/7eae986b-d425-48b2-adf2-3c777f4444f3",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],  
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
        "month": 0,
        "dayOfMonth": 0,
        "daysOfWeek": [],
        "firstDayOfWeek": "sunday",
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "numberOfOccurrences": 0,
        "recurrenceTimeZone": null,
        "startDate": "2020-09-08",
        "endDate": null
      }
    },
  "applyActions": []
  }
}
```

### <a name="example-2-create-an-access-review-on-all-teams-with-inactive-guest-users"></a><span data-ttu-id="eab2b-194">Пример 2. Создание обзора доступа для всех групп с неактивными гостевых пользователей</span><span class="sxs-lookup"><span data-stu-id="eab2b-194">Example 2: Create an access review on all teams with inactive guest users</span></span>

<span data-ttu-id="eab2b-195">Это пример создания обзора доступа со следующими настройками:</span><span class="sxs-lookup"><span data-stu-id="eab2b-195">This is an example of creating an access review with the following settings:</span></span>
+ <span data-ttu-id="eab2b-196">В обзоре рассматриваются все группы с неактивными гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="eab2b-196">The review reviews all teams with inactive guest users.</span></span> <span data-ttu-id="eab2b-197">Период бездействия — 30 дней с даты начала проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="eab2b-197">The period of inactivity is 30 days from the start date of the access review.</span></span>
+ <span data-ttu-id="eab2b-198">Владельцы групп — это рецензенты и назначены рецензенты откатов.</span><span class="sxs-lookup"><span data-stu-id="eab2b-198">The group owners are the reviewers and fallback reviewers are assigned.</span></span>
+ <span data-ttu-id="eab2b-199">Он повторяется на третий день каждого квартала и продолжается бесконечно.</span><span class="sxs-lookup"><span data-stu-id="eab2b-199">It recurs on the third day of every quarter and continues indefinitely.</span></span>
+ <span data-ttu-id="eab2b-200">**autoApplyDecisionsEnabled** устанавливается с `true` **значением defaultDecision.** `Deny`</span><span class="sxs-lookup"><span data-stu-id="eab2b-200">**autoApplyDecisionsEnabled** is set to `true` with the **defaultDecision** set to `Deny`.</span></span>

#### <a name="request"></a><span data-ttu-id="eab2b-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="eab2b-201">Request</span></span>
<span data-ttu-id="eab2b-202">В теле запроса поставляем представление JSON объекта [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="eab2b-202">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="eab2b-203">HTTP</span><span class="sxs-lookup"><span data-stu-id="eab2b-203">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition_inactiveguests_M365"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Review inactive guests on teams",
  "descriptionForAdmins": "Control guest user access to our teams.",
  "descriptionForReviewers": "Information security is everyone's responsibility. Review our access policy for more.",
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
  },
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
    },
  "reviewers": [
    {
      "query": "./owners",
      "queryType": "MicrosoftGraph"
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "recommendationsEnabled": true,
    "instanceDurationInDays": 3,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "dayOfMonth": 5,
        "interval": 3
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-05-04T00:00:00.000Z"
      }
    },
    "defaultDecisionEnabled": true,
    "defaultDecision": "Deny",
    "autoApplyDecisionsEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="eab2b-204">C#</span><span class="sxs-lookup"><span data-stu-id="eab2b-204">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-inactiveguests-m365-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eab2b-205">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eab2b-205">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-inactiveguests-m365-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eab2b-206">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eab2b-206">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-inactiveguests-m365-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eab2b-207">Java</span><span class="sxs-lookup"><span data-stu-id="eab2b-207">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-inactiveguests-m365-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eab2b-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="eab2b-208">Response</span></span>
><span data-ttu-id="eab2b-209">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eab2b-209">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
  "id": "b0966e21-a01e-43c9-8f8b-9ba30ed5710a",
  "displayName": "Review inactive guests on teams",
  "createdDateTime": "2021-05-04T18:27:02.6719849Z",
  "lastModifiedDateTime": "2021-05-04T18:27:24.0889623Z",
  "status": "InProgress",
  "descriptionForAdmins": "Control guest user access to our teams.",
  "descriptionForReviewers": "Information security is everyone's responsibility. Review our access policy for more.",
  "createdBy": {
    "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
    "displayName": "MOD Administrator",
    "userPrincipalName": "admin@contoso.com"
  },
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "queryRoot": null,
    "inactiveDuration": "P30D"
  },
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team'))&$count=true",
    "queryType": "MicrosoftGraph",
    "queryRoot": null
  },
  "reviewers": [
    {
      "query": "./owners",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "backupReviewers": [],
  "fallbackReviewers": [
    {
      "query": "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": true,
    "defaultDecision": "Deny",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": true,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 3,
        "month": 0,
        "dayOfMonth": 5,
        "daysOfWeek": [],
        "firstDayOfWeek": "sunday",
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "numberOfOccurrences": 0,
        "recurrenceTimeZone": null,
        "startDate": "2021-05-05",
        "endDate": null
      }
    },
    "applyActions": []
  }
}
```

### <a name="example-3-create-an-access-review-of-all-users-to-an-application"></a><span data-ttu-id="eab2b-210">Пример 3. Создание обзора доступа всех пользователей к приложению</span><span class="sxs-lookup"><span data-stu-id="eab2b-210">Example 3: Create an access review of all users to an application</span></span>

<span data-ttu-id="eab2b-211">Это пример создания обзора доступа со следующими настройками:</span><span class="sxs-lookup"><span data-stu-id="eab2b-211">This is an example of creating an access review with the following settings:</span></span>
+ <span data-ttu-id="eab2b-212">В обзоре проверяется доступ пользователей к приложению.</span><span class="sxs-lookup"><span data-stu-id="eab2b-212">The review reviews user access to an application.</span></span>
+ <span data-ttu-id="eab2b-213">Менеджеры людей — это рецензенты, а рецензенты откатов — члены группы.</span><span class="sxs-lookup"><span data-stu-id="eab2b-213">The people managers are the reviewers and fallback reviewers are the members of a group.</span></span>
+ <span data-ttu-id="eab2b-214">Он повторяется в течение полугода и заканчивается 1 год с началаDate.</span><span class="sxs-lookup"><span data-stu-id="eab2b-214">It recurs semi-annually and ends 1 year from the startDate.</span></span>

#### <a name="request"></a><span data-ttu-id="eab2b-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="eab2b-215">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eab2b-216">HTTP</span><span class="sxs-lookup"><span data-stu-id="eab2b-216">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition_allusers_M365_AADRole"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Review employee access to LinkedIn",
  "descriptionForAdmins": "Review employee access to LinkedIn",
  "scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/users",
        "queryType": "MicrosoftGraph"
      }
    ],
    "resourceScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
        "queryType": "MicrosoftGraph"
      }
    ]
  },
  "reviewers": [
    {
      "query": "./manager",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "backupReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph"
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": true,
    "defaultDecision": "Recommendation",
    "instanceDurationInDays": 180,
    "autoApplyDecisionsEnabled": true,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 6,
        "dayOfMonth": 0
      },
      "range": {
        "type": "numbered",
        "startDate": "2021-05-05",
        "endDate": "2022-05-05"
      }
    }
  }
}
```
# <a name="c"></a>[<span data-ttu-id="eab2b-217">C#</span><span class="sxs-lookup"><span data-stu-id="eab2b-217">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-allusers-m365-aadrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eab2b-218">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eab2b-218">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-allusers-m365-aadrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eab2b-219">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eab2b-219">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-allusers-m365-aadrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eab2b-220">Java</span><span class="sxs-lookup"><span data-stu-id="eab2b-220">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-allusers-m365-aadrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eab2b-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="eab2b-221">Response</span></span>
><span data-ttu-id="eab2b-222">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eab2b-222">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
  "id": "1f79f34b-8667-40d9-875c-893b630b3dec",
  "scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/users",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
      }
    ],
    "resourceScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
      }
    ]
  },
  "reviewers": [
    {
      "query": "./manager",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "backupReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "settings": {
    "instanceDurationInDays": 180,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 6,
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
        "startDate": "2021-05-05",
        "endDate": "2022-05-05"
      }
    }
  }
}
```


<!--
{
  "type": "#page.annotation",
  "description": "Create accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
