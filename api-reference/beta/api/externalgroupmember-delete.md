---
title: Удаление externalGroupMember
description: Удаление объекта externalGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 24bfa2da5277192f4f14e828a7e6ea2d5b5d9ce1
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873173"
---
# <a name="delete-externalgroupmember"></a><span data-ttu-id="552dc-103">Удаление externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="552dc-103">Delete externalGroupMember</span></span>

<span data-ttu-id="552dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="552dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="552dc-105">Удаление объекта [externalGroupMember.](../resources/externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="552dc-105">Delete an [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="552dc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="552dc-106">Permissions</span></span>

<span data-ttu-id="552dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="552dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="552dc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="552dc-109">Permission type</span></span>                        | <span data-ttu-id="552dc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="552dc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="552dc-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="552dc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="552dc-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="552dc-112">Not supported</span></span>                               |
| <span data-ttu-id="552dc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="552dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="552dc-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="552dc-114">Not supported</span></span>                               |
| <span data-ttu-id="552dc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="552dc-115">Application</span></span>                            | <span data-ttu-id="552dc-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="552dc-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="552dc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="552dc-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}/members/{externalGroupMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="552dc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="552dc-118">Request headers</span></span>

| <span data-ttu-id="552dc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="552dc-119">Name</span></span>          | <span data-ttu-id="552dc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="552dc-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="552dc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="552dc-121">Authorization</span></span> | <span data-ttu-id="552dc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="552dc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="552dc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="552dc-124">Request body</span></span>

<span data-ttu-id="552dc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="552dc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="552dc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="552dc-126">Response</span></span>

<span data-ttu-id="552dc-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="552dc-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="552dc-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="552dc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="552dc-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="552dc-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="552dc-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="552dc-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroupmember"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```
# <a name="c"></a>[<span data-ttu-id="552dc-131">C#</span><span class="sxs-lookup"><span data-stu-id="552dc-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroupmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="552dc-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="552dc-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroupmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="552dc-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="552dc-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroupmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="552dc-134">Java</span><span class="sxs-lookup"><span data-stu-id="552dc-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroupmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="552dc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="552dc-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
