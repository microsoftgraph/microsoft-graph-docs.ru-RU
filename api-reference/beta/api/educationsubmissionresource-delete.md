---
title: Удаление Едукатионсубмиссионресаурце
description: Удаляет ресурс из отправки. Это может сделать только студентом. Если ресурс был скопирован из назначения, то после удаления текущей копии будет создан новый экземпляр ресурса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4dc8b2970bf6cf241c93934593d0424d538fc01a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955407"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="0fdd7-105">Удаление Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="0fdd7-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="0fdd7-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fdd7-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fdd7-107">Удаляет ресурс из отправки.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="0fdd7-108">Это может сделать только студентом.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-108">This can only be done by the student.</span></span> <span data-ttu-id="0fdd7-109">Если ресурс был скопирован из назначения, то после удаления текущей копии будет создан новый экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="0fdd7-110">Это позволяет «сбросить» ресурс в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="0fdd7-111">Если ресурс не был скопирован из назначения, но добавлен из учащегося, ресурс просто удаляется.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="0fdd7-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fdd7-112">Permissions</span></span>
<span data-ttu-id="0fdd7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fdd7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fdd7-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fdd7-115">Permission type</span></span>      | <span data-ttu-id="0fdd7-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fdd7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fdd7-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fdd7-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="0fdd7-118">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fdd7-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="0fdd7-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fdd7-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0fdd7-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-120">Not supported.</span></span>  |
|<span data-ttu-id="0fdd7-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fdd7-121">Application</span></span> | <span data-ttu-id="0fdd7-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0fdd7-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fdd7-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="0fdd7-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fdd7-124">Request headers</span></span>
| <span data-ttu-id="0fdd7-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0fdd7-125">Header</span></span>       | <span data-ttu-id="0fdd7-126">Значение</span><span class="sxs-lookup"><span data-stu-id="0fdd7-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0fdd7-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0fdd7-127">Authorization</span></span>  | <span data-ttu-id="0fdd7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0fdd7-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0fdd7-130">Request body</span></span>
<span data-ttu-id="0fdd7-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0fdd7-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fdd7-132">Response</span></span>
<span data-ttu-id="0fdd7-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fdd7-135">Пример</span><span class="sxs-lookup"><span data-stu-id="0fdd7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fdd7-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fdd7-136">Request</span></span>
<span data-ttu-id="0fdd7-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0fdd7-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fdd7-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="0fdd7-139">C#</span><span class="sxs-lookup"><span data-stu-id="0fdd7-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0fdd7-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0fdd7-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0fdd7-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0fdd7-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0fdd7-142">Java</span><span class="sxs-lookup"><span data-stu-id="0fdd7-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0fdd7-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fdd7-143">Response</span></span>
<span data-ttu-id="0fdd7-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0fdd7-144">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


