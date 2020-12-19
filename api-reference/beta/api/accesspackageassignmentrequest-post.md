---
title: Создание accessPackageAssignmentRequest
description: Создайте новый accessPackageAssignmentRequest.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75388c02cf63113c28475b77b194a67c76d588b8
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719551"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="30ef0-103">Создание accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="30ef0-103">Create accessPackageAssignmentRequest</span></span>

<span data-ttu-id="30ef0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30ef0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30ef0-105">В [средстве управления правами Azure AD](../resources/entitlementmanagement-root.md)создайте новый [объект accessPackageAssignmentRequest.](../resources/accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="30ef0-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>  <span data-ttu-id="30ef0-106">Эта операция используется для назначения пользователя пакету доступа или удаления назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="30ef0-106">This operation is used to assign a user to an access package, or to remove an access package assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="30ef0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30ef0-107">Permissions</span></span>

<span data-ttu-id="30ef0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30ef0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30ef0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30ef0-110">Permission type</span></span>                        | <span data-ttu-id="30ef0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30ef0-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="30ef0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30ef0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="30ef0-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30ef0-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="30ef0-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30ef0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30ef0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30ef0-115">Not supported.</span></span> |
| <span data-ttu-id="30ef0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30ef0-116">Application</span></span>                            | <span data-ttu-id="30ef0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30ef0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30ef0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30ef0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="30ef0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30ef0-119">Request headers</span></span>

| <span data-ttu-id="30ef0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="30ef0-120">Name</span></span>          | <span data-ttu-id="30ef0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="30ef0-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="30ef0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30ef0-122">Authorization</span></span> | <span data-ttu-id="30ef0-123">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="30ef0-123">Bearer \{token\}.</span></span> <span data-ttu-id="30ef0-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="30ef0-124">Required.</span></span> |
| <span data-ttu-id="30ef0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30ef0-125">Content-Type</span></span>  | <span data-ttu-id="30ef0-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30ef0-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30ef0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30ef0-128">Request body</span></span>

<span data-ttu-id="30ef0-129">В теле запроса укажу представление объекта [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="30ef0-129">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

<span data-ttu-id="30ef0-130">Чтобы администратор запрашивал создание назначения для пользователя, свойство **requestType** имеет значение , а свойство `AdminAdd` **accessPackageAssignment** содержит назначенного пользователя, свойство `targetId` **assignmentPolicyId,** определяющие [accessPackageAssignmentPolicy,](../resources/accesspackageassignmentpolicy.md)и свойство **accessPackageId,** определяющие [accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="30ef0-130">For an administrator to request to create an assignment for a user, the value of the **requestType** property is `AdminAdd`, and the **accessPackageAssignment** property contains the `targetId` of the user being assigned, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>

<span data-ttu-id="30ef0-131">Чтобы администратор запрашивал удаление назначения, свойство **requestType** имеет значение , а свойство `AdminRemove` **accessPackageAssignment** содержит свойство **id,** определяющие удаляемую [accessPackageAssignment.](../resources/accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="30ef0-131">For an administrator to request to remove an assignment, the value of the **requestType** property is `AdminRemove`, and the **accessPackageAssignment** property contains the **id** property identifying the [accessPackageAssignment](../resources/accesspackageassignment.md) being removed.</span></span>

<span data-ttu-id="30ef0-132">Чтобы пользователь, не управляющего, запросил создание назначения для себя, свойство **requestType** имеет значение , а свойство `UserAdd` **accessPackageAssignment содержит свойство accessPackageAssignment** с ИД самих пользователей, свойство `targetId` **assignmentPolicyId,** определяющие [accessPackageAssignmentPolicy,](../resources/accesspackageassignmentpolicy.md)и свойство **accessPackageId,** определяющие [accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="30ef0-132">For a non-administrator user to request to create an assignment for themselves, the value of the **requestType** property is `UserAdd`, and the **accessPackageAssignment** property contains the `targetId` with the ID of the users themselves, the **assignmentPolicyId** property identifying the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md), and the **accessPackageId** property identifying the [accessPackage](../resources/accesspackage.md).</span></span>  <span data-ttu-id="30ef0-133">Пользователь, который делает запрос, должен уже существовать в каталоге.</span><span class="sxs-lookup"><span data-stu-id="30ef0-133">The user making the request must already exist in the directory.</span></span>

## <a name="response"></a><span data-ttu-id="30ef0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="30ef0-134">Response</span></span>

<span data-ttu-id="30ef0-135">В случае успешного выполнения этот метод возвращает код отклика из 200 рядов и новый объект [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30ef0-135">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>  

<span data-ttu-id="30ef0-136">Если это запрос, то затем также создается `AdminAdd` [accessPackageAssignment](../resources/accesspackageassignment.md) и, при необходимости, [accessPackageSubject.](../resources/accesspackagesubject.md)</span><span class="sxs-lookup"><span data-stu-id="30ef0-136">If this is an `AdminAdd` request, then subsequently an [accessPackageAssignment](../resources/accesspackageassignment.md) and, if needed, an [accessPackageSubject](../resources/accesspackagesubject.md) are also created.</span></span> <span data-ttu-id="30ef0-137">Их можно найти с помощью параметров запроса при [перечислении объектов accessPackageAssignment.](accesspackageassignment-list.md)</span><span class="sxs-lookup"><span data-stu-id="30ef0-137">You can locate those using the query parameters when [listing accessPackageAssignments](accesspackageassignment-list.md).</span></span>

## <a name="examples"></a><span data-ttu-id="30ef0-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="30ef0-138">Examples</span></span>
### <a name="example-1-admin-requests-a-direct-assignment-for-a-user"></a><span data-ttu-id="30ef0-139">Пример 1. Администратор запрашивает прямое назначение для пользователя</span><span class="sxs-lookup"><span data-stu-id="30ef0-139">Example 1: Admin requests a direct assignment for a user</span></span>
#### <a name="request"></a><span data-ttu-id="30ef0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="30ef0-140">Request</span></span>

<span data-ttu-id="30ef0-141">Ниже приводится пример запроса на прямое назначение, в котором администратор запрашивает создание назначения для пользователя.</span><span class="sxs-lookup"><span data-stu-id="30ef0-141">The following is an example of the request for a direct assignment, in which the administrator is requesting the creation of an assignment for the user.</span></span> <span data-ttu-id="30ef0-142">Так как [accessPackageSubject](../resources/accesspackagesubject.md) может еще не существовать, **значение targetID** — это ИД объекта назначенного пользователя, значение **accessPackageId** — это нужный пакет доступа для этого пользователя, а **значение assignmentPolicyId** — это политика прямого назначения в этом пакете доступа.</span><span class="sxs-lookup"><span data-stu-id="30ef0-142">Because the [accessPackageSubject](../resources/accesspackagesubject.md) might not yet exist, the value of the **targetID** is the object ID of the user being assigned, the value of the **accessPackageId** is the desired access package for that user, and the value of **assignmentPolicyId** is a direct assignment policy in that access package.</span></span>
 

# <a name="http"></a>[<span data-ttu-id="30ef0-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="30ef0-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
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
# <a name="c"></a>[<span data-ttu-id="30ef0-144">C#</span><span class="sxs-lookup"><span data-stu-id="30ef0-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30ef0-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30ef0-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30ef0-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30ef0-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30ef0-147">Java</span><span class="sxs-lookup"><span data-stu-id="30ef0-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="30ef0-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="30ef0-148">Response</span></span>

<span data-ttu-id="30ef0-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30ef0-149">The following is an example of the response.</span></span>

> <span data-ttu-id="30ef0-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30ef0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-user-requests-a-package-and-answers-questions-for-approval"></a><span data-ttu-id="30ef0-152">Пример 2. Пользователь запрашивает пакет и отвечает на вопросы на утверждение</span><span class="sxs-lookup"><span data-stu-id="30ef0-152">Example 2: User requests a package and answers questions for approval</span></span>
#### <a name="request"></a><span data-ttu-id="30ef0-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="30ef0-153">Request</span></span>

<span data-ttu-id="30ef0-154">Ниже приводится пример запроса, в котором запрашиватель предоставил ответ утвержденному, чтобы помочь ему принять решение.</span><span class="sxs-lookup"><span data-stu-id="30ef0-154">The following is an example of a request where the requestor provided answers to the approver to help them make their decision.</span></span>
 


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


---


#### <a name="response"></a><span data-ttu-id="30ef0-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="30ef0-155">Response</span></span>

<span data-ttu-id="30ef0-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30ef0-156">The following is an example of the response.</span></span>

> <span data-ttu-id="30ef0-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30ef0-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


