---
title: Список allowedUsers
description: Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный принтер.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6857b20f872a7e868175910c84a0d54c11b7b6f0
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947906"
---
# <a name="list-allowedusers"></a><span data-ttu-id="4a158-103">Список allowedUsers</span><span class="sxs-lookup"><span data-stu-id="4a158-103">List allowedUsers</span></span>

<span data-ttu-id="4a158-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a158-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a158-105">Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный [принтер](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="4a158-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a158-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a158-106">Permissions</span></span>
<span data-ttu-id="4a158-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a158-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4a158-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="4a158-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="4a158-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a158-110">Permission type</span></span> | <span data-ttu-id="4a158-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a158-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4a158-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a158-112">Delegated (work or school account)</span></span>| <span data-ttu-id="4a158-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4a158-113">Users.Read.All</span></span> |
|<span data-ttu-id="4a158-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a158-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a158-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a158-115">Not Supported.</span></span>|
|<span data-ttu-id="4a158-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4a158-116">Application</span></span>|<span data-ttu-id="4a158-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a158-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a158-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a158-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedUsers
```

## <a name="request-headers"></a><span data-ttu-id="4a158-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a158-119">Request headers</span></span>
| <span data-ttu-id="4a158-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4a158-120">Name</span></span>      |<span data-ttu-id="4a158-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4a158-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a158-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a158-122">Authorization</span></span> | <span data-ttu-id="4a158-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a158-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a158-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a158-125">Request body</span></span>
<span data-ttu-id="4a158-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a158-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4a158-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4a158-127">Response</span></span>
<span data-ttu-id="4a158-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [userIdentity](../resources/userIdentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a158-128">If successful, this method returns a `200 OK` response code and a collection of [userIdentity](../resources/userIdentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a158-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4a158-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a158-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a158-130">Request</span></span>
<span data-ttu-id="4a158-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a158-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a158-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a158-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="4a158-133">C#</span><span class="sxs-lookup"><span data-stu-id="4a158-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a158-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a158-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a158-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a158-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4a158-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a158-136">Response</span></span>
<span data-ttu-id="4a158-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a158-137">The following is an example of the response.</span></span>
><span data-ttu-id="4a158-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a158-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 286

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printIdentity)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
