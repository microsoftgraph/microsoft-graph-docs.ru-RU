---
title: Удаление b2cUserFlow
description: Удаление объекта b2cUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26e4b244128a8dbd61179197d82d9d83a920b91f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991514"
---
# <a name="delete-b2cuserflow"></a><span data-ttu-id="d1c94-103">Удаление b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="d1c94-103">Delete b2cUserFlow</span></span>

<span data-ttu-id="d1c94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1c94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1c94-105">Удаление объекта [b2cUserFlow](../resources/b2cuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="d1c94-105">Delete a [b2cUserFlow](../resources/b2cuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1c94-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1c94-106">Permissions</span></span>

<span data-ttu-id="d1c94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1c94-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1c94-109">Permission type</span></span>      | <span data-ttu-id="d1c94-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1c94-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1c94-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1c94-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1c94-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d1c94-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d1c94-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1c94-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d1c94-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1c94-114">Not supported.</span></span>|
|<span data-ttu-id="d1c94-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1c94-115">Application</span></span>|<span data-ttu-id="d1c94-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d1c94-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d1c94-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="d1c94-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d1c94-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d1c94-118">Global administrator</span></span>
* <span data-ttu-id="d1c94-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="d1c94-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d1c94-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1c94-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d1c94-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1c94-121">Request headers</span></span>

|<span data-ttu-id="d1c94-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d1c94-122">Name</span></span>|<span data-ttu-id="d1c94-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d1c94-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="d1c94-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1c94-124">Authorization</span></span>|<span data-ttu-id="d1c94-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1c94-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1c94-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1c94-127">Request body</span></span>

<span data-ttu-id="d1c94-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1c94-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1c94-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1c94-129">Response</span></span>

<span data-ttu-id="d1c94-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d1c94-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d1c94-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d1c94-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1c94-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1c94-132">Request</span></span>

<span data-ttu-id="d1c94-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1c94-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d1c94-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1c94-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2cUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="d1c94-135">C#</span><span class="sxs-lookup"><span data-stu-id="d1c94-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1c94-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1c94-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1c94-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1c94-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d1c94-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1c94-138">Response</span></span>

<span data-ttu-id="d1c94-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d1c94-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


