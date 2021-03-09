---
title: Get itemPhone
description: Извлечение свойств и связей объекта itemPhone.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0622fef3be1d34c6bac46601eb42af2d2420d2c6
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50577431"
---
# <a name="get-itemphonenumber"></a><span data-ttu-id="658b9-103">Получить itemPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="658b9-103">Get itemPhoneNumber</span></span>

<span data-ttu-id="658b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="658b9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="658b9-105">Извлечение свойств и связей объекта [itemPhone](../resources/itemphone.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="658b9-105">Retrieve the properties and relationships of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="658b9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="658b9-106">Permissions</span></span>

<span data-ttu-id="658b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="658b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="658b9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="658b9-109">Permission type</span></span>                        | <span data-ttu-id="658b9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="658b9-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="658b9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="658b9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="658b9-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="658b9-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="658b9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="658b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="658b9-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="658b9-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="658b9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="658b9-115">Application</span></span>                            | <span data-ttu-id="658b9-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="658b9-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="658b9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="658b9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/phones/{id}
GET /users/{userId}/profile/phones/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="658b9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="658b9-118">Optional query parameters</span></span>

<span data-ttu-id="658b9-119">Этот метод поддерживает параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="658b9-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="658b9-120">Укажите список свойств, которые необходимо включить в ответ, разделив их запятой.</span><span class="sxs-lookup"><span data-stu-id="658b9-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="658b9-121">Для оптимальной производительности выберите только подмножество необходимых свойств.</span><span class="sxs-lookup"><span data-stu-id="658b9-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="658b9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="658b9-122">Request headers</span></span>
|<span data-ttu-id="658b9-123">Имя</span><span class="sxs-lookup"><span data-stu-id="658b9-123">Name</span></span>|<span data-ttu-id="658b9-124">Описание</span><span class="sxs-lookup"><span data-stu-id="658b9-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="658b9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="658b9-125">Authorization</span></span>|<span data-ttu-id="658b9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="658b9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="658b9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="658b9-128">Request body</span></span>
<span data-ttu-id="658b9-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="658b9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="658b9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="658b9-130">Response</span></span>

<span data-ttu-id="658b9-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект itemPhone](../resources/itemphone.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="658b9-131">If successful, this method returns a `200 OK` response code and an [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="658b9-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="658b9-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="658b9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="658b9-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="658b9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="658b9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itemphone"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/phones/{id}
```
# <a name="c"></a>[<span data-ttu-id="658b9-135">C#</span><span class="sxs-lookup"><span data-stu-id="658b9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="658b9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="658b9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="658b9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="658b9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="658b9-138">Java</span><span class="sxs-lookup"><span data-stu-id="658b9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-itemphone-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="658b9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="658b9-139">Response</span></span>
<span data-ttu-id="658b9-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="658b9-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
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
  "displayName": "Car Phone",
  "type": "other",
  "number": "+7 499 342 22 13"
}
```


