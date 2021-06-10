---
title: Создание accessPackageAssignmentRequest
description: Создание нового accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d455bde8192cfd37713d32f10e5bb8d8b908cec0
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2021
ms.locfileid: "52868877"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="8e92c-103">Создание accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e92c-103">Create accessPackageAssignmentRequest</span></span>

<span data-ttu-id="8e92c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e92c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e92c-105">В [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md)создайте новый объект [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8e92c-105">In [Azure AD Entitlement Management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>  <span data-ttu-id="8e92c-106">Эта операция используется для назначения пользователя пакету доступа или удаления назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="8e92c-106">This operation is used to assign a user to an access package, or to remove an access package assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e92c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e92c-107">Permissions</span></span>

<span data-ttu-id="8e92c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e92c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e92c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e92c-110">Permission type</span></span>                        | <span data-ttu-id="8e92c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e92c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e92c-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e92c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e92c-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e92c-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="8e92c-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e92c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e92c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e92c-115">Not supported.</span></span> |
| <span data-ttu-id="8e92c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e92c-116">Application</span></span>                            | <span data-ttu-id="8e92c-117">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e92c-117">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e92c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e92c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="8e92c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e92c-119">Request headers</span></span>

| <span data-ttu-id="8e92c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="8e92c-120">Name</span></span>          | <span data-ttu-id="8e92c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8e92c-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8e92c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e92c-122">Authorization</span></span> | <span data-ttu-id="8e92c-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e92c-p103">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="8e92c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e92c-125">Content-Type</span></span>  | <span data-ttu-id="8e92c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e92c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e92c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e92c-128">Request body</span></span>

<span data-ttu-id="8e92c-129">В теле запроса поставляем представление JSON объекта [accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8e92c-129">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="8e92c-130">Для администратора, запрашиваемого для создания назначения для пользователя, значение свойства **requestType** составляет , а свойство `AdminAdd` **accessPackageAssignment** содержит назначенного пользователя, свойство `targetId` **assignmentPolicyId,** определяющий [accessPackageAssignmentPolicy,](../resources/accesspackageassignmentpolicy.md)и **свойство accessPackageId,** определяющий [accessPackageage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="8e92c-130">For an administrator to request to create an assignment for a user, the value of the **requestType** property is `AdminAdd`, and the **accessPackageAssignment** property contains the `targetId` of the user being assigned, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>

<span data-ttu-id="8e92c-131">Для администратора, запрашиваемого для удаления назначения, значение свойства **requestType** составляет , а свойство accessPackageAssignment содержит свойство id, определяющий удаляемую `AdminRemove`  [accessPackageAssignment.](../resources/accesspackageassignment.md) </span><span class="sxs-lookup"><span data-stu-id="8e92c-131">For an administrator to request to remove an assignment, the value of the **requestType** property is `AdminRemove`, and the **accessPackageAssignment** property contains the **id** property identifying the [accessPackageAssignment](../resources/accesspackageassignment.md) being removed.</span></span>

<span data-ttu-id="8e92c-132">Чтобы пользователь, не вступив в администратор, попросил создать свое собственное назначение для первого назначения или возобновления назначения, значение свойства **requestType** составляет `UserAdd` .</span><span class="sxs-lookup"><span data-stu-id="8e92c-132">For a non-administrator user to request to create their own assignment for either a first assignment or renew assignment, the value of the **requestType** property is `UserAdd`.</span></span> <span data-ttu-id="8e92c-133">Свойство **accessPackageAssignment** содержит свойство `targetId` с `id` пользователями.</span><span class="sxs-lookup"><span data-stu-id="8e92c-133">The **accessPackageAssignment** property contains the `targetId` with the `id` of the users.</span></span> <span data-ttu-id="8e92c-134">Свойство **assignmentPolicyId** определяет [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e92c-134">The **assignmentPolicyId** property identifies the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="8e92c-135">Свойство **accessPackageId** определяет [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="8e92c-135">The **accessPackageId** property identifies the [accessPackage](../resources/accesspackage.md).</span></span> <span data-ttu-id="8e92c-136">Пользователь, делая запрос, должен уже существовать в каталоге.</span><span class="sxs-lookup"><span data-stu-id="8e92c-136">The user making the request must already exist in the directory.</span></span>

<span data-ttu-id="8e92c-137">Чтобы пользователь, не вступив в администратор, запрашивал расширение своих назначений, значение свойства **requestType** `UserExtend` составляет .</span><span class="sxs-lookup"><span data-stu-id="8e92c-137">For a non-administrator user to request to extend their own assignments, the value of the **requestType** property is `UserExtend`.</span></span> <span data-ttu-id="8e92c-138">Свойство **accessPackageAssignment** содержит свойство `targetId` с `id` пользователями.</span><span class="sxs-lookup"><span data-stu-id="8e92c-138">The **accessPackageAssignment** property contains the `targetId` with the `id` of the users.</span></span> <span data-ttu-id="8e92c-139">Свойство **assignmentPolicyId** определяет [accessPackageAssignmentPolicy.](../resources/accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8e92c-139">The **assignmentPolicyId** property identifies the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="8e92c-140">Свойство **accessPackageId** определяет [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="8e92c-140">The **accessPackageId** property identifies the [accessPackage](../resources/accesspackage.md).</span></span> <span data-ttu-id="8e92c-141">Пользователь, делая запрос, должен уже существовать в каталоге.</span><span class="sxs-lookup"><span data-stu-id="8e92c-141">The user making the request must already exist in the directory.</span></span>

## <a name="response"></a><span data-ttu-id="8e92c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e92c-142">Response</span></span>

<span data-ttu-id="8e92c-143">В случае успешного выполнения этот метод возвращает код ответа из 200 серий и новый объект [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8e92c-143">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>  

<span data-ttu-id="8e92c-144">Если это запрос, то впоследствии создается `AdminAdd` [accessPackageAssignment](../resources/accesspackageassignment.md) и, при необходимости, [accessPackageSubject.](../resources/accesspackagesubject.md)</span><span class="sxs-lookup"><span data-stu-id="8e92c-144">If this is an `AdminAdd` request, then subsequently an [accessPackageAssignment](../resources/accesspackageassignment.md) and, if needed, an [accessPackageSubject](../resources/accesspackagesubject.md) are also created.</span></span> <span data-ttu-id="8e92c-145">Вы можете найти тех, кто использует параметры запроса при [перечислении accessPackageAssignments](accesspackageassignment-list.md).</span><span class="sxs-lookup"><span data-stu-id="8e92c-145">You can locate those using the query parameters when [listing accessPackageAssignments](accesspackageassignment-list.md).</span></span>

## <a name="examples"></a><span data-ttu-id="8e92c-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="8e92c-146">Examples</span></span>
### <a name="example-1-admin-requests-a-direct-assignment-for-a-user"></a><span data-ttu-id="8e92c-147">Пример 1. Администратор запрашивает прямое назначение для пользователя</span><span class="sxs-lookup"><span data-stu-id="8e92c-147">Example 1: Admin requests a direct assignment for a user</span></span>
#### <a name="request"></a><span data-ttu-id="8e92c-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e92c-148">Request</span></span>

<span data-ttu-id="8e92c-149">Ниже приводится пример запроса на прямое назначение, в котором администратор запрашивает создание назначения для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e92c-149">The following is an example of the request for a direct assignment, in which the administrator is requesting the creation of an assignment for the user.</span></span> <span data-ttu-id="8e92c-150">Так как [accessPackageSubject](../resources/accesspackagesubject.md) может еще не существовать, значение **targetID** — это объектный ID назначенного пользователя, значение **accessPackageId** — это желаемый пакет доступа для этого пользователя, а значение **assignmentPolicyId** — это политика прямого назначения в этом пакете доступа.</span><span class="sxs-lookup"><span data-stu-id="8e92c-150">Because the [accessPackageSubject](../resources/accesspackagesubject.md) might not yet exist, the value of the **targetID** is the object ID of the user being assigned, the value of the **accessPackageId** is the desired access package for that user, and the value of **assignmentPolicyId** is a direct assignment policy in that access package.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="8e92c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e92c-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_1"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "accessPackageAssignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="8e92c-152">C#</span><span class="sxs-lookup"><span data-stu-id="8e92c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e92c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e92c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e92c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e92c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e92c-155">Java</span><span class="sxs-lookup"><span data-stu-id="8e92c-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e92c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e92c-156">Response</span></span>

<span data-ttu-id="8e92c-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e92c-157">The following is an example of the response.</span></span>

> <span data-ttu-id="8e92c-158">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8e92c-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted",
  "isValidationOnly": false
}
```

### <a name="example-2-user-requests-a-package-and-answers-questions-for-approval"></a><span data-ttu-id="8e92c-159">Пример 2. Пользователь запрашивает пакет и отвечает на вопросы для утверждения</span><span class="sxs-lookup"><span data-stu-id="8e92c-159">Example 2: User requests a package and answers questions for approval</span></span>
#### <a name="request"></a><span data-ttu-id="8e92c-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e92c-160">Request</span></span>

<span data-ttu-id="8e92c-161">Ниже приводится пример запроса, в котором запросчик предоставил ответы на вопросы, чтобы помочь ему принять решение.</span><span class="sxs-lookup"><span data-stu-id="8e92c-161">The following is an example of a request where the requestor provided answers to the approver to help them make their decision.</span></span>
 



# <a name="http"></a>[<span data-ttu-id="8e92c-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e92c-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests_2"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "UserAdd",
    "accessPackageAssignment": {
        "targetId": "46184453-e63b-4f20-86c2-c557ed5d5df9",
        "assignmentPolicyId": "2264bf65-76ba-417b-a27d-54d291f0cbc8",
        "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF"
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA"
        }
    }]
}
```
# <a name="c"></a>[<span data-ttu-id="8e92c-163">C#</span><span class="sxs-lookup"><span data-stu-id="8e92c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e92c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e92c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e92c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e92c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e92c-166">Java</span><span class="sxs-lookup"><span data-stu-id="8e92c-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="8e92c-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e92c-167">Response</span></span>

<span data-ttu-id="8e92c-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e92c-168">The following is an example of the response.</span></span>

> <span data-ttu-id="8e92c-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8e92c-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e382d02-4454-436b-b700-59c7dd77f466",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
        "answeredQuestion": {
            "id" : "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF",
            "isRequired": false,
            "text": {
                "defaultText": "what state are you from?",
                "localizedTexts": [{
                    "text": "¿De qué estado eres?",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
            "choices": [{
                "actualValue": "AZ",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Arizona",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "CA",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "California",
                        "languageCode": "es"
                    }]
                }
            }, {
                "actualValue": "OH",
                "displayValue": {
                    "localizedTexts": [{
                        "text": "Ohio",
                        "languageCode": "es"
                    }]
                }
            }],
            "allowsMultipleSelection": false
        }
    }, {
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
        "answeredQuestion": {
            "id" : "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA",
            "isRequired": false,
            "text": {
                "defaultText": "Who is your manager?",
                "localizedTexts": [{
                    "text": "por qué necesita acceso a este paquete",
                    "languageCode": "es"
                }]
            },
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": false
        }
    }]
}
```
### <a name="example-3-request-a-package-and-provide-a-justification"></a><span data-ttu-id="8e92c-170">Пример 3. Запрос пакета и обоснование</span><span class="sxs-lookup"><span data-stu-id="8e92c-170">Example 3: Request a package and provide a justification</span></span>
#### <a name="request"></a><span data-ttu-id="8e92c-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e92c-171">Request</span></span>

<span data-ttu-id="8e92c-172">В следующем примере показано, как запросить пакет доступа и предоставить обоснование для утвержденного.</span><span class="sxs-lookup"><span data-stu-id="8e92c-172">The following example shows how to request an access package and provide justification to the approver.</span></span>
 


<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
    "requestType": "UserAdd",
    "accessPackageAssignment": {
        "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b"
    },
    "justification":"Need access to New Hire access package"
}
```

#### <a name="response"></a><span data-ttu-id="8e92c-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e92c-173">Response</span></span>

<span data-ttu-id="8e92c-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e92c-174">The following is an example of the response.</span></span>

> <span data-ttu-id="8e92c-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e92c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "813bbc6b-31f5-4cdf-8fed-1ba4284a1e3f",
    "requestType": "UserAdd",
    "requestState": "Submitted",
    "requestStatus": "Accepted",
    "isValidationOnly": false,
    "expirationDateTime": null,
    "justification": "Requested for the new task.",
    "answers": [],
    "schedule": {
        "startDateTime": null,
        "recurrence": null,
        "expiration": {
            "endDateTime": null,
            "duration": null,
            "type": null
        }
    }
}
```

### <a name="example-4-remove-an-assignment"></a><span data-ttu-id="8e92c-177">Пример 4. Удаление назначения</span><span class="sxs-lookup"><span data-stu-id="8e92c-177">Example 4: Remove an assignment</span></span>

<span data-ttu-id="8e92c-178">Чтобы удалить назначения, создайте новый объект accessPackageAssignmentRequest со следующими настройками:</span><span class="sxs-lookup"><span data-stu-id="8e92c-178">To remove assignments, create a new accessPackageAssignmentRequest object with the following settings:</span></span>

+ <span data-ttu-id="8e92c-179">Значение свойства **requestType,** установленного для `AdminRemove` .</span><span class="sxs-lookup"><span data-stu-id="8e92c-179">The value of the **requestType** property set to `AdminRemove`.</span></span>
+ <span data-ttu-id="8e92c-180">В свойство accessPackageAssignment включите список с идентификатором объектов accessPackageAssignment для удаления.</span><span class="sxs-lookup"><span data-stu-id="8e92c-180">In the accessPackageAssignment property, include a list with the identifier of the accessPackageAssignment objects to delete.</span></span>

#### <a name="request"></a><span data-ttu-id="8e92c-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e92c-181">Request</span></span>

<span data-ttu-id="8e92c-182">В следующем примере показано, как удалить назначение.</span><span class="sxs-lookup"><span data-stu-id="8e92c-182">The following example shows how to remove an assignment.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

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

#### <a name="response"></a><span data-ttu-id="8e92c-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e92c-183">Response</span></span>

<span data-ttu-id="8e92c-184">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8e92c-184">The following is an example of the response.</span></span>

> <span data-ttu-id="8e92c-p110">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e92c-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessPackageAssignmentRequests/$entity",

    "id": "78eaee8c-e6cf-48c9-8f99-aae44c35e379",
    "requestType": "AdminRemove",
    "requestState": "Submitted",
    "requestStatus": "Accepted"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


