---
title: Удаление Усерфлов
description: Удаление Усерфлов.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6f864005497b90111a499a2733c83c33142a39e1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953313"
---
# <a name="delete-userflow"></a><span data-ttu-id="fa457-103">Удаление Усерфлов</span><span class="sxs-lookup"><span data-stu-id="fa457-103">Delete userFlow</span></span>

<span data-ttu-id="fa457-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa457-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa457-105">Удаление существующего объекта [усерфлов](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="fa457-105">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa457-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa457-106">Permissions</span></span>

<span data-ttu-id="fa457-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa457-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa457-109">Permission type</span></span>                        | <span data-ttu-id="fa457-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa457-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa457-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa457-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa457-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa457-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="fa457-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa457-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa457-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa457-114">Not supported.</span></span> |
| <span data-ttu-id="fa457-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa457-115">Application</span></span>                            | <span data-ttu-id="fa457-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa457-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa457-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa457-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fa457-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa457-118">Request headers</span></span>

| <span data-ttu-id="fa457-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fa457-119">Name</span></span>          | <span data-ttu-id="fa457-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fa457-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fa457-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa457-121">Authorization</span></span> | <span data-ttu-id="fa457-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa457-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa457-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa457-124">Request body</span></span>

<span data-ttu-id="fa457-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa457-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa457-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa457-126">Response</span></span>

<span data-ttu-id="fa457-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fa457-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa457-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="fa457-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa457-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa457-130">Request</span></span>

<span data-ttu-id="fa457-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa457-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa457-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa457-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="fa457-133">C#</span><span class="sxs-lookup"><span data-stu-id="fa457-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa457-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa457-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa457-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa457-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa457-136">Java</span><span class="sxs-lookup"><span data-stu-id="fa457-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fa457-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa457-137">Response</span></span>

<span data-ttu-id="fa457-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fa457-138">The following is an example of the response.</span></span>

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


