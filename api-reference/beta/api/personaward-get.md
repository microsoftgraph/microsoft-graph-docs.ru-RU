---
title: Получение Персонавард
description: Чтение свойств и связей объекта Персонавард.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a7a0c13010854db62cc34dbcd897af47a9b9982f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968399"
---
# <a name="get-personaward"></a><span data-ttu-id="d4b9b-103">Получение Персонавард</span><span class="sxs-lookup"><span data-stu-id="d4b9b-103">Get personAward</span></span>

<span data-ttu-id="d4b9b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4b9b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4b9b-105">Считывание свойств и связей объекта [персонавард](../resources/personaward.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4b9b-105">Read the properties and relationships of a [personAward](../resources/personaward.md) object from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4b9b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4b9b-106">Permissions</span></span>

<span data-ttu-id="d4b9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4b9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4b9b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4b9b-109">Permission type</span></span>                        | <span data-ttu-id="d4b9b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4b9b-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="d4b9b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4b9b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4b9b-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d4b9b-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d4b9b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4b9b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4b9b-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d4b9b-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d4b9b-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="d4b9b-115">Application</span></span>                            | <span data-ttu-id="d4b9b-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d4b9b-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="d4b9b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4b9b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/awards/{id}
GET /users/{id | userPrincipalName}/profile/awards/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4b9b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d4b9b-118">Optional query parameters</span></span>

<span data-ttu-id="d4b9b-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="d4b9b-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="d4b9b-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="d4b9b-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="d4b9b-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="d4b9b-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4b9b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4b9b-122">Request headers</span></span>
|<span data-ttu-id="d4b9b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d4b9b-123">Name</span></span>|<span data-ttu-id="d4b9b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d4b9b-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d4b9b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4b9b-125">Authorization</span></span>|<span data-ttu-id="d4b9b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4b9b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4b9b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4b9b-128">Request body</span></span>
<span data-ttu-id="d4b9b-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d4b9b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4b9b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4b9b-130">Response</span></span>

<span data-ttu-id="d4b9b-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [персонавард](../resources/personaward.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d4b9b-131">If successful, this method returns a `200 OK` response code and an [personAward](../resources/personaward.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4b9b-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4b9b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4b9b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4b9b-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="d4b9b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4b9b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personAward"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/awards/{id}
```
# <a name="c"></a>[<span data-ttu-id="d4b9b-135">C#</span><span class="sxs-lookup"><span data-stu-id="d4b9b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personaward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4b9b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4b9b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personaward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4b9b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4b9b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personaward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d4b9b-138">Java</span><span class="sxs-lookup"><span data-stu-id="d4b9b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-personaward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d4b9b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4b9b-139">Response</span></span>

<span data-ttu-id="d4b9b-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d4b9b-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAward"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
  "description": "Lifetime Achievement award from the International Association of Branding Managers",
  "displayName": "Lifetime Achievement Award For Excellence in Branding",
  "issuedDate": "Date",
  "issuingAuthority": "International Association of Branding Management",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```


