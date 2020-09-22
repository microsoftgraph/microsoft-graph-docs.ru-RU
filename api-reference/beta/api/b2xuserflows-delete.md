---
title: Удаление b2xUserFlow
description: Удаление объекта b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 586af0af699aa528dfe6b0a7d15988e9edca3e0d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991434"
---
# <a name="delete-b2xuserflow"></a><span data-ttu-id="ad325-103">Удаление b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="ad325-103">Delete b2xUserFlow</span></span>

<span data-ttu-id="ad325-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad325-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad325-105">Удаление объекта [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="ad325-105">Delete a [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad325-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad325-106">Permissions</span></span>

<span data-ttu-id="ad325-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad325-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad325-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad325-109">Permission type</span></span>      | <span data-ttu-id="ad325-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad325-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad325-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad325-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad325-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ad325-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ad325-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad325-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ad325-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad325-114">Not supported.</span></span>|
|<span data-ttu-id="ad325-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad325-115">Application</span></span>|<span data-ttu-id="ad325-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ad325-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ad325-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="ad325-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ad325-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ad325-118">Global administrator</span></span>
* <span data-ttu-id="ad325-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="ad325-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ad325-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad325-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/b2xUserFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ad325-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad325-121">Request headers</span></span>

|<span data-ttu-id="ad325-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ad325-122">Name</span></span>|<span data-ttu-id="ad325-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ad325-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ad325-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad325-124">Authorization</span></span>|<span data-ttu-id="ad325-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad325-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad325-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad325-127">Request body</span></span>

<span data-ttu-id="ad325-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad325-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad325-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad325-129">Response</span></span>

<span data-ttu-id="ad325-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ad325-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ad325-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ad325-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad325-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad325-132">Request</span></span>

<span data-ttu-id="ad325-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad325-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ad325-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad325-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_b2xUserFlows"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="ad325-135">C#</span><span class="sxs-lookup"><span data-stu-id="ad325-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad325-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad325-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad325-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad325-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad325-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad325-138">Response</span></span>

<span data-ttu-id="ad325-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad325-139">The following is an example of the response.</span></span>

<span data-ttu-id="ad325-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad325-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```


