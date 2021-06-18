---
title: Удаление educationAssignmentResource
description: Удалите определенный ресурс, присоединенный к назначению.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 16cb969fc4f1980c7ec5b37f5dfb8c1c384c6e7f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993014"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="b53d8-103">Удаление educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="b53d8-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="b53d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b53d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b53d8-105">Удалите определенный ресурс, присоединенный к назначению.</span><span class="sxs-lookup"><span data-stu-id="b53d8-105">Delete a specific resource attached to an assignment.</span></span>

<span data-ttu-id="b53d8-106">В общем, удалить ресурс могут только преподаватели в классе.</span><span class="sxs-lookup"><span data-stu-id="b53d8-106">In general, only teachers in the class can remove a resource.</span></span> <span data-ttu-id="b53d8-107">Однако после публикации задания преподаватели не могут удалять ресурсы, помеченные как "distributeToStudents".</span><span class="sxs-lookup"><span data-stu-id="b53d8-107">However, teachers cannot remove resources marked as "distributeToStudents", after the assignment has been published to students.</span></span>

## <a name="permissions"></a><span data-ttu-id="b53d8-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b53d8-108">Permissions</span></span>
<span data-ttu-id="b53d8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b53d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b53d8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b53d8-111">Permission type</span></span>      | <span data-ttu-id="b53d8-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b53d8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b53d8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b53d8-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="b53d8-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b53d8-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b53d8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b53d8-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b53d8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b53d8-116">Not supported.</span></span>  |
|<span data-ttu-id="b53d8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b53d8-117">Application</span></span> | <span data-ttu-id="b53d8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b53d8-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b53d8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b53d8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c

```
## <a name="request-headers"></a><span data-ttu-id="b53d8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b53d8-120">Request headers</span></span>
| <span data-ttu-id="b53d8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b53d8-121">Header</span></span>       | <span data-ttu-id="b53d8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b53d8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b53d8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b53d8-123">Authorization</span></span>  | <span data-ttu-id="b53d8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b53d8-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b53d8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b53d8-126">Request body</span></span>
<span data-ttu-id="b53d8-127">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b53d8-127">Don't supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b53d8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b53d8-128">Response</span></span>
<span data-ttu-id="b53d8-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b53d8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b53d8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b53d8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b53d8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b53d8-132">Request</span></span>
<span data-ttu-id="b53d8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b53d8-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b53d8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b53d8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="b53d8-135">C#</span><span class="sxs-lookup"><span data-stu-id="b53d8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b53d8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b53d8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b53d8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b53d8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b53d8-138">Java</span><span class="sxs-lookup"><span data-stu-id="b53d8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b53d8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b53d8-139">Response</span></span>
<span data-ttu-id="b53d8-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b53d8-140">The following is an example of the response.</span></span> 


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


