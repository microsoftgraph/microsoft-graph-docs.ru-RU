---
title: Удаление Едисковерикасе
description: Удаление объекта Едисковерикасе.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 836e510906e0e35ce1a1be4b8a6556d0467e9e10
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966783"
---
# <a name="delete-ediscoverycase"></a><span data-ttu-id="db292-103">Удаление Едисковерикасе</span><span class="sxs-lookup"><span data-stu-id="db292-103">Delete ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db292-104">Удаление объекта [едисковерикасе](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="db292-104">Delete an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db292-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db292-105">Permissions</span></span>

<span data-ttu-id="db292-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db292-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db292-108">Permission type</span></span>                        | <span data-ttu-id="db292-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db292-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db292-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db292-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="db292-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="db292-111">User.Read</span></span>      |
| <span data-ttu-id="db292-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db292-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db292-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db292-113">Not supported.</span></span> |
| <span data-ttu-id="db292-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db292-114">Application</span></span>                            | <span data-ttu-id="db292-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db292-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db292-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db292-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="db292-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db292-117">Request headers</span></span>

| <span data-ttu-id="db292-118">Имя</span><span class="sxs-lookup"><span data-stu-id="db292-118">Name</span></span>          | <span data-ttu-id="db292-119">Описание</span><span class="sxs-lookup"><span data-stu-id="db292-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="db292-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db292-120">Authorization</span></span> | <span data-ttu-id="db292-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db292-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db292-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db292-123">Request body</span></span>

<span data-ttu-id="db292-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db292-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db292-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="db292-125">Response</span></span>

<span data-ttu-id="db292-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="db292-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db292-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="db292-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db292-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="db292-129">Request</span></span>

<span data-ttu-id="db292-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db292-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db292-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="db292-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_ediscoverycase"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```
# <a name="c"></a>[<span data-ttu-id="db292-132">C#</span><span class="sxs-lookup"><span data-stu-id="db292-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db292-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db292-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db292-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db292-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db292-135">Java</span><span class="sxs-lookup"><span data-stu-id="db292-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db292-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db292-136">Response</span></span>

<span data-ttu-id="db292-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="db292-137">The following is an example of the response.</span></span>

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
  "description": "Delete ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


