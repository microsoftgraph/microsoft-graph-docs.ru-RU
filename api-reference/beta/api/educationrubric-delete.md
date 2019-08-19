---
title: Удаление Едукатионрубрик
description: Удаление объекта Едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2d9d3b67ec4ef0ef8bdd6684489630228355e3d1
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461091"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="8ecf6-103">Удаление Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="8ecf6-103">Delete educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ecf6-104">Удаление объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="8ecf6-104">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ecf6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ecf6-105">Permissions</span></span>

<span data-ttu-id="8ecf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ecf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ecf6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ecf6-108">Permission type</span></span>                        | <span data-ttu-id="8ecf6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ecf6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8ecf6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ecf6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ecf6-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ecf6-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8ecf6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ecf6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ecf6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-113">Not supported.</span></span> |
| <span data-ttu-id="8ecf6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ecf6-114">Application</span></span>                            | <span data-ttu-id="8ecf6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ecf6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ecf6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8ecf6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ecf6-117">Request headers</span></span>

| <span data-ttu-id="8ecf6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8ecf6-118">Name</span></span>          | <span data-ttu-id="8ecf6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8ecf6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8ecf6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ecf6-120">Authorization</span></span> | <span data-ttu-id="8ecf6-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8ecf6-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ecf6-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8ecf6-122">Request body</span></span>

<span data-ttu-id="8ecf6-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ecf6-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ecf6-124">Response</span></span>

<span data-ttu-id="8ecf6-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ecf6-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="8ecf6-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ecf6-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ecf6-128">Request</span></span>

<span data-ttu-id="8ecf6-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8ecf6-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ecf6-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8ecf6-131">C#</span><span class="sxs-lookup"><span data-stu-id="8ecf6-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8ecf6-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ecf6-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8ecf6-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8ecf6-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8ecf6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ecf6-134">Response</span></span>

<span data-ttu-id="8ecf6-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8ecf6-135">The following is an example of the response.</span></span>

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
