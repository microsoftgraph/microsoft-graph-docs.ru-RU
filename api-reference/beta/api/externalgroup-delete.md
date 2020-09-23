---
title: Удаление Екстерналграуп
description: Удаляет объект Екстерналграуп.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 43fb3f0cb0740fe3c7fef23bb244681967cbb13d
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223077"
---
# <a name="delete-externalgroup"></a><span data-ttu-id="1918e-103">Удаление Екстерналграуп</span><span class="sxs-lookup"><span data-stu-id="1918e-103">Delete externalGroup</span></span>

<span data-ttu-id="1918e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1918e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1918e-105">Удаление объекта [екстерналграуп](../resources/externalgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="1918e-105">Delete an [externalGroup](../resources/externalgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1918e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1918e-106">Permissions</span></span>

<span data-ttu-id="1918e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1918e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1918e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1918e-109">Permission type</span></span>                        | <span data-ttu-id="1918e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1918e-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1918e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1918e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1918e-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1918e-112">Not supported</span></span>                               |
| <span data-ttu-id="1918e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1918e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1918e-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="1918e-114">Not supported</span></span>                               |
| <span data-ttu-id="1918e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1918e-115">Application</span></span>                            | <span data-ttu-id="1918e-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1918e-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="1918e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1918e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="1918e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1918e-118">Request headers</span></span>

| <span data-ttu-id="1918e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1918e-119">Name</span></span>          | <span data-ttu-id="1918e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1918e-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1918e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1918e-121">Authorization</span></span> | <span data-ttu-id="1918e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1918e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1918e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1918e-124">Request body</span></span>

<span data-ttu-id="1918e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1918e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1918e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1918e-126">Response</span></span>

<span data-ttu-id="1918e-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1918e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1918e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="1918e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1918e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1918e-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1918e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="1918e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroup"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000
```
# <a name="c"></a>[<span data-ttu-id="1918e-131">C#</span><span class="sxs-lookup"><span data-stu-id="1918e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1918e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1918e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1918e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1918e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="1918e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1918e-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
