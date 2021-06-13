---
title: Список ресурсов отправки
description: Список ресурсов, связанных с отправкой.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 174f9fa606ab9f4a4bdc85fb60dd1e4f75d7ae39
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911812"
---
# <a name="list-submission-resources"></a><span data-ttu-id="1db32-103">Список ресурсов отправки</span><span class="sxs-lookup"><span data-stu-id="1db32-103">List submission resources</span></span>

<span data-ttu-id="1db32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1db32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1db32-105">Список ресурсов, связанных с отправкой.</span><span class="sxs-lookup"><span data-stu-id="1db32-105">List the resources associated with a submission.</span></span> 

<span data-ttu-id="1db32-106">Объект **submissionResource** — это оболочка вокруг фактического объекта ресурса, над который работает студент.</span><span class="sxs-lookup"><span data-stu-id="1db32-106">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="1db32-107">Оболочка также включает указатель на ресурсы назначения, если он был скопирован из назначения во время процесса назначения.</span><span class="sxs-lookup"><span data-stu-id="1db32-107">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="1db32-108">Эти ресурсы являются рабочей копией назначения.</span><span class="sxs-lookup"><span data-stu-id="1db32-108">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="1db32-109">**SubmittedResources —** это ресурсы, официально отправленные для оценки.</span><span class="sxs-lookup"><span data-stu-id="1db32-109">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="1db32-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1db32-110">Permissions</span></span>

<span data-ttu-id="1db32-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1db32-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1db32-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1db32-113">Permission type</span></span>                        | <span data-ttu-id="1db32-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1db32-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1db32-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1db32-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="1db32-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1db32-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="1db32-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1db32-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1db32-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1db32-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="1db32-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="1db32-119">Application</span></span>                            | <span data-ttu-id="1db32-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1db32-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1db32-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1db32-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1db32-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1db32-122">Optional query parameters</span></span>

<span data-ttu-id="1db32-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1db32-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1db32-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1db32-124">Request headers</span></span>

| <span data-ttu-id="1db32-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1db32-125">Header</span></span>        | <span data-ttu-id="1db32-126">Значение</span><span class="sxs-lookup"><span data-stu-id="1db32-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="1db32-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1db32-127">Authorization</span></span> | <span data-ttu-id="1db32-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1db32-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1db32-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1db32-130">Request body</span></span>

<span data-ttu-id="1db32-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1db32-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1db32-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="1db32-132">Response</span></span>

<span data-ttu-id="1db32-133">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1db32-133">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1db32-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1db32-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1db32-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1db32-135">Request</span></span>

<span data-ttu-id="1db32-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1db32-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1db32-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="1db32-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/submissions/{id}/resources
```
# <a name="c"></a>[<span data-ttu-id="1db32-138">C#</span><span class="sxs-lookup"><span data-stu-id="1db32-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1db32-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1db32-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1db32-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1db32-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1db32-141">Java</span><span class="sxs-lookup"><span data-stu-id="1db32-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1db32-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1db32-142">Response</span></span>

<span data-ttu-id="1db32-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1db32-143">The following is an example of the response.</span></span> 

><span data-ttu-id="1db32-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1db32-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
