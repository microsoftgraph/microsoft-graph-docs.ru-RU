---
title: Удаление Усерфлов
description: Удаление Усерфлов.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d7a46184eef4a38ee13b961bc6cdbbaea15a888d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446459"
---
# <a name="delete-userflow"></a><span data-ttu-id="7e2b2-103">Удаление Усерфлов</span><span class="sxs-lookup"><span data-stu-id="7e2b2-103">Delete userFlow</span></span>

<span data-ttu-id="7e2b2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7e2b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e2b2-105">Удаление существующего объекта [усерфлов](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="7e2b2-105">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e2b2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e2b2-106">Permissions</span></span>

<span data-ttu-id="7e2b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e2b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e2b2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e2b2-109">Permission type</span></span>                        | <span data-ttu-id="7e2b2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e2b2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7e2b2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e2b2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e2b2-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7e2b2-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="7e2b2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e2b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e2b2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e2b2-114">Not supported.</span></span> |
| <span data-ttu-id="7e2b2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e2b2-115">Application</span></span>                            | <span data-ttu-id="7e2b2-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7e2b2-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e2b2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e2b2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7e2b2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7e2b2-118">Request headers</span></span>

| <span data-ttu-id="7e2b2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7e2b2-119">Name</span></span>          | <span data-ttu-id="7e2b2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7e2b2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7e2b2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7e2b2-121">Authorization</span></span> | <span data-ttu-id="7e2b2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e2b2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e2b2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7e2b2-124">Request body</span></span>

<span data-ttu-id="7e2b2-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e2b2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e2b2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e2b2-126">Response</span></span>

<span data-ttu-id="7e2b2-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7e2b2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e2b2-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="7e2b2-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e2b2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e2b2-130">Request</span></span>

<span data-ttu-id="7e2b2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e2b2-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e2b2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e2b2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="7e2b2-133">C#</span><span class="sxs-lookup"><span data-stu-id="7e2b2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e2b2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e2b2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e2b2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e2b2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7e2b2-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e2b2-136">Response</span></span>

<span data-ttu-id="7e2b2-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7e2b2-137">The following is an example of the response.</span></span>

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
