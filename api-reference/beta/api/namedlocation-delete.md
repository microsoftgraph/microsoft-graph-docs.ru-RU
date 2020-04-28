---
title: Удаление Намедлокатион
description: Удаление объекта Намедлокатион.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a8f4fb240d2b2966f6f5fdb00fc43dc5683fb67c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448422"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="6f61f-103">Удаление Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="6f61f-103">Delete namedLocation</span></span>

<span data-ttu-id="6f61f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f61f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f61f-105">Удаление объекта [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f61f-105">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f61f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f61f-106">Permissions</span></span>

<span data-ttu-id="6f61f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f61f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f61f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f61f-109">Permission type</span></span>                        | <span data-ttu-id="6f61f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f61f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6f61f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f61f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f61f-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="6f61f-112">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="6f61f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f61f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f61f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f61f-114">Not supported.</span></span> |
| <span data-ttu-id="6f61f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f61f-115">Application</span></span>                            | <span data-ttu-id="6f61f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f61f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f61f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f61f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6f61f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f61f-118">Request headers</span></span>

| <span data-ttu-id="6f61f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6f61f-119">Name</span></span>          | <span data-ttu-id="6f61f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6f61f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6f61f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f61f-121">Authorization</span></span> | <span data-ttu-id="6f61f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f61f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f61f-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f61f-124">Request body</span></span>

<span data-ttu-id="6f61f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f61f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f61f-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f61f-126">Response</span></span>

<span data-ttu-id="6f61f-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6f61f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f61f-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="6f61f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6f61f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f61f-130">Request</span></span>

<span data-ttu-id="6f61f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f61f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f61f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f61f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="6f61f-133">C#</span><span class="sxs-lookup"><span data-stu-id="6f61f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-namedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f61f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f61f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-namedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f61f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f61f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-namedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6f61f-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f61f-136">Response</span></span>

<span data-ttu-id="6f61f-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f61f-137">The following is an example of the response.</span></span>

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
  "description": "Delete namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
