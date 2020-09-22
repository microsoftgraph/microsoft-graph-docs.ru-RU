---
title: Удаление индикатора службы угроз
description: Удаление объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: b5de10f7423294b0e9d0a044c6a8fcd7b0c831d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994367"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="a6905-103">Удаление индикатора службы угроз</span><span class="sxs-lookup"><span data-stu-id="a6905-103">Delete threat intelligence indicator</span></span>

<span data-ttu-id="a6905-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6905-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6905-105">Удаление объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="a6905-105">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6905-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6905-106">Permissions</span></span>

<span data-ttu-id="a6905-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6905-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6905-109">Permission type</span></span>                        | <span data-ttu-id="a6905-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6905-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a6905-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6905-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6905-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a6905-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="a6905-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6905-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6905-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6905-114">Not supported.</span></span> |
| <span data-ttu-id="a6905-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6905-115">Application</span></span>                            | <span data-ttu-id="a6905-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a6905-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6905-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6905-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a6905-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6905-118">Request headers</span></span>

| <span data-ttu-id="a6905-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a6905-119">Name</span></span>          | <span data-ttu-id="a6905-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a6905-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a6905-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6905-121">Authorization</span></span> | <span data-ttu-id="a6905-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a6905-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6905-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6905-123">Request body</span></span>

<span data-ttu-id="a6905-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6905-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6905-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6905-125">Response</span></span>

<span data-ttu-id="a6905-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a6905-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6905-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a6905-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6905-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6905-129">Request</span></span>

<span data-ttu-id="a6905-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6905-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6905-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6905-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="c"></a>[<span data-ttu-id="a6905-132">C#</span><span class="sxs-lookup"><span data-stu-id="a6905-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6905-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6905-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6905-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6905-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6905-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6905-135">Response</span></span>

<span data-ttu-id="a6905-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a6905-136">The following is an example of the response.</span></span>

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
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


