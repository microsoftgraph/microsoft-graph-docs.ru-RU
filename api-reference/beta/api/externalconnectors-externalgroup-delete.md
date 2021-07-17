---
title: Удаление externalGroup
description: Удаляет объект externalGroup.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 4b415075dbcd47ecf8d3ad1e92fbf410863ba2d8
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467673"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="cc00d-103">Удаление externalGroup</span><span class="sxs-lookup"><span data-stu-id="cc00d-103">Delete externalGroup</span></span>

<span data-ttu-id="cc00d-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="cc00d-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc00d-105">Удаление [объекта externalGroup.](../resources/externalconnectors-externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="cc00d-105">Delete an [externalGroup](../resources/externalconnectors-externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc00d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc00d-106">Permissions</span></span>

<span data-ttu-id="cc00d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc00d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc00d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc00d-109">Permission type</span></span>                        | <span data-ttu-id="cc00d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc00d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cc00d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc00d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc00d-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cc00d-112">Not supported</span></span>                               |
| <span data-ttu-id="cc00d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc00d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc00d-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="cc00d-114">Not supported</span></span>                               |
| <span data-ttu-id="cc00d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cc00d-115">Application</span></span>                            | <span data-ttu-id="cc00d-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc00d-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="cc00d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc00d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="cc00d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc00d-118">Request headers</span></span>

| <span data-ttu-id="cc00d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cc00d-119">Name</span></span>          | <span data-ttu-id="cc00d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cc00d-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cc00d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc00d-121">Authorization</span></span> | <span data-ttu-id="cc00d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc00d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc00d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc00d-124">Request body</span></span>

<span data-ttu-id="cc00d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc00d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc00d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc00d-126">Response</span></span>

<span data-ttu-id="cc00d-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cc00d-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cc00d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="cc00d-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cc00d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc00d-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cc00d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc00d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```
# <a name="c"></a>[<span data-ttu-id="cc00d-131">C#</span><span class="sxs-lookup"><span data-stu-id="cc00d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc00d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc00d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc00d-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc00d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc00d-134">Java</span><span class="sxs-lookup"><span data-stu-id="cc00d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="cc00d-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc00d-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
