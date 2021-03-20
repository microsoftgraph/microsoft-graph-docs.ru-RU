---
title: Удаление преподавателя
description: Удаление преподавателя для курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a60e6ea90387ee080317c523d7c9722780b44e6b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951638"
---
# <a name="remove-teacher"></a><span data-ttu-id="8e583-103">Удаление преподавателя</span><span class="sxs-lookup"><span data-stu-id="8e583-103">Remove teacher</span></span>

<span data-ttu-id="8e583-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e583-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e583-105">Удаление преподавателя для курса.</span><span class="sxs-lookup"><span data-stu-id="8e583-105">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e583-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e583-106">Permissions</span></span>

<span data-ttu-id="8e583-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e583-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e583-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e583-109">Permission type</span></span>                        | <span data-ttu-id="8e583-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e583-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="8e583-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e583-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e583-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e583-112">Not supported.</span></span>                              |
| <span data-ttu-id="8e583-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e583-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e583-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e583-114">Not supported.</span></span>                              |
| <span data-ttu-id="8e583-115">Application</span><span class="sxs-lookup"><span data-stu-id="8e583-115">Application</span></span>                            | <span data-ttu-id="8e583-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e583-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="8e583-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e583-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8e583-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e583-118">Request headers</span></span>

| <span data-ttu-id="8e583-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e583-119">Header</span></span>        | <span data-ttu-id="8e583-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8e583-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="8e583-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e583-121">Authorization</span></span> | <span data-ttu-id="8e583-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e583-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e583-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e583-124">Request body</span></span>

<span data-ttu-id="8e583-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e583-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e583-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e583-126">Response</span></span>

<span data-ttu-id="8e583-127">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="8e583-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e583-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8e583-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8e583-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e583-129">Request</span></span>

<span data-ttu-id="8e583-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e583-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8e583-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e583-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_2"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/{id}/teachers/14012
```
# <a name="c"></a>[<span data-ttu-id="8e583-132">C#</span><span class="sxs-lookup"><span data-stu-id="8e583-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e583-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e583-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e583-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e583-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e583-135">Java</span><span class="sxs-lookup"><span data-stu-id="8e583-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8e583-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e583-136">Response</span></span>

<span data-ttu-id="8e583-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e583-137">The following is an example of the response.</span></span> 

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


