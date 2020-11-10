---
title: Удаление Екстерналграупмембер
description: Удаление объекта Екстерналграупмембер.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b6a6c79288d2eee9ff4ef2cbb0a9d200a6735050
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954624"
---
# <a name="delete-externalgroupmember"></a><span data-ttu-id="de773-103">Удаление Екстерналграупмембер</span><span class="sxs-lookup"><span data-stu-id="de773-103">Delete externalGroupMember</span></span>

<span data-ttu-id="de773-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de773-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de773-105">Удаление объекта [екстерналграупмембер](../resources/externalgroupmember.md) .</span><span class="sxs-lookup"><span data-stu-id="de773-105">Delete an [externalGroupMember](../resources/externalgroupmember.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="de773-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de773-106">Permissions</span></span>

<span data-ttu-id="de773-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de773-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de773-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de773-109">Permission type</span></span>                        | <span data-ttu-id="de773-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="de773-110">Permissions (from most to least privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de773-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de773-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="de773-112">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de773-112">Not supported</span></span>                               |
| <span data-ttu-id="de773-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de773-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de773-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="de773-114">Not supported</span></span>                               |
| <span data-ttu-id="de773-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de773-115">Application</span></span>                            | <span data-ttu-id="de773-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de773-116">ExternalItem.ReadWrite.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="de773-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de773-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /external/connections/{connectionId}/groups/{externalGroupId}/members/{externalGroupMemberId}
```

## <a name="request-headers"></a><span data-ttu-id="de773-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de773-118">Request headers</span></span>

| <span data-ttu-id="de773-119">Имя</span><span class="sxs-lookup"><span data-stu-id="de773-119">Name</span></span>          | <span data-ttu-id="de773-120">Описание</span><span class="sxs-lookup"><span data-stu-id="de773-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="de773-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de773-121">Authorization</span></span> | <span data-ttu-id="de773-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de773-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de773-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de773-124">Request body</span></span>

<span data-ttu-id="de773-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de773-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de773-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="de773-126">Response</span></span>

<span data-ttu-id="de773-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="de773-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="de773-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="de773-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de773-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="de773-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="de773-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="de773-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalgroupmember"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members/14m1b9c38qe647f6a
```
# <a name="c"></a>[<span data-ttu-id="de773-131">C#</span><span class="sxs-lookup"><span data-stu-id="de773-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalgroupmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de773-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de773-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalgroupmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de773-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de773-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalgroupmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de773-134">Java</span><span class="sxs-lookup"><span data-stu-id="de773-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalgroupmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="de773-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="de773-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
