---
title: Удаление educationAssignmentResource
description: Удалите определенный ресурс, присоединенный к назначению.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7e853534998978f89e44cbd8f657a56250c599a0
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911909"
---
# <a name="delete-educationassignmentresource"></a><span data-ttu-id="96aa2-103">Удаление educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="96aa2-103">Delete educationAssignmentResource</span></span>

<span data-ttu-id="96aa2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96aa2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96aa2-105">Удалите определенный ресурс, присоединенный к назначению.</span><span class="sxs-lookup"><span data-stu-id="96aa2-105">Delete a specific resource attached to an assignment.</span></span> <span data-ttu-id="96aa2-106">Удалить ресурс могут только преподаватели в классе.</span><span class="sxs-lookup"><span data-stu-id="96aa2-106">Only teachers in the class can remove a resource.</span></span> <span data-ttu-id="96aa2-107">После публикации задания учащимся преподаватели не могут удалять ресурсы, помеченные как "distributeToStudents".</span><span class="sxs-lookup"><span data-stu-id="96aa2-107">After an assignment has been published to students, teachers cannot remove resources that are marked as "distributeToStudents".</span></span>

## <a name="permissions"></a><span data-ttu-id="96aa2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96aa2-108">Permissions</span></span>
<span data-ttu-id="96aa2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96aa2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96aa2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96aa2-111">Permission type</span></span>      | <span data-ttu-id="96aa2-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96aa2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96aa2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96aa2-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="96aa2-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96aa2-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="96aa2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96aa2-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="96aa2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96aa2-116">Not supported.</span></span>  |
|<span data-ttu-id="96aa2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96aa2-117">Application</span></span> | <span data-ttu-id="96aa2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96aa2-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="96aa2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96aa2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="96aa2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96aa2-120">Request headers</span></span>
| <span data-ttu-id="96aa2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96aa2-121">Header</span></span>       | <span data-ttu-id="96aa2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="96aa2-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96aa2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96aa2-123">Authorization</span></span>  | <span data-ttu-id="96aa2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96aa2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96aa2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96aa2-126">Request body</span></span>
<span data-ttu-id="96aa2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96aa2-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="96aa2-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="96aa2-128">Response</span></span>
<span data-ttu-id="96aa2-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="96aa2-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96aa2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="96aa2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96aa2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="96aa2-132">Request</span></span>
<span data-ttu-id="96aa2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96aa2-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96aa2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="96aa2-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "delete_educationassignmentresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="c"></a>[<span data-ttu-id="96aa2-135">C#</span><span class="sxs-lookup"><span data-stu-id="96aa2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96aa2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96aa2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96aa2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96aa2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96aa2-138">Java</span><span class="sxs-lookup"><span data-stu-id="96aa2-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96aa2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="96aa2-139">Response</span></span>
<span data-ttu-id="96aa2-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="96aa2-140">The following is an example of the response.</span></span> 


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


