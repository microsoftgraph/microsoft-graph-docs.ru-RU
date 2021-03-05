---
title: Удаление certificateBasedAuthConfiguration
description: Удаление certificateBasedAuthConfiguration.
localization_priority: Normal
author: adimitui
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d4ae573fe7ef62dc673cbdab4d1f9df831a3f894
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434848"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="ed52d-103">Удаление certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed52d-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="ed52d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed52d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed52d-105">Удаление [объекта certificateBasedAuthConfiguration.](../resources/certificateBasedAuthConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ed52d-105">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed52d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed52d-106">Permissions</span></span>

<span data-ttu-id="ed52d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed52d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed52d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed52d-109">Permission type</span></span>                        | <span data-ttu-id="ed52d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed52d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ed52d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed52d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed52d-112">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed52d-112">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="ed52d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed52d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed52d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed52d-114">Not supported.</span></span> |
| <span data-ttu-id="ed52d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed52d-115">Application</span></span>    | <span data-ttu-id="ed52d-116">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed52d-116">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed52d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed52d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ed52d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed52d-118">Request headers</span></span>

| <span data-ttu-id="ed52d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ed52d-119">Name</span></span>          | <span data-ttu-id="ed52d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ed52d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ed52d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed52d-121">Authorization</span></span> | <span data-ttu-id="ed52d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed52d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed52d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ed52d-124">Request body</span></span>

<span data-ttu-id="ed52d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed52d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed52d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed52d-126">Response</span></span>

<span data-ttu-id="ed52d-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ed52d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed52d-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="ed52d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed52d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed52d-130">Request</span></span>

<span data-ttu-id="ed52d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed52d-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed52d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed52d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="ed52d-133">C#</span><span class="sxs-lookup"><span data-stu-id="ed52d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed52d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed52d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed52d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed52d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed52d-136">Java</span><span class="sxs-lookup"><span data-stu-id="ed52d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed52d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed52d-137">Response</span></span>

<span data-ttu-id="ed52d-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ed52d-138">The following is an example of the response.</span></span>

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
  "description": "Delete certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

