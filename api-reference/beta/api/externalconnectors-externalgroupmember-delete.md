---
title: Удаление externalGroupMember
description: Удаление внешнего объектаGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 2e72739cb637593e2a846536e3b92a40dde693f4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467672"
---
# <a name="delete-externalgroupmember"></a><span data-ttu-id="d4c5b-103">Удаление externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="d4c5b-103">Delete externalGroupMember</span></span>

<span data-ttu-id="d4c5b-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="d4c5b-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4c5b-105">Удаление [внешнего объектаGroupMember.](../resources/externalconnectors-externalgroupmember.md)</span><span class="sxs-lookup"><span data-stu-id="d4c5b-105">Delete an [externalGroupMember](../resources/externalconnectors-externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4c5b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4c5b-106">Permissions</span></span>

<span data-ttu-id="d4c5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4c5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4c5b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4c5b-109">Permission type</span></span>                        | <span data-ttu-id="d4c5b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4c5b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4c5b-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4c5b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4c5b-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d4c5b-112">Not supported</span></span>                               |
| <span data-ttu-id="d4c5b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4c5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4c5b-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d4c5b-114">Not supported</span></span>                               |
| <span data-ttu-id="d4c5b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d4c5b-115">Application</span></span>                            | <span data-ttu-id="d4c5b-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4c5b-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span>                 |

## <a name="http-request"></a><span data-ttu-id="d4c5b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4c5b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}/members/{externalGroupMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="d4c5b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4c5b-118">Request headers</span></span>

| <span data-ttu-id="d4c5b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d4c5b-119">Name</span></span>          | <span data-ttu-id="d4c5b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d4c5b-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d4c5b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4c5b-121">Authorization</span></span> | <span data-ttu-id="d4c5b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4c5b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4c5b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4c5b-124">Request body</span></span>

<span data-ttu-id="d4c5b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4c5b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4c5b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4c5b-126">Response</span></span>

<span data-ttu-id="d4c5b-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d4c5b-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d4c5b-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4c5b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4c5b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4c5b-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d4c5b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4c5b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroupmember"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```
# <a name="c"></a>[<span data-ttu-id="d4c5b-131">C#</span><span class="sxs-lookup"><span data-stu-id="d4c5b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroupmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4c5b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4c5b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroupmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4c5b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4c5b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroupmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4c5b-134">Java</span><span class="sxs-lookup"><span data-stu-id="d4c5b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroupmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d4c5b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4c5b-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
