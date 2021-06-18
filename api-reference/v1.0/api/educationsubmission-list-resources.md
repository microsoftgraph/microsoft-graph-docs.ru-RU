---
title: Список ресурсов отправки
description: Список ресурсов, связанных с отправкой.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a2f1f12f750ab3387c437bd62fda70621feba489
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993485"
---
# <a name="list-submission-resources"></a><span data-ttu-id="ea8ee-103">Список ресурсов отправки</span><span class="sxs-lookup"><span data-stu-id="ea8ee-103">List submission resources</span></span>

<span data-ttu-id="ea8ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea8ee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea8ee-105">Список ресурсов, связанных с [отправкой.](../resources/educationsubmission.md)</span><span class="sxs-lookup"><span data-stu-id="ea8ee-105">List the resources associated with a [submission](../resources/educationsubmission.md).</span></span> 

<span data-ttu-id="ea8ee-106">Объект **submissionResource** — это оболочка вокруг фактического объекта ресурса, над который работает студент.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-106">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="ea8ee-107">Оболочка также включает указатель на ресурсы назначения, если он был скопирован из назначения во время процесса назначения.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-107">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="ea8ee-108">Эти ресурсы являются рабочей копией назначения.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-108">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="ea8ee-109">**SubmittedResources —** это ресурсы, официально отправленные для оценки.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-109">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea8ee-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea8ee-110">Permissions</span></span>

<span data-ttu-id="ea8ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea8ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea8ee-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea8ee-113">Permission type</span></span>                        | <span data-ttu-id="ea8ee-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea8ee-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ea8ee-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea8ee-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea8ee-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea8ee-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="ea8ee-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea8ee-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea8ee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="ea8ee-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="ea8ee-119">Application</span></span>                            | <span data-ttu-id="ea8ee-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea8ee-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea8ee-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea8ee-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea8ee-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea8ee-122">Optional query parameters</span></span>

<span data-ttu-id="ea8ee-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea8ee-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea8ee-124">Request headers</span></span>

| <span data-ttu-id="ea8ee-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea8ee-125">Header</span></span>        | <span data-ttu-id="ea8ee-126">Значение</span><span class="sxs-lookup"><span data-stu-id="ea8ee-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ea8ee-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ea8ee-127">Authorization</span></span> | <span data-ttu-id="ea8ee-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea8ee-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea8ee-130">Request body</span></span>

<span data-ttu-id="ea8ee-131">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-131">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea8ee-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea8ee-132">Response</span></span>

<span data-ttu-id="ea8ee-133">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-133">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea8ee-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ea8ee-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea8ee-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea8ee-135">Request</span></span>

<span data-ttu-id="ea8ee-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ea8ee-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea8ee-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources
```
# <a name="c"></a>[<span data-ttu-id="ea8ee-138">C#</span><span class="sxs-lookup"><span data-stu-id="ea8ee-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea8ee-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea8ee-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea8ee-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea8ee-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea8ee-141">Java</span><span class="sxs-lookup"><span data-stu-id="ea8ee-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ea8ee-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea8ee-142">Response</span></span>

<span data-ttu-id="ea8ee-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-143">The following is an example of the response.</span></span> 

><span data-ttu-id="ea8ee-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ea8ee-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
