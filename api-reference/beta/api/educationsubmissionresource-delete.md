---
title: Удаление Едукатионсубмиссионресаурце
description: Удаляет ресурс из отправки. Это может сделать только студентом. Если ресурс был скопирован из назначения, то после удаления текущей копии будет создан новый экземпляр ресурса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ffba53cee0cd3038db3e97fab2ff3a27c881bed3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424731"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="64c74-105">Удаление Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="64c74-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="64c74-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="64c74-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64c74-107">Удаляет ресурс из отправки.</span><span class="sxs-lookup"><span data-stu-id="64c74-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="64c74-108">Это может сделать только студентом.</span><span class="sxs-lookup"><span data-stu-id="64c74-108">This can only be done by the student.</span></span> <span data-ttu-id="64c74-109">Если ресурс был скопирован из назначения, то после удаления текущей копии будет создан новый экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="64c74-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="64c74-110">Это позволяет «сбросить» ресурс в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="64c74-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="64c74-111">Если ресурс не был скопирован из назначения, но добавлен из учащегося, ресурс просто удаляется.</span><span class="sxs-lookup"><span data-stu-id="64c74-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="64c74-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64c74-112">Permissions</span></span>
<span data-ttu-id="64c74-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64c74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64c74-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64c74-115">Permission type</span></span>      | <span data-ttu-id="64c74-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64c74-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64c74-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64c74-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="64c74-118">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64c74-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="64c74-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64c74-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="64c74-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c74-120">Not supported.</span></span>  |
|<span data-ttu-id="64c74-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64c74-121">Application</span></span> | <span data-ttu-id="64c74-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c74-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="64c74-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64c74-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="64c74-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64c74-124">Request headers</span></span>
| <span data-ttu-id="64c74-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64c74-125">Header</span></span>       | <span data-ttu-id="64c74-126">Значение</span><span class="sxs-lookup"><span data-stu-id="64c74-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64c74-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64c74-127">Authorization</span></span>  | <span data-ttu-id="64c74-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64c74-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64c74-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64c74-130">Request body</span></span>
<span data-ttu-id="64c74-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64c74-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="64c74-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c74-132">Response</span></span>
<span data-ttu-id="64c74-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64c74-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64c74-135">Пример</span><span class="sxs-lookup"><span data-stu-id="64c74-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64c74-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="64c74-136">Request</span></span>
<span data-ttu-id="64c74-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64c74-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="64c74-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="64c74-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="64c74-139">C#</span><span class="sxs-lookup"><span data-stu-id="64c74-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64c74-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64c74-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64c74-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64c74-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64c74-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c74-142">Response</span></span>
<span data-ttu-id="64c74-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="64c74-143">The following is an example of the response.</span></span> 

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
