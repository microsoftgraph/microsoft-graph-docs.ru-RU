---
title: Получение учетной записи службы
description: Получение свойств и связей объекта учетной записи.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 124778b379e1362d223467446bf74b569197422a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973971"
---
# <a name="get-webaccount"></a><span data-ttu-id="ec99e-103">Получение учетной записи службы</span><span class="sxs-lookup"><span data-stu-id="ec99e-103">Get webAccount</span></span>

<span data-ttu-id="ec99e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec99e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec99e-105">Получение свойств и связей объекта [учетной записи](../resources/webaccount.md) сайта из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ec99e-105">Retrieve the properties and relationships of a [webAccount](../resources/webaccount.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec99e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec99e-106">Permissions</span></span>

<span data-ttu-id="ec99e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec99e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec99e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec99e-109">Permission type</span></span>                        | <span data-ttu-id="ec99e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ec99e-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="ec99e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec99e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec99e-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ec99e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ec99e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec99e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec99e-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ec99e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ec99e-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ec99e-115">Application</span></span>                            | <span data-ttu-id="ec99e-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ec99e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="ec99e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec99e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/webAccounts/{id}
GET /users/{id | userPrincipalName}/profile/webAccounts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec99e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec99e-118">Optional query parameters</span></span>

<span data-ttu-id="ec99e-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="ec99e-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="ec99e-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="ec99e-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="ec99e-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="ec99e-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec99e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec99e-122">Request headers</span></span>

| <span data-ttu-id="ec99e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ec99e-123">Name</span></span>           |<span data-ttu-id="ec99e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ec99e-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ec99e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec99e-125">Authorization</span></span>  | <span data-ttu-id="ec99e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec99e-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="ec99e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec99e-128">Request body</span></span>

<span data-ttu-id="ec99e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec99e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec99e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec99e-130">Response</span></span>

<span data-ttu-id="ec99e-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [учетной записи](../resources/webaccount.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ec99e-131">If successful, this method returns a `200 OK` response code and the requested [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec99e-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="ec99e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec99e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec99e-133">Request</span></span>

<span data-ttu-id="ec99e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec99e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec99e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec99e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_webaccount"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
```
# <a name="c"></a>[<span data-ttu-id="ec99e-136">C#</span><span class="sxs-lookup"><span data-stu-id="ec99e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec99e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec99e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec99e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec99e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec99e-139">Java</span><span class="sxs-lookup"><span data-stu-id="ec99e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-webaccount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec99e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec99e-140">Response</span></span>

<span data-ttu-id="ec99e-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ec99e-141">The following is an example of the response.</span></span>

> <span data-ttu-id="ec99e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ec99e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
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
  "source": null,
  "description": "My Github contributions!",
  "userId": "innocenty.popov",
  "service": {
    "name": "GitHub",
    "webUrl": "https://github.com"
  },
  "statusMessage": null,
  "webUrl": "https://github.com/innocenty.popov"
}
```


