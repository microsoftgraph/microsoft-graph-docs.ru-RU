---
title: Получение объекта itemAddress
description: Чтение свойств и связей объекта itemAddress.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: c7004e265b683c4ed0733e4d2c3e24791af2db18
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820076"
---
# <a name="get-itemaddress"></a><span data-ttu-id="466d3-103">Получение объекта itemAddress</span><span class="sxs-lookup"><span data-stu-id="466d3-103">Get itemAddress</span></span>
<span data-ttu-id="466d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="466d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="466d3-105">Чтение свойств и связей объекта [itemAddress.](../resources/itemaddress.md)</span><span class="sxs-lookup"><span data-stu-id="466d3-105">Read the properties and relationships of an [itemAddress](../resources/itemaddress.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="466d3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="466d3-106">Permissions</span></span>

<span data-ttu-id="466d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="466d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="466d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="466d3-109">Permission type</span></span>                        | <span data-ttu-id="466d3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="466d3-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="466d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="466d3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="466d3-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="466d3-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="466d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="466d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="466d3-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="466d3-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="466d3-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="466d3-115">Application</span></span>                            | <span data-ttu-id="466d3-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="466d3-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="466d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="466d3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/addresses/{id}
GET /users/{id | userPrincipalName}/profile/addresses/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="466d3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="466d3-118">Optional query parameters</span></span>

<span data-ttu-id="466d3-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="466d3-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="466d3-120">Укажите список свойств, включаемых в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="466d3-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="466d3-121">Для оптимальной производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="466d3-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="466d3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="466d3-122">Request headers</span></span>
|<span data-ttu-id="466d3-123">Имя</span><span class="sxs-lookup"><span data-stu-id="466d3-123">Name</span></span>|<span data-ttu-id="466d3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="466d3-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="466d3-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="466d3-125">Authorization</span></span>|<span data-ttu-id="466d3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="466d3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="466d3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="466d3-128">Request body</span></span>
<span data-ttu-id="466d3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="466d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="466d3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="466d3-130">Response</span></span>

<span data-ttu-id="466d3-131">При успешном выполнении этот метод возвращает код `200 OK` ответа [и объект itemAddress](../resources/itemaddress.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="466d3-131">If successful, this method returns a `200 OK` response code and an [itemAddress](../resources/itemaddress.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="466d3-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="466d3-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="466d3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="466d3-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="466d3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="466d3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemaddress"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/addresses/{id}
```
# <a name="c"></a>[<span data-ttu-id="466d3-135">C#</span><span class="sxs-lookup"><span data-stu-id="466d3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemaddress-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="466d3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="466d3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemaddress-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="466d3-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="466d3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemaddress-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="466d3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="466d3-138">Response</span></span>

<span data-ttu-id="466d3-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="466d3-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAddress"
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
  "displayName": "Home",
  "detail": {
    "type": "home",
    "postOfficeBox": null,
    "street": "221B Baker Street",
    "city": "London",
    "state": null,
    "countryOrRegion": "United Kingdom",
    "postalCode": "E14 3TD"
  },
  "geoCoordinates": null
}
```
