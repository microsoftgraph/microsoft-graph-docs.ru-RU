---
title: Удаление Едукатионассигнментресаурце
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e2b0e901284a56c5b123bf4f89b5a5573796ad50
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955693"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="cae01-103">Удаление Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="cae01-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cae01-104">Удаление ресурса из назначения.</span><span class="sxs-lookup"><span data-stu-id="cae01-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="cae01-105">Только преподаватели в классе могут удалить ресурс.</span><span class="sxs-lookup"><span data-stu-id="cae01-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="cae01-106">После публикации назначения для учащихся преподаватели не могут удалять ресурсы, помеченные как "Дистрибутетостудентс".</span><span class="sxs-lookup"><span data-stu-id="cae01-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="cae01-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae01-107">Permissions</span></span>
<span data-ttu-id="cae01-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae01-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae01-110">Permission type</span></span>      | <span data-ttu-id="cae01-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cae01-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae01-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae01-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="cae01-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cae01-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="cae01-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae01-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cae01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae01-115">Not supported.</span></span>  |
|<span data-ttu-id="cae01-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae01-116">Application</span></span> | <span data-ttu-id="cae01-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae01-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cae01-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae01-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="cae01-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cae01-119">Request headers</span></span>
| <span data-ttu-id="cae01-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cae01-120">Header</span></span>       | <span data-ttu-id="cae01-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cae01-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cae01-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cae01-122">Authorization</span></span>  | <span data-ttu-id="cae01-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cae01-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cae01-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cae01-125">Request body</span></span>
<span data-ttu-id="cae01-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cae01-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cae01-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae01-127">Response</span></span>
<span data-ttu-id="cae01-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cae01-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cae01-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cae01-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cae01-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae01-131">Request</span></span>
<span data-ttu-id="cae01-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae01-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cae01-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae01-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cae01-134">C#</span><span class="sxs-lookup"><span data-stu-id="cae01-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cae01-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="cae01-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cae01-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cae01-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cae01-137">Java</span><span class="sxs-lookup"><span data-stu-id="cae01-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cae01-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae01-138">Response</span></span>
<span data-ttu-id="cae01-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cae01-139">The following is an example of the response.</span></span> 


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
