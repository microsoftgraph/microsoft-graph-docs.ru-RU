---
title: Удаление Усерфлов
description: Удаление Усерфлов.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8750ecc9770d0b067704c271b7b7bc898d57d542
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938053"
---
# <a name="delete-userflow"></a><span data-ttu-id="30d1d-103">Удаление Усерфлов</span><span class="sxs-lookup"><span data-stu-id="30d1d-103">Delete userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30d1d-104">Удаление существующего объекта [усерфлов](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="30d1d-104">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="30d1d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30d1d-105">Permissions</span></span>

<span data-ttu-id="30d1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30d1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30d1d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30d1d-108">Permission type</span></span>                        | <span data-ttu-id="30d1d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30d1d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="30d1d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30d1d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="30d1d-111">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="30d1d-111">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="30d1d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30d1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30d1d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30d1d-113">Not supported.</span></span> |
| <span data-ttu-id="30d1d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30d1d-114">Application</span></span>                            | <span data-ttu-id="30d1d-115">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="30d1d-115">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30d1d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30d1d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="30d1d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30d1d-117">Request headers</span></span>

| <span data-ttu-id="30d1d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="30d1d-118">Name</span></span>          | <span data-ttu-id="30d1d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="30d1d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="30d1d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30d1d-120">Authorization</span></span> | <span data-ttu-id="30d1d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30d1d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30d1d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30d1d-123">Request body</span></span>

<span data-ttu-id="30d1d-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30d1d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30d1d-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="30d1d-125">Response</span></span>

<span data-ttu-id="30d1d-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="30d1d-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30d1d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="30d1d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="30d1d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="30d1d-129">Request</span></span>

<span data-ttu-id="30d1d-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30d1d-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="30d1d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="30d1d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30d1d-132">C#</span><span class="sxs-lookup"><span data-stu-id="30d1d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30d1d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30d1d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30d1d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30d1d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30d1d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="30d1d-135">Response</span></span>

<span data-ttu-id="30d1d-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="30d1d-136">The following is an example of the response.</span></span>

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
  "description": "Delete userFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
