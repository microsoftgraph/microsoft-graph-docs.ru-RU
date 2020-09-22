---
title: Удаление Цертификатебаседаусконфигуратион
description: Удаление Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fe31837442897822346c4c5cf38b71ea4913a775
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983363"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="7dc21-103">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="7dc21-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="7dc21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dc21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dc21-105">Удаление объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7dc21-105">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dc21-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7dc21-106">Permissions</span></span>

<span data-ttu-id="7dc21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dc21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7dc21-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7dc21-109">Permission type</span></span>                        | <span data-ttu-id="7dc21-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7dc21-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7dc21-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7dc21-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7dc21-112">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc21-112">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="7dc21-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7dc21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dc21-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dc21-114">Not supported.</span></span> |
| <span data-ttu-id="7dc21-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7dc21-115">Application</span></span>    | <span data-ttu-id="7dc21-116">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dc21-116">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dc21-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7dc21-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7dc21-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7dc21-118">Request headers</span></span>

| <span data-ttu-id="7dc21-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7dc21-119">Name</span></span>          | <span data-ttu-id="7dc21-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7dc21-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7dc21-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dc21-121">Authorization</span></span> | <span data-ttu-id="7dc21-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="7dc21-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dc21-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7dc21-123">Request body</span></span>

<span data-ttu-id="7dc21-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7dc21-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dc21-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dc21-125">Response</span></span>

<span data-ttu-id="7dc21-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7dc21-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7dc21-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7dc21-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7dc21-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7dc21-129">Request</span></span>

<span data-ttu-id="7dc21-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7dc21-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7dc21-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dc21-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="7dc21-132">C#</span><span class="sxs-lookup"><span data-stu-id="7dc21-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dc21-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dc21-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dc21-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dc21-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7dc21-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7dc21-135">Response</span></span>

<span data-ttu-id="7dc21-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7dc21-136">The following is an example of the response.</span></span>

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


