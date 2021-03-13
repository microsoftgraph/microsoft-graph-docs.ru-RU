---
title: Удаление случая
description: Удаление объекта дела.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: eeedaacb05ea4c846a79739d30f7d0c329d88fcf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776762"
---
# <a name="delete-case"></a><span data-ttu-id="3cde2-103">Удаление случая</span><span class="sxs-lookup"><span data-stu-id="3cde2-103">Delete case</span></span>

<span data-ttu-id="3cde2-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3cde2-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cde2-105">Удаление [объекта дела.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="3cde2-105">Delete a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cde2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cde2-106">Permissions</span></span>

<span data-ttu-id="3cde2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cde2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cde2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cde2-109">Permission type</span></span>|<span data-ttu-id="3cde2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cde2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cde2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cde2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3cde2-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cde2-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="3cde2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cde2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cde2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cde2-114">Not supported.</span></span>|
|<span data-ttu-id="3cde2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cde2-115">Application</span></span>|<span data-ttu-id="3cde2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cde2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cde2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cde2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3cde2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cde2-118">Request headers</span></span>

| <span data-ttu-id="3cde2-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3cde2-119">Name</span></span>          | <span data-ttu-id="3cde2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3cde2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3cde2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cde2-121">Authorization</span></span> | <span data-ttu-id="3cde2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cde2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cde2-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cde2-124">Request body</span></span>

<span data-ttu-id="3cde2-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3cde2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cde2-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cde2-126">Response</span></span>

<span data-ttu-id="3cde2-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3cde2-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="3cde2-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3cde2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cde2-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cde2-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3cde2-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cde2-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_case"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```

# <a name="c"></a>[<span data-ttu-id="3cde2-131">C#</span><span class="sxs-lookup"><span data-stu-id="3cde2-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cde2-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cde2-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cde2-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cde2-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cde2-134">Java</span><span class="sxs-lookup"><span data-stu-id="3cde2-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3cde2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cde2-135">Response</span></span>

<span data-ttu-id="3cde2-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3cde2-136">The following is an example of the response.</span></span>

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
  "description": "Delete case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
