---
title: Удаление educationAssignment
description: Удаление существующего назначения. Удалять назначения могут только преподаватели внутри класса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 39d26a7fdc20ec7a28e89d1186733821f5189850
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436181"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="d5462-104">Удаление educationAssignment</span><span class="sxs-lookup"><span data-stu-id="d5462-104">Delete educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5462-105">Удаление существующего назначения.</span><span class="sxs-lookup"><span data-stu-id="d5462-105">Delete an existing assignment.</span></span> <span data-ttu-id="d5462-106">Удалять назначения могут только преподаватели внутри класса.</span><span class="sxs-lookup"><span data-stu-id="d5462-106">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5462-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5462-107">Permissions</span></span>

<span data-ttu-id="d5462-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5462-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5462-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5462-110">Permission type</span></span>                        | <span data-ttu-id="d5462-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5462-111">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="d5462-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5462-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5462-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5462-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d5462-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5462-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5462-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5462-115">Not Supported.</span></span>                                          |
| <span data-ttu-id="d5462-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5462-116">Application</span></span>                            | <span data-ttu-id="d5462-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5462-117">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="d5462-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5462-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d5462-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5462-119">Request headers</span></span>

| <span data-ttu-id="d5462-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5462-120">Header</span></span>        | <span data-ttu-id="d5462-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d5462-121">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d5462-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5462-122">Authorization</span></span> | <span data-ttu-id="d5462-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5462-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5462-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5462-125">Request body</span></span>

<span data-ttu-id="d5462-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5462-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5462-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5462-127">Response</span></span>

<span data-ttu-id="d5462-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d5462-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5462-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d5462-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5462-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5462-131">Request</span></span>

<span data-ttu-id="d5462-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5462-132">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d5462-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5462-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5462-134">C#</span><span class="sxs-lookup"><span data-stu-id="d5462-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5462-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="d5462-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5462-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d5462-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d5462-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5462-137">Response</span></span>
<span data-ttu-id="d5462-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d5462-138">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
