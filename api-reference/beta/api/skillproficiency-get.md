---
title: Получение СкиллпрофиЦиенци
description: Получение свойств и связей объекта скиллпрофиЦиенци.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b7a4039240a91db30ceb0a3c6f2f13817ed26f67
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973153"
---
# <a name="get-skillproficiency"></a><span data-ttu-id="271ec-103">Получение СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="271ec-103">Get skillProficiency</span></span>

<span data-ttu-id="271ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="271ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="271ec-105">Получение свойств и связей объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="271ec-105">Retrieve the properties and relationships of a [skillproficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="271ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="271ec-106">Permissions</span></span>

<span data-ttu-id="271ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="271ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="271ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="271ec-109">Permission type</span></span>                        | <span data-ttu-id="271ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="271ec-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="271ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="271ec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="271ec-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="271ec-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="271ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="271ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="271ec-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="271ec-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="271ec-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="271ec-115">Application</span></span>                            | <span data-ttu-id="271ec-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="271ec-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="271ec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="271ec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/skills/{id}
GET /users/{id | userPrincipalName}/profile/skills/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="271ec-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="271ec-118">Optional query parameters</span></span>

<span data-ttu-id="271ec-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="271ec-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="271ec-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="271ec-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="271ec-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="271ec-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="271ec-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="271ec-122">Request headers</span></span>

| <span data-ttu-id="271ec-123">Имя</span><span class="sxs-lookup"><span data-stu-id="271ec-123">Name</span></span>           | <span data-ttu-id="271ec-124">Описание</span><span class="sxs-lookup"><span data-stu-id="271ec-124">Description</span></span>                  |
|:---------------|:-----------------------------|
| <span data-ttu-id="271ec-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="271ec-125">Authorization</span></span>  | <span data-ttu-id="271ec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="271ec-p103">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="271ec-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="271ec-128">Content-Type</span></span>   | <span data-ttu-id="271ec-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="271ec-p104">application/json. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="271ec-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="271ec-131">Request body</span></span>

<span data-ttu-id="271ec-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="271ec-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="271ec-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="271ec-133">Response</span></span>

<span data-ttu-id="271ec-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [скиллпрофиЦиенци](../resources/skillproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="271ec-134">If successful, this method returns a `200 OK` response code and the requested [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="271ec-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="271ec-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="271ec-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="271ec-136">Request</span></span>

<span data-ttu-id="271ec-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="271ec-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="271ec-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="271ec-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_skillproficiency"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/skills/{id}
```
# <a name="c"></a>[<span data-ttu-id="271ec-139">C#</span><span class="sxs-lookup"><span data-stu-id="271ec-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="271ec-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="271ec-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="271ec-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="271ec-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="271ec-142">Java</span><span class="sxs-lookup"><span data-stu-id="271ec-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-skillproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="271ec-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="271ec-143">Response</span></span>

<span data-ttu-id="271ec-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="271ec-144">The following is an example of the response.</span></span>

> <span data-ttu-id="271ec-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="271ec-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
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
  "categories": [
    "Professional"
  ],
  "displayName": "API Design",
  "proficiency": "advancedProfessional",
  "webUrl": null,
  "collaborationTags": [
    "ableToMentor"
  ]
}
```


