---
title: Удаление educationUser
description: Удаление пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c753c30b1bdc00a5375affeef22f324193a577d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42423961"
---
# <a name="delete-educationuser"></a><span data-ttu-id="baedc-103">Удаление educationUser</span><span class="sxs-lookup"><span data-stu-id="baedc-103">Delete educationUser</span></span>

<span data-ttu-id="baedc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="baedc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baedc-105">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="baedc-105">Delete a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="baedc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="baedc-106">Permissions</span></span>

<span data-ttu-id="baedc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baedc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="baedc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="baedc-109">Permission type</span></span>                        | <span data-ttu-id="baedc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="baedc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="baedc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="baedc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="baedc-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baedc-112">Not supported.</span></span>                              |
| <span data-ttu-id="baedc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="baedc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baedc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baedc-114">Not supported.</span></span>                              |
| <span data-ttu-id="baedc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="baedc-115">Application</span></span>                            | <span data-ttu-id="baedc-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baedc-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="baedc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="baedc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="baedc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="baedc-118">Request headers</span></span>

| <span data-ttu-id="baedc-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="baedc-119">Header</span></span>        | <span data-ttu-id="baedc-120">Значение</span><span class="sxs-lookup"><span data-stu-id="baedc-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="baedc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="baedc-121">Authorization</span></span> | <span data-ttu-id="baedc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baedc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="baedc-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="baedc-124">Request body</span></span>

<span data-ttu-id="baedc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="baedc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="baedc-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="baedc-126">Response</span></span>

<span data-ttu-id="baedc-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="baedc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baedc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="baedc-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="baedc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="baedc-130">Request</span></span>

<span data-ttu-id="baedc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="baedc-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="baedc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="baedc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
# <a name="c"></a>[<span data-ttu-id="baedc-133">C#</span><span class="sxs-lookup"><span data-stu-id="baedc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="baedc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="baedc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="baedc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="baedc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="baedc-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="baedc-136">Response</span></span>

<span data-ttu-id="baedc-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="baedc-137">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
