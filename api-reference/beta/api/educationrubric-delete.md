---
title: Удаление Едукатионрубрик
description: Удаление объекта Едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7ce4f5f3f7de8f57499a13130a776302378500a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425851"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="2e0e2-103">Удаление Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="2e0e2-103">Delete educationRubric</span></span>

<span data-ttu-id="2e0e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e0e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e0e2-105">Удаление объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="2e0e2-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e0e2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e0e2-106">Permissions</span></span>

<span data-ttu-id="2e0e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e0e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e0e2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e0e2-109">Permission type</span></span>                        | <span data-ttu-id="2e0e2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e0e2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2e0e2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e0e2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e0e2-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e0e2-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="2e0e2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e0e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e0e2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e0e2-114">Not supported.</span></span> |
| <span data-ttu-id="2e0e2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e0e2-115">Application</span></span>                            | <span data-ttu-id="2e0e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e0e2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e0e2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e0e2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2e0e2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e0e2-118">Request headers</span></span>

| <span data-ttu-id="2e0e2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="2e0e2-119">Name</span></span>          | <span data-ttu-id="2e0e2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2e0e2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2e0e2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e0e2-121">Authorization</span></span> | <span data-ttu-id="2e0e2-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2e0e2-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e0e2-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2e0e2-123">Request body</span></span>

<span data-ttu-id="2e0e2-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2e0e2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e0e2-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e0e2-125">Response</span></span>

<span data-ttu-id="2e0e2-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2e0e2-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e0e2-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="2e0e2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2e0e2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e0e2-129">Request</span></span>

<span data-ttu-id="2e0e2-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e0e2-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e0e2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e0e2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="c"></a>[<span data-ttu-id="2e0e2-132">C#</span><span class="sxs-lookup"><span data-stu-id="2e0e2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e0e2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e0e2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e0e2-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e0e2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e0e2-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="2e0e2-135">Response</span></span>

<span data-ttu-id="2e0e2-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2e0e2-136">The following is an example of the response.</span></span>

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
