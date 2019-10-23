---
title: Удаление Цертификатебаседаусконфигуратион
description: Удаление Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 113823fcb19014255b8334fb88f6a9f897eace8b
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37632562"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="81f52-103">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="81f52-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="81f52-104">Удаление объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="81f52-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81f52-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81f52-105">Permissions</span></span>

<span data-ttu-id="81f52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81f52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81f52-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81f52-108">Permission type</span></span>                        | <span data-ttu-id="81f52-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81f52-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="81f52-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81f52-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="81f52-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f52-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="81f52-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81f52-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81f52-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81f52-113">Not supported.</span></span> |
| <span data-ttu-id="81f52-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="81f52-114">Application</span></span>    | <span data-ttu-id="81f52-115">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81f52-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81f52-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81f52-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="81f52-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81f52-117">Request headers</span></span>

| <span data-ttu-id="81f52-118">Имя</span><span class="sxs-lookup"><span data-stu-id="81f52-118">Name</span></span>          | <span data-ttu-id="81f52-119">Описание</span><span class="sxs-lookup"><span data-stu-id="81f52-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="81f52-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81f52-120">Authorization</span></span> | <span data-ttu-id="81f52-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81f52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81f52-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81f52-123">Request body</span></span>

<span data-ttu-id="81f52-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81f52-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81f52-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="81f52-125">Response</span></span>

<span data-ttu-id="81f52-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="81f52-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81f52-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="81f52-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81f52-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="81f52-129">Request</span></span>

<span data-ttu-id="81f52-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81f52-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81f52-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="81f52-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="81f52-132">C#</span><span class="sxs-lookup"><span data-stu-id="81f52-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81f52-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81f52-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81f52-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81f52-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="81f52-135">Java</span><span class="sxs-lookup"><span data-stu-id="81f52-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81f52-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="81f52-136">Response</span></span>

<span data-ttu-id="81f52-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="81f52-137">The following is an example of the response.</span></span>

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
