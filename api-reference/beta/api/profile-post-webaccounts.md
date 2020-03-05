---
title: Создание учетной записи
description: Создайте новый объект учетной записи.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 36c519f1d6fa3f7236eafe9a005e3e80451a9a0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455048"
---
# <a name="create-webaccount"></a><span data-ttu-id="cdab7-103">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="cdab7-103">Create webAccount</span></span>

<span data-ttu-id="cdab7-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cdab7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdab7-105">Создайте новый объект [учетной записи](../resources/webaccount.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="cdab7-105">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cdab7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdab7-106">Permissions</span></span>

<span data-ttu-id="cdab7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdab7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cdab7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdab7-109">Permission type</span></span>                        | <span data-ttu-id="cdab7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cdab7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cdab7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdab7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cdab7-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cdab7-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cdab7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdab7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdab7-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cdab7-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="cdab7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdab7-115">Application</span></span>                            | <span data-ttu-id="cdab7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdab7-116">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdab7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdab7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="cdab7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdab7-118">Request headers</span></span>

| <span data-ttu-id="cdab7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cdab7-119">Name</span></span>      |<span data-ttu-id="cdab7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cdab7-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cdab7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cdab7-121">Authorization</span></span>  | <span data-ttu-id="cdab7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdab7-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cdab7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cdab7-124">Content-Type</span></span>   | <span data-ttu-id="cdab7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdab7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdab7-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdab7-127">Request body</span></span>

<span data-ttu-id="cdab7-128">В тексте запроса добавьте представление объекта [учетной записи](../resources/webaccount.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdab7-128">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cdab7-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdab7-129">Response</span></span>

<span data-ttu-id="cdab7-130">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [учетной записи](../resources/webaccount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cdab7-130">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdab7-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="cdab7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cdab7-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdab7-132">Request</span></span>

<span data-ttu-id="cdab7-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdab7-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdab7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdab7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_webaccount_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/webAccounts
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="cdab7-135">C#</span><span class="sxs-lookup"><span data-stu-id="cdab7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-webaccount-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdab7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdab7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-webaccount-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdab7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdab7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-webaccount-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cdab7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cdab7-138">Response</span></span>

<span data-ttu-id="cdab7-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cdab7-139">The following is an example of the response.</span></span>

> <span data-ttu-id="cdab7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdab7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create webAccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
