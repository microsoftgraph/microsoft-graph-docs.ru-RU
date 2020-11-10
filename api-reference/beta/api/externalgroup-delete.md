---
title: Удаление Екстерналграуп
description: Удаляет объект Екстерналграуп.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7cf287b7886cc9f0ee5cdb0d3e20ee5e43cb4ce5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954666"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="be0fc-103">Удаление Екстерналграуп</span><span class="sxs-lookup"><span data-stu-id="be0fc-103">Delete externalGroup</span></span>

<span data-ttu-id="be0fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be0fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be0fc-105">Удаление объекта [екстерналграуп](../resources/externalgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="be0fc-105">Delete an [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be0fc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="be0fc-106">Permissions</span></span>

<span data-ttu-id="be0fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be0fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be0fc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be0fc-109">Permission type</span></span>                        | <span data-ttu-id="be0fc-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be0fc-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be0fc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be0fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be0fc-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be0fc-112">Not supported</span></span>                               |
| <span data-ttu-id="be0fc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be0fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be0fc-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="be0fc-114">Not supported</span></span>                               |
| <span data-ttu-id="be0fc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be0fc-115">Application</span></span>                            | <span data-ttu-id="be0fc-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be0fc-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="be0fc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be0fc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="be0fc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be0fc-118">Request headers</span></span>

| <span data-ttu-id="be0fc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="be0fc-119">Name</span></span>          | <span data-ttu-id="be0fc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="be0fc-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="be0fc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be0fc-121">Authorization</span></span> | <span data-ttu-id="be0fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be0fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be0fc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be0fc-124">Request body</span></span>

<span data-ttu-id="be0fc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="be0fc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be0fc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="be0fc-126">Response</span></span>

<span data-ttu-id="be0fc-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="be0fc-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="be0fc-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="be0fc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be0fc-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="be0fc-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="be0fc-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="be0fc-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```
# <a name="c"></a>[<span data-ttu-id="be0fc-131">C#</span><span class="sxs-lookup"><span data-stu-id="be0fc-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be0fc-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be0fc-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be0fc-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be0fc-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be0fc-134">Java</span><span class="sxs-lookup"><span data-stu-id="be0fc-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="be0fc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="be0fc-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
