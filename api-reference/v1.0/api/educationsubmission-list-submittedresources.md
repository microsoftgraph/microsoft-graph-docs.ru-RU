---
title: Список, представленныйРесурсеи
description: Список ресурсов, официально отправленных для классификации.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2fc647442d302bfd38705725374e8933dc9e0702
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993450"
---
# <a name="list-submittedresources"></a><span data-ttu-id="f97fc-103">Список, представленныйРесурсеи</span><span class="sxs-lookup"><span data-stu-id="f97fc-103">List submittedResources</span></span>

<span data-ttu-id="f97fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f97fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f97fc-105">Список ресурсов, официально отправленных для классификации.</span><span class="sxs-lookup"><span data-stu-id="f97fc-105">List the resources that have officially been submitted for grading.</span></span> 

<span data-ttu-id="f97fc-106">Учащийся, которому принадлежит отправка, не может изменить представленный список без повторного отправки задания.</span><span class="sxs-lookup"><span data-stu-id="f97fc-106">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="f97fc-107">Это оболочка вокруг реального ресурса и может содержать указатель обратно на фактический ресурс назначения, если этот ресурс был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="f97fc-107">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="f97fc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f97fc-108">Permissions</span></span>
<span data-ttu-id="f97fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f97fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f97fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f97fc-111">Permission type</span></span>      | <span data-ttu-id="f97fc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f97fc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f97fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f97fc-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f97fc-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f97fc-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f97fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f97fc-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f97fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f97fc-116">Not supported.</span></span>  |
|<span data-ttu-id="f97fc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f97fc-117">Application</span></span> | <span data-ttu-id="f97fc-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f97fc-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f97fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f97fc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f97fc-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f97fc-120">Optional query parameters</span></span>
<span data-ttu-id="f97fc-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f97fc-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f97fc-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f97fc-122">Request headers</span></span>
| <span data-ttu-id="f97fc-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f97fc-123">Header</span></span>       | <span data-ttu-id="f97fc-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f97fc-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f97fc-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f97fc-125">Authorization</span></span>  | <span data-ttu-id="f97fc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f97fc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f97fc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f97fc-128">Request body</span></span>
<span data-ttu-id="f97fc-129">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f97fc-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f97fc-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f97fc-130">Response</span></span>
<span data-ttu-id="f97fc-131">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f97fc-131">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f97fc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f97fc-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="f97fc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f97fc-133">Request</span></span>
<span data-ttu-id="f97fc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f97fc-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f97fc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f97fc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_submittedresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/submittedResources
```
# <a name="c"></a>[<span data-ttu-id="f97fc-136">C#</span><span class="sxs-lookup"><span data-stu-id="f97fc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submittedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f97fc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f97fc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submittedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f97fc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f97fc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submittedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f97fc-139">Java</span><span class="sxs-lookup"><span data-stu-id="f97fc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submittedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f97fc-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f97fc-140">Response</span></span>
<span data-ttu-id="f97fc-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f97fc-141">The following is an example of the response.</span></span> 

><span data-ttu-id="f97fc-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f97fc-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
        "assignmentResourceUrl": null,
        "id": "0f7dd681-f1b6-4f78-b8fb-a579fc4a36ae",
        "resource": {
            "@odata.type": "#microsoft.graph.educationLinkResource",
            "displayName": "ABC",
            "createdDateTime": "2021-03-11T20:47:53.0823323Z",
            "lastModifiedDateTime": "2021-03-11T20:47:53.0823323Z",
            "link": "https://www.bing.com/",
            "createdBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
                    "displayName": null
                }
            },
            "lastModifiedBy": {
                "application": null,
                "device": null,
                "user": {
                    "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
                    "displayName": null
                }
            }
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
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
