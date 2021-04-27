---
title: Get personInterest
description: Извлечение свойств и связей объекта personInterest.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5860d04fcbffae85054334b51be1d50a1ffc82c1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037860"
---
# <a name="get-personinterest"></a><span data-ttu-id="098f6-103">Get personInterest</span><span class="sxs-lookup"><span data-stu-id="098f6-103">Get personInterest</span></span>

<span data-ttu-id="098f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="098f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="098f6-105">Извлечение свойств и связей [объекта personInterest](../resources/personinterest.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="098f6-105">Retrieve the properties and relationships of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="098f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="098f6-106">Permissions</span></span>

<span data-ttu-id="098f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="098f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="098f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="098f6-109">Permission type</span></span>                        | <span data-ttu-id="098f6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="098f6-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="098f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="098f6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="098f6-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="098f6-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="098f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="098f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="098f6-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="098f6-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="098f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="098f6-115">Application</span></span>                            | <span data-ttu-id="098f6-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="098f6-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="098f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="098f6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/interests/{id}
GET /users/{id | userPrincipalName}/profile/interests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="098f6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="098f6-118">Optional query parameters</span></span>

<span data-ttu-id="098f6-119">Этот метод поддерживает параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="098f6-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="098f6-120">Укажите список свойств, которые необходимо включить в ответ, разделив их запятой.</span><span class="sxs-lookup"><span data-stu-id="098f6-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="098f6-121">Для оптимальной производительности выберите только подмножество необходимых свойств.</span><span class="sxs-lookup"><span data-stu-id="098f6-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="098f6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="098f6-122">Request headers</span></span>

| <span data-ttu-id="098f6-123">Имя</span><span class="sxs-lookup"><span data-stu-id="098f6-123">Name</span></span>           |<span data-ttu-id="098f6-124">Описание</span><span class="sxs-lookup"><span data-stu-id="098f6-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="098f6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="098f6-125">Authorization</span></span>  | <span data-ttu-id="098f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="098f6-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="098f6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="098f6-128">Request body</span></span>

<span data-ttu-id="098f6-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="098f6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="098f6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="098f6-130">Response</span></span>

<span data-ttu-id="098f6-131">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [personInterest](../resources/personinterest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="098f6-131">If successful, this method returns a `200 OK` response code and the requested [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="098f6-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="098f6-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="098f6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="098f6-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="098f6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="098f6-134">HTTP</span></span>](#tab/http)

<span data-ttu-id="098f6-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="098f6-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_personinterest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/interests/{id}
```
# <a name="c"></a>[<span data-ttu-id="098f6-136">C#</span><span class="sxs-lookup"><span data-stu-id="098f6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="098f6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="098f6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="098f6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="098f6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="098f6-139">Java</span><span class="sxs-lookup"><span data-stu-id="098f6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-personinterest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="098f6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="098f6-140">Response</span></span>

<span data-ttu-id="098f6-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="098f6-141">The following is an example of the response.</span></span>

> <span data-ttu-id="098f6-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="098f6-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


