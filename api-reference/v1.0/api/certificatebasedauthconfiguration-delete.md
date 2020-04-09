---
title: Удаление Цертификатебаседаусконфигуратион
description: Удаление Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ca0722a3aa9c0ab778c9964cfee043afc47e30b
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181703"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="7496e-103">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7496e-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="7496e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7496e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7496e-105">Удаление объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7496e-105">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7496e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7496e-106">Permissions</span></span>

<span data-ttu-id="7496e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7496e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7496e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7496e-109">Permission type</span></span>                        | <span data-ttu-id="7496e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7496e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7496e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7496e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7496e-112">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7496e-112">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="7496e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7496e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7496e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7496e-114">Not supported.</span></span> |
| <span data-ttu-id="7496e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7496e-115">Application</span></span>    | <span data-ttu-id="7496e-116">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7496e-116">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7496e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7496e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7496e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7496e-118">Request headers</span></span>

| <span data-ttu-id="7496e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7496e-119">Name</span></span>          | <span data-ttu-id="7496e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7496e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7496e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7496e-121">Authorization</span></span> | <span data-ttu-id="7496e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7496e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7496e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7496e-124">Request body</span></span>

<span data-ttu-id="7496e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7496e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7496e-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="7496e-126">Response</span></span>

<span data-ttu-id="7496e-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7496e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7496e-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="7496e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7496e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7496e-130">Request</span></span>

<span data-ttu-id="7496e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7496e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7496e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7496e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="7496e-133">C#</span><span class="sxs-lookup"><span data-stu-id="7496e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7496e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7496e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7496e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7496e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7496e-136">Java</span><span class="sxs-lookup"><span data-stu-id="7496e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7496e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7496e-137">Response</span></span>

<span data-ttu-id="7496e-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7496e-138">The following is an example of the response.</span></span>

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
