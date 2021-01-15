---
title: Удаление externalGroup
description: Удаляет объект externalGroup.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: a039ab9969766a6fa1716c481c0d74f5b8bf125d
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873187"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="7bfe7-103">Удаление externalGroup</span><span class="sxs-lookup"><span data-stu-id="7bfe7-103">Delete externalGroup</span></span>

<span data-ttu-id="7bfe7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bfe7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bfe7-105">Удаление объекта [externalGroup.](../resources/externalgroup.md)</span><span class="sxs-lookup"><span data-stu-id="7bfe7-105">Delete an [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bfe7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bfe7-106">Permissions</span></span>

<span data-ttu-id="7bfe7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bfe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7bfe7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bfe7-109">Permission type</span></span>                        | <span data-ttu-id="7bfe7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bfe7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7bfe7-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bfe7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bfe7-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7bfe7-112">Not supported</span></span>                               |
| <span data-ttu-id="7bfe7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bfe7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bfe7-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="7bfe7-114">Not supported</span></span>                               |
| <span data-ttu-id="7bfe7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="7bfe7-115">Application</span></span>                            | <span data-ttu-id="7bfe7-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bfe7-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="7bfe7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bfe7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="7bfe7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bfe7-118">Request headers</span></span>

| <span data-ttu-id="7bfe7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7bfe7-119">Name</span></span>          | <span data-ttu-id="7bfe7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7bfe7-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7bfe7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bfe7-121">Authorization</span></span> | <span data-ttu-id="7bfe7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bfe7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bfe7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bfe7-124">Request body</span></span>

<span data-ttu-id="7bfe7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7bfe7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bfe7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bfe7-126">Response</span></span>

<span data-ttu-id="7bfe7-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7bfe7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7bfe7-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7bfe7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7bfe7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bfe7-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7bfe7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bfe7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```
# <a name="c"></a>[<span data-ttu-id="7bfe7-131">C#</span><span class="sxs-lookup"><span data-stu-id="7bfe7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bfe7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bfe7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bfe7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bfe7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7bfe7-134">Java</span><span class="sxs-lookup"><span data-stu-id="7bfe7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="7bfe7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bfe7-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
