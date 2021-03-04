---
title: Удаление identityApiConnector
description: Удаляет объект identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 74d8b44e73b6343efd55240e51bb22896e78ce6e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435632"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="94b18-103">Удаление identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="94b18-103">Delete identityApiConnector</span></span>

<span data-ttu-id="94b18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94b18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94b18-105">Удаляет объект [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="94b18-105">Deletes an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94b18-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94b18-106">Permissions</span></span>

<span data-ttu-id="94b18-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94b18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94b18-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94b18-109">Permission type</span></span>                        | <span data-ttu-id="94b18-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94b18-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="94b18-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94b18-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94b18-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94b18-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="94b18-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94b18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94b18-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94b18-114">Not supported.</span></span>  |
| <span data-ttu-id="94b18-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="94b18-115">Application</span></span>                            | <span data-ttu-id="94b18-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94b18-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="94b18-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="94b18-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="94b18-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="94b18-118">Global administrator</span></span>
* <span data-ttu-id="94b18-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="94b18-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="94b18-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94b18-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="94b18-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94b18-121">Request headers</span></span>
|<span data-ttu-id="94b18-122">Имя</span><span class="sxs-lookup"><span data-stu-id="94b18-122">Name</span></span>|<span data-ttu-id="94b18-123">Описание</span><span class="sxs-lookup"><span data-stu-id="94b18-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="94b18-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94b18-124">Authorization</span></span>|<span data-ttu-id="94b18-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94b18-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="94b18-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="94b18-127">Request body</span></span>
<span data-ttu-id="94b18-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94b18-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94b18-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="94b18-129">Response</span></span>

<span data-ttu-id="94b18-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="94b18-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="94b18-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="94b18-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94b18-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="94b18-132">Request</span></span>

<span data-ttu-id="94b18-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94b18-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94b18-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="94b18-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="94b18-135">C#</span><span class="sxs-lookup"><span data-stu-id="94b18-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94b18-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94b18-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94b18-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94b18-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94b18-138">Java</span><span class="sxs-lookup"><span data-stu-id="94b18-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94b18-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="94b18-139">Response</span></span>

<span data-ttu-id="94b18-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="94b18-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
