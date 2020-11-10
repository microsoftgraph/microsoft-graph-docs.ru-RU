---
title: Получение Персонцертификатион
description: Чтение свойств и связей объекта Персонцертификатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: cb6e947695aecfb6e1aa6f4242ce95266e941d12
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972816"
---
# <a name="get-personcertification"></a><span data-ttu-id="28413-103">Получение Персонцертификатион</span><span class="sxs-lookup"><span data-stu-id="28413-103">Get personCertification</span></span>
<span data-ttu-id="28413-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28413-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28413-105">Чтение свойств и связей объекта [персонцертификатион](../resources/personcertification.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="28413-105">Read the properties and relationships of a [personCertification](../resources/personcertification.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="28413-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28413-106">Permissions</span></span>

<span data-ttu-id="28413-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28413-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28413-109">Permission type</span></span>                        | <span data-ttu-id="28413-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28413-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="28413-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28413-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="28413-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="28413-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="28413-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28413-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28413-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="28413-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="28413-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="28413-115">Application</span></span>                            | <span data-ttu-id="28413-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="28413-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="28413-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28413-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/certifications/{id}
GET /users/{id | userPrincipalName}/profile/certifications/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28413-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="28413-118">Optional query parameters</span></span>

<span data-ttu-id="28413-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="28413-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="28413-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="28413-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="28413-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="28413-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28413-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28413-122">Request headers</span></span>
|<span data-ttu-id="28413-123">Имя</span><span class="sxs-lookup"><span data-stu-id="28413-123">Name</span></span>|<span data-ttu-id="28413-124">Описание</span><span class="sxs-lookup"><span data-stu-id="28413-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="28413-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28413-125">Authorization</span></span>|<span data-ttu-id="28413-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28413-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="28413-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28413-128">Request body</span></span>
<span data-ttu-id="28413-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28413-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28413-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="28413-130">Response</span></span>

<span data-ttu-id="28413-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [персонцертификатион](../resources/personcertification.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28413-131">If successful, this method returns a `200 OK` response code and an [personCertification](../resources/personcertification.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28413-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="28413-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28413-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="28413-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="28413-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="28413-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_personCertification"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/certifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="28413-135">C#</span><span class="sxs-lookup"><span data-stu-id="28413-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-personcertification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28413-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28413-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-personcertification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28413-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28413-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-personcertification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28413-138">Java</span><span class="sxs-lookup"><span data-stu-id="28413-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-personcertification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="28413-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="28413-139">Response</span></span>

<span data-ttu-id="28413-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="28413-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personCertification"
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
  "certificationId": "KB-1235466333663322",
  "description": "Blackbelt in Marketing - Brand Management",
  "displayName": "Marketing Blackbelt - Brand Management",
  "endDate": "Date",
  "issuedDate": "Date",
  "issuingAuthority": "International Academy of Marketing Excellence",
  "issuingCompany": "International Academy of Marketing Excellence",
  "startDate": "Date",
  "thumbnailUrl": "https://iame.io/dfhdfdfd334.jpg",
  "webUrl": "https://www.iame.io/blackbelt"
}
```


