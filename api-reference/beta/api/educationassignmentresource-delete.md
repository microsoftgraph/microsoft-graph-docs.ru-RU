---
title: Удаление Едукатионассигнментресаурце
description: .
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: afec6b216fe22eadffdc76049220cdd1f02c74a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320884"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="41acf-103">Удаление Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="41acf-103">Delete educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41acf-104">Удаление ресурса из назначения.</span><span class="sxs-lookup"><span data-stu-id="41acf-104">Delete a resource from an assignment.</span></span> <span data-ttu-id="41acf-105">Только преподаватели в классе могут удалить ресурс.</span><span class="sxs-lookup"><span data-stu-id="41acf-105">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="41acf-106">После публикации назначения для учащихся преподаватели не могут удалять ресурсы, помеченные как "Дистрибутетостудентс".</span><span class="sxs-lookup"><span data-stu-id="41acf-106">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="41acf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41acf-107">Permissions</span></span>
<span data-ttu-id="41acf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41acf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41acf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41acf-110">Permission type</span></span>      | <span data-ttu-id="41acf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41acf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41acf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41acf-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="41acf-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41acf-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="41acf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41acf-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="41acf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41acf-115">Not supported.</span></span>  |
|<span data-ttu-id="41acf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41acf-116">Application</span></span> | <span data-ttu-id="41acf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41acf-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="41acf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41acf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="41acf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41acf-119">Request headers</span></span>
| <span data-ttu-id="41acf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41acf-120">Header</span></span>       | <span data-ttu-id="41acf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="41acf-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41acf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41acf-122">Authorization</span></span>  | <span data-ttu-id="41acf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41acf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41acf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41acf-125">Request body</span></span>
<span data-ttu-id="41acf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41acf-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="41acf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="41acf-127">Response</span></span>
<span data-ttu-id="41acf-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="41acf-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41acf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="41acf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41acf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="41acf-131">Request</span></span>
<span data-ttu-id="41acf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41acf-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="41acf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="41acf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41acf-134">C#</span><span class="sxs-lookup"><span data-stu-id="41acf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41acf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41acf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41acf-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="41acf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41acf-137">Java</span><span class="sxs-lookup"><span data-stu-id="41acf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="41acf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="41acf-138">Response</span></span>
<span data-ttu-id="41acf-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41acf-139">The following is an example of the response.</span></span> 


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
