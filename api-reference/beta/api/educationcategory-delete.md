---
title: Удаление Едукатионкатегори
description: Удаление существующей категории.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2ae8d378760989b13e9597e86be01a2c5a6140cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427076"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="8c63a-103">Удаление Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="8c63a-103">Delete educationCategory</span></span>

<span data-ttu-id="8c63a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c63a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c63a-105">Удаление существующей категории.</span><span class="sxs-lookup"><span data-stu-id="8c63a-105">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c63a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c63a-106">Permissions</span></span>

<span data-ttu-id="8c63a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c63a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c63a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c63a-109">Permission type</span></span>                        | <span data-ttu-id="8c63a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c63a-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="8c63a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c63a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c63a-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c63a-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8c63a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c63a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c63a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c63a-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="8c63a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c63a-115">Application</span></span>                            | <span data-ttu-id="8c63a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c63a-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="8c63a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c63a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8c63a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c63a-118">Request headers</span></span>

| <span data-ttu-id="8c63a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c63a-119">Header</span></span>        | <span data-ttu-id="8c63a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8c63a-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="8c63a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c63a-121">Authorization</span></span> | <span data-ttu-id="8c63a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c63a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c63a-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c63a-124">Request body</span></span>

<span data-ttu-id="8c63a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c63a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c63a-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c63a-126">Response</span></span>

<span data-ttu-id="8c63a-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8c63a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c63a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="8c63a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c63a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c63a-130">Request</span></span>

<span data-ttu-id="8c63a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c63a-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8c63a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c63a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="c"></a>[<span data-ttu-id="8c63a-133">C#</span><span class="sxs-lookup"><span data-stu-id="8c63a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c63a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c63a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c63a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c63a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c63a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="8c63a-136">Response</span></span>

<span data-ttu-id="8c63a-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8c63a-137">The following is an example of the response.</span></span> 

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
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
