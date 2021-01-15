---
title: Удаление identityApiConnector
description: Удаляет объект identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3f021afd1285d00e71ef9ddab25210f00c8ac2be
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873684"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="d2dbd-103">Удаление identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="d2dbd-103">Delete identityApiConnector</span></span>

<span data-ttu-id="d2dbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2dbd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2dbd-105">Удаляет объект [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="d2dbd-105">Deletes an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2dbd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2dbd-106">Permissions</span></span>

<span data-ttu-id="d2dbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2dbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2dbd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2dbd-109">Permission type</span></span>                        | <span data-ttu-id="d2dbd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2dbd-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d2dbd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2dbd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2dbd-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2dbd-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="d2dbd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2dbd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2dbd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2dbd-114">Not supported.</span></span>  |
| <span data-ttu-id="d2dbd-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d2dbd-115">Application</span></span>                            | <span data-ttu-id="d2dbd-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2dbd-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="d2dbd-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="d2dbd-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d2dbd-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d2dbd-118">Global administrator</span></span>
* <span data-ttu-id="d2dbd-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="d2dbd-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d2dbd-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2dbd-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="d2dbd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2dbd-121">Request headers</span></span>
|<span data-ttu-id="d2dbd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d2dbd-122">Name</span></span>|<span data-ttu-id="d2dbd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d2dbd-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d2dbd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2dbd-124">Authorization</span></span>|<span data-ttu-id="d2dbd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2dbd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2dbd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2dbd-127">Request body</span></span>
<span data-ttu-id="d2dbd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2dbd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2dbd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2dbd-129">Response</span></span>

<span data-ttu-id="d2dbd-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d2dbd-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d2dbd-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d2dbd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2dbd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2dbd-132">Request</span></span>

<span data-ttu-id="d2dbd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2dbd-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d2dbd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2dbd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="d2dbd-135">C#</span><span class="sxs-lookup"><span data-stu-id="d2dbd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2dbd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2dbd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2dbd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2dbd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2dbd-138">Java</span><span class="sxs-lookup"><span data-stu-id="d2dbd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2dbd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2dbd-139">Response</span></span>

<span data-ttu-id="d2dbd-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2dbd-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
