---
title: Получение personName
description: Получение свойств и связей объекта personName.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 93a5e52285ae4e1eb346a7dd8a6a76f35a77892d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811716"
---
# <a name="get-personname"></a><span data-ttu-id="3adaf-103">Получение personName</span><span class="sxs-lookup"><span data-stu-id="3adaf-103">Get personName</span></span>

<span data-ttu-id="3adaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3adaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3adaf-105">Получение свойств и связей объекта [PersonName](../resources/personname.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="3adaf-105">Retrieve the properties and relationships of a [personName](../resources/personname.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3adaf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3adaf-106">Permissions</span></span>

<span data-ttu-id="3adaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3adaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3adaf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3adaf-109">Permission type</span></span>                        | <span data-ttu-id="3adaf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3adaf-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="3adaf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3adaf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3adaf-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3adaf-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="3adaf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3adaf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3adaf-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3adaf-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="3adaf-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3adaf-115">Application</span></span>                            | <span data-ttu-id="3adaf-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3adaf-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="3adaf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3adaf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names/{id}
GET /users/{id | userPrincipalName}/profile/names/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3adaf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3adaf-118">Optional query parameters</span></span>

<span data-ttu-id="3adaf-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="3adaf-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="3adaf-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="3adaf-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="3adaf-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="3adaf-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3adaf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3adaf-122">Request headers</span></span>

| <span data-ttu-id="3adaf-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3adaf-123">Name</span></span>           |<span data-ttu-id="3adaf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3adaf-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="3adaf-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3adaf-125">Authorization</span></span>  | <span data-ttu-id="3adaf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3adaf-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="3adaf-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3adaf-128">Content-Type</span></span>   | <span data-ttu-id="3adaf-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3adaf-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3adaf-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3adaf-131">Request body</span></span>

<span data-ttu-id="3adaf-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3adaf-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3adaf-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="3adaf-133">Response</span></span>

<span data-ttu-id="3adaf-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3adaf-134">If successful, this method returns a `200 OK` response code and the requested [personName](../resources/personname.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3adaf-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="3adaf-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3adaf-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="3adaf-136">Request</span></span>

<span data-ttu-id="3adaf-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3adaf-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3adaf-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3adaf-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personname"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names/{id}
```
# <a name="c"></a>[<span data-ttu-id="3adaf-139">C#</span><span class="sxs-lookup"><span data-stu-id="3adaf-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personname-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3adaf-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3adaf-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personname-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3adaf-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3adaf-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personname-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="3adaf-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="3adaf-142">Response</span></span>

<span data-ttu-id="3adaf-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3adaf-143">The following is an example of the response.</span></span>

> <span data-ttu-id="3adaf-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3adaf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName"
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
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": "Kesha",
  "suffix": null,
  "title": null,
  "pronunciation": {
    "displayName": "In-no ken-te ",
    "first": "In-no ken-te Pop-ov",
    "maiden": null,
    "middle": null,
    "last": "Pop-ov"
  }
}
```
