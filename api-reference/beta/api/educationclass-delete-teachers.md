---
title: Удаление преподавателя
description: Удаление преподавателя для курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a900c16e96d4cc91846de86b757987032ba2fd18
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426999"
---
# <a name="remove-teacher"></a><span data-ttu-id="2a8c8-103">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="2a8c8-103">Remove teacher</span></span>

<span data-ttu-id="2a8c8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2a8c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a8c8-105">Удаление преподавателя для курса.</span><span class="sxs-lookup"><span data-stu-id="2a8c8-105">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a8c8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a8c8-106">Permissions</span></span>

<span data-ttu-id="2a8c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a8c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a8c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a8c8-109">Permission type</span></span>                        | <span data-ttu-id="2a8c8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a8c8-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2a8c8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a8c8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a8c8-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a8c8-112">Not supported.</span></span>                              |
| <span data-ttu-id="2a8c8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a8c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a8c8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a8c8-114">Not supported.</span></span>                              |
| <span data-ttu-id="2a8c8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a8c8-115">Application</span></span>                            | <span data-ttu-id="2a8c8-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a8c8-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="2a8c8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a8c8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2a8c8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a8c8-118">Request headers</span></span>

| <span data-ttu-id="2a8c8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a8c8-119">Header</span></span>        | <span data-ttu-id="2a8c8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2a8c8-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="2a8c8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a8c8-121">Authorization</span></span> | <span data-ttu-id="2a8c8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a8c8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a8c8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a8c8-124">Request body</span></span>

<span data-ttu-id="2a8c8-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a8c8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a8c8-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a8c8-126">Response</span></span>

<span data-ttu-id="2a8c8-127">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="2a8c8-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a8c8-128">Пример</span><span class="sxs-lookup"><span data-stu-id="2a8c8-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2a8c8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a8c8-129">Request</span></span>

<span data-ttu-id="2a8c8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a8c8-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a8c8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a8c8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/{id}/teachers/14012
```
# <a name="c"></a>[<span data-ttu-id="2a8c8-132">C#</span><span class="sxs-lookup"><span data-stu-id="2a8c8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a8c8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a8c8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a8c8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a8c8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2a8c8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a8c8-135">Response</span></span>

<span data-ttu-id="2a8c8-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a8c8-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
