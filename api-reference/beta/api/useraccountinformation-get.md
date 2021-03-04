---
title: Get userAccountInformation
description: Извлечение свойств и связей объекта userAccountInformation.
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: ec6b24daf3b2314e8175a7456f3187f2ac67178c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443320"
---
# <a name="get-useraccountinformation"></a><span data-ttu-id="2848a-103">Get userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="2848a-103">Get userAccountInformation</span></span>

<span data-ttu-id="2848a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2848a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2848a-105">Извлечение свойств и связей [объекта userAccountInformation](../resources/useraccountinformation.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="2848a-105">Retrieve the properties and relationships of an [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2848a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2848a-106">Permissions</span></span>

<span data-ttu-id="2848a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2848a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2848a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2848a-109">Permission type</span></span>                        | <span data-ttu-id="2848a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2848a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="2848a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2848a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2848a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2848a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2848a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2848a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2848a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2848a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2848a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2848a-115">Application</span></span>                            | <span data-ttu-id="2848a-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2848a-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="2848a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2848a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/account/{id}
GET /users/{id | userPrincipalName}/profile/account/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2848a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2848a-118">Optional query parameters</span></span>

<span data-ttu-id="2848a-119">Этот метод поддерживает параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="2848a-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="2848a-120">Укажите список свойств, которые необходимо включить в ответ, разделив их запятой.</span><span class="sxs-lookup"><span data-stu-id="2848a-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="2848a-121">Для оптимальной производительности выберите только подмножество необходимых свойств.</span><span class="sxs-lookup"><span data-stu-id="2848a-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2848a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2848a-122">Request headers</span></span>

| <span data-ttu-id="2848a-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2848a-123">Name</span></span>          |<span data-ttu-id="2848a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2848a-124">Description</span></span>                |
|:--------------|:--------------------------|
| <span data-ttu-id="2848a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2848a-125">Authorization</span></span> | <span data-ttu-id="2848a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2848a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2848a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2848a-128">Request body</span></span>

<span data-ttu-id="2848a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2848a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2848a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="2848a-130">Response</span></span>

<span data-ttu-id="2848a-131">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [userAccountInformation](../resources/useraccountinformation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2848a-131">If successful, this method returns a `200 OK` response code and the requested [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2848a-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2848a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2848a-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2848a-133">Request</span></span>

<span data-ttu-id="2848a-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2848a-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2848a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2848a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/account/{id}
```
# <a name="c"></a>[<span data-ttu-id="2848a-136">C#</span><span class="sxs-lookup"><span data-stu-id="2848a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-useraccountinformation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2848a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2848a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-useraccountinformation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2848a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2848a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-useraccountinformation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2848a-139">Java</span><span class="sxs-lookup"><span data-stu-id="2848a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-useraccountinformation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2848a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2848a-140">Response</span></span>

<span data-ttu-id="2848a-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2848a-141">The following is an example of the response.</span></span>

> <span data-ttu-id="2848a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2848a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
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
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```


