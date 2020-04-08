---
title: Удаление Цертификатебаседаусконфигуратион
description: Удаление Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f549c29015f5352fc9674ecd0a0c1a1422b125d3
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181065"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="44eae-103">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="44eae-103">Delete certificateBasedAuthConfiguration</span></span>

<span data-ttu-id="44eae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44eae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44eae-105">Удаление объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="44eae-105">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44eae-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44eae-106">Permissions</span></span>

<span data-ttu-id="44eae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44eae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44eae-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44eae-109">Permission type</span></span>                        | <span data-ttu-id="44eae-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44eae-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="44eae-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44eae-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="44eae-112">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44eae-112">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="44eae-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44eae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44eae-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44eae-114">Not supported.</span></span> |
| <span data-ttu-id="44eae-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44eae-115">Application</span></span>    | <span data-ttu-id="44eae-116">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44eae-116">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44eae-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44eae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="44eae-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44eae-118">Request headers</span></span>

| <span data-ttu-id="44eae-119">Имя</span><span class="sxs-lookup"><span data-stu-id="44eae-119">Name</span></span>          | <span data-ttu-id="44eae-120">Описание</span><span class="sxs-lookup"><span data-stu-id="44eae-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="44eae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44eae-121">Authorization</span></span> | <span data-ttu-id="44eae-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="44eae-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="44eae-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44eae-123">Request body</span></span>

<span data-ttu-id="44eae-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44eae-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44eae-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="44eae-125">Response</span></span>

<span data-ttu-id="44eae-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="44eae-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44eae-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="44eae-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="44eae-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="44eae-129">Request</span></span>

<span data-ttu-id="44eae-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44eae-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="44eae-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="44eae-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="c"></a>[<span data-ttu-id="44eae-132">C#</span><span class="sxs-lookup"><span data-stu-id="44eae-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="44eae-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44eae-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="44eae-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="44eae-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="44eae-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="44eae-135">Response</span></span>

<span data-ttu-id="44eae-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="44eae-136">The following is an example of the response.</span></span>

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
