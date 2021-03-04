---
title: Удаление b2cIdentityUserFlow
description: Удаление объекта b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 11ea70b285f20e281d342e808ad1a15b98041572
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438353"
---
# <a name="delete-b2cidentityuserflow"></a><span data-ttu-id="e6c47-103">Удаление b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="e6c47-103">Delete b2cIdentityUserFlow</span></span>

<span data-ttu-id="e6c47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6c47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6c47-105">Удаление [объекта b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="e6c47-105">Delete a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6c47-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6c47-106">Permissions</span></span>

<span data-ttu-id="e6c47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6c47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6c47-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6c47-109">Permission type</span></span>      | <span data-ttu-id="e6c47-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6c47-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6c47-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6c47-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e6c47-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c47-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e6c47-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6c47-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e6c47-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6c47-114">Not supported.</span></span>|
|<span data-ttu-id="e6c47-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e6c47-115">Application</span></span>|<span data-ttu-id="e6c47-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c47-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e6c47-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="e6c47-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e6c47-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e6c47-118">Global administrator</span></span>
* <span data-ttu-id="e6c47-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="e6c47-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e6c47-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6c47-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2cUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e6c47-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6c47-121">Request headers</span></span>

|<span data-ttu-id="e6c47-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e6c47-122">Name</span></span>|<span data-ttu-id="e6c47-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e6c47-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e6c47-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6c47-124">Authorization</span></span>|<span data-ttu-id="e6c47-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6c47-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6c47-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6c47-127">Request body</span></span>

<span data-ttu-id="e6c47-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6c47-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6c47-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6c47-129">Response</span></span>

<span data-ttu-id="e6c47-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6c47-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e6c47-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e6c47-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6c47-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6c47-132">Request</span></span>

<span data-ttu-id="e6c47-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6c47-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6c47-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6c47-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2cUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="e6c47-135">C#</span><span class="sxs-lookup"><span data-stu-id="e6c47-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6c47-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6c47-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6c47-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6c47-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6c47-138">Java</span><span class="sxs-lookup"><span data-stu-id="e6c47-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e6c47-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6c47-139">Response</span></span>

<span data-ttu-id="e6c47-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e6c47-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


