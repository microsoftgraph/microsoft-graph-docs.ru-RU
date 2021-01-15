---
title: Удаление userSource
description: Удаляет объект userSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 631d547aefec38258d69ccb48d325fc955e65a57
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873033"
---
# <a name="delete-usersource"></a><span data-ttu-id="7015f-103">Удаление userSource</span><span class="sxs-lookup"><span data-stu-id="7015f-103">Delete userSource</span></span>

<span data-ttu-id="7015f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7015f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7015f-105">Удаление объекта [userSource.](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="7015f-105">Delete a [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7015f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7015f-106">Permissions</span></span>

<span data-ttu-id="7015f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7015f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7015f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7015f-109">Permission type</span></span>|<span data-ttu-id="7015f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7015f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7015f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7015f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7015f-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="7015f-112">User.Read</span></span>|
|<span data-ttu-id="7015f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7015f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7015f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7015f-114">Not supported.</span></span>|
|<span data-ttu-id="7015f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7015f-115">Application</span></span>|<span data-ttu-id="7015f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7015f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7015f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7015f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources/{userSourceId}
```

## <a name="request-headers"></a><span data-ttu-id="7015f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7015f-118">Request headers</span></span>

|<span data-ttu-id="7015f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7015f-119">Name</span></span>|<span data-ttu-id="7015f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7015f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7015f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7015f-121">Authorization</span></span>|<span data-ttu-id="7015f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7015f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7015f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7015f-124">Request body</span></span>

<span data-ttu-id="7015f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7015f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7015f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7015f-126">Response</span></span>

<span data-ttu-id="7015f-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7015f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7015f-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="7015f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7015f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7015f-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7015f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7015f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_usersource"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735
```
# <a name="c"></a>[<span data-ttu-id="7015f-131">C#</span><span class="sxs-lookup"><span data-stu-id="7015f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7015f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7015f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7015f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7015f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7015f-134">Java</span><span class="sxs-lookup"><span data-stu-id="7015f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7015f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7015f-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
