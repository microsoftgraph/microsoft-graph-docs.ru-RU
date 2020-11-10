---
title: Удаление Цертификатебаседаусконфигуратион
description: Удаление Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7baac52887e83b431bd76029849cb8c24207dac7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959453"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="8f6aa-103">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8f6aa-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="8f6aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f6aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f6aa-105">Удаление объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8f6aa-105">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f6aa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f6aa-106">Permissions</span></span>

<span data-ttu-id="8f6aa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f6aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f6aa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f6aa-109">Permission type</span></span>                        | <span data-ttu-id="8f6aa-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f6aa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f6aa-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f6aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f6aa-112">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f6aa-112">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="8f6aa-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f6aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f6aa-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f6aa-114">Not supported.</span></span> |
| <span data-ttu-id="8f6aa-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f6aa-115">Application</span></span>    | <span data-ttu-id="8f6aa-116">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f6aa-116">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f6aa-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f6aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8f6aa-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f6aa-118">Request headers</span></span>

| <span data-ttu-id="8f6aa-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8f6aa-119">Name</span></span>          | <span data-ttu-id="8f6aa-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8f6aa-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8f6aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f6aa-121">Authorization</span></span> | <span data-ttu-id="8f6aa-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8f6aa-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f6aa-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f6aa-123">Request body</span></span>

<span data-ttu-id="8f6aa-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f6aa-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f6aa-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f6aa-125">Response</span></span>

<span data-ttu-id="8f6aa-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8f6aa-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8f6aa-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f6aa-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f6aa-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f6aa-129">Request</span></span>

<span data-ttu-id="8f6aa-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f6aa-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8f6aa-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f6aa-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="8f6aa-132">C#</span><span class="sxs-lookup"><span data-stu-id="8f6aa-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f6aa-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f6aa-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f6aa-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f6aa-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f6aa-135">Java</span><span class="sxs-lookup"><span data-stu-id="8f6aa-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-certificatebasedauthconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f6aa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f6aa-136">Response</span></span>

<span data-ttu-id="8f6aa-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f6aa-137">The following is an example of the response.</span></span>

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


