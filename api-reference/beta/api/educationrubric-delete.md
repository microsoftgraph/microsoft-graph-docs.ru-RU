---
title: Удаление Едукатионрубрик
description: Удаление объекта Едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 277429b3b784ddb4607c3483c88375d401f457b3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002424"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="590ac-103">Удаление Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="590ac-103">Delete educationRubric</span></span>

<span data-ttu-id="590ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="590ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="590ac-105">Удаление объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="590ac-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="590ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="590ac-106">Permissions</span></span>

<span data-ttu-id="590ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="590ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="590ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="590ac-109">Permission type</span></span>                        | <span data-ttu-id="590ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="590ac-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="590ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="590ac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="590ac-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="590ac-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="590ac-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="590ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="590ac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="590ac-114">Not supported.</span></span> |
| <span data-ttu-id="590ac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="590ac-115">Application</span></span>                            | <span data-ttu-id="590ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="590ac-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="590ac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="590ac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="590ac-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="590ac-118">Request headers</span></span>

| <span data-ttu-id="590ac-119">Имя</span><span class="sxs-lookup"><span data-stu-id="590ac-119">Name</span></span>          | <span data-ttu-id="590ac-120">Описание</span><span class="sxs-lookup"><span data-stu-id="590ac-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="590ac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="590ac-121">Authorization</span></span> | <span data-ttu-id="590ac-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="590ac-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="590ac-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="590ac-123">Request body</span></span>

<span data-ttu-id="590ac-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="590ac-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="590ac-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="590ac-125">Response</span></span>

<span data-ttu-id="590ac-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="590ac-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="590ac-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="590ac-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="590ac-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="590ac-129">Request</span></span>

<span data-ttu-id="590ac-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="590ac-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="590ac-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="590ac-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="c"></a>[<span data-ttu-id="590ac-132">C#</span><span class="sxs-lookup"><span data-stu-id="590ac-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="590ac-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="590ac-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="590ac-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="590ac-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="590ac-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="590ac-135">Response</span></span>

<span data-ttu-id="590ac-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="590ac-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


