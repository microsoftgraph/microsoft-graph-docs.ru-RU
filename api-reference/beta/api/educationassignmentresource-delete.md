---
title: Удаление Едукатионассигнментресаурце
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a7f7646474f9c26557a46b46d08cf40fe3241558
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966482"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="1952d-103">Удаление Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="1952d-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="1952d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1952d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1952d-105">Удаление ресурса из назначения.</span><span class="sxs-lookup"><span data-stu-id="1952d-105">Delete a resource from an assignment.</span></span> <span data-ttu-id="1952d-106">Только преподаватели в классе могут удалить ресурс.</span><span class="sxs-lookup"><span data-stu-id="1952d-106">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="1952d-107">После публикации назначения для учащихся преподаватели не могут удалять ресурсы, помеченные как "Дистрибутетостудентс".</span><span class="sxs-lookup"><span data-stu-id="1952d-107">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="1952d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1952d-108">Permissions</span></span>
<span data-ttu-id="1952d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1952d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1952d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1952d-111">Permission type</span></span>      | <span data-ttu-id="1952d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1952d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1952d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1952d-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="1952d-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1952d-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1952d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1952d-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1952d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1952d-116">Not supported.</span></span>  |
|<span data-ttu-id="1952d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1952d-117">Application</span></span> | <span data-ttu-id="1952d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1952d-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1952d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1952d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1952d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1952d-120">Request headers</span></span>
| <span data-ttu-id="1952d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1952d-121">Header</span></span>       | <span data-ttu-id="1952d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1952d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1952d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1952d-123">Authorization</span></span>  | <span data-ttu-id="1952d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1952d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1952d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1952d-126">Request body</span></span>
<span data-ttu-id="1952d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1952d-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1952d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1952d-128">Response</span></span>
<span data-ttu-id="1952d-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1952d-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1952d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1952d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1952d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1952d-132">Request</span></span>
<span data-ttu-id="1952d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1952d-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1952d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1952d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="1952d-135">C#</span><span class="sxs-lookup"><span data-stu-id="1952d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1952d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1952d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1952d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1952d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1952d-138">Java</span><span class="sxs-lookup"><span data-stu-id="1952d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1952d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1952d-139">Response</span></span>
<span data-ttu-id="1952d-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1952d-140">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


