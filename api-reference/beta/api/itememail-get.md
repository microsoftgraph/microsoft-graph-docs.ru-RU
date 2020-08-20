---
title: Получение объекта itemEmail
description: Получение свойств и связей объекта itemEmail.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bd6f8a61ad52e8df7692253d9588c748bfce9d91
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820049"
---
# <a name="get-itememail"></a><span data-ttu-id="9702e-103">Получение объекта itemEmail</span><span class="sxs-lookup"><span data-stu-id="9702e-103">Get itemEmail</span></span>

<span data-ttu-id="9702e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9702e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9702e-105">Получение свойств и связей объекта [itemEmail](../resources/itememail.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="9702e-105">Retrieve the properties and relationships of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9702e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9702e-106">Permissions</span></span>

<span data-ttu-id="9702e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9702e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9702e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9702e-109">Permission type</span></span>                        | <span data-ttu-id="9702e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9702e-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="9702e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9702e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9702e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9702e-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9702e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9702e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9702e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9702e-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9702e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9702e-115">Application</span></span>                            | <span data-ttu-id="9702e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9702e-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="9702e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9702e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/emails/{id}
GET /users/{id | userPrincipalName}/profile/emails/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9702e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9702e-118">Optional query parameters</span></span>

<span data-ttu-id="9702e-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="9702e-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="9702e-120">Укажите список свойств, включаемых в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="9702e-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="9702e-121">Для оптимальной производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="9702e-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9702e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9702e-122">Request headers</span></span>
|<span data-ttu-id="9702e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9702e-123">Name</span></span>|<span data-ttu-id="9702e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9702e-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9702e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9702e-125">Authorization</span></span>|<span data-ttu-id="9702e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9702e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9702e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9702e-128">Request body</span></span>
<span data-ttu-id="9702e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9702e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9702e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="9702e-130">Response</span></span>

<span data-ttu-id="9702e-131">При успешном выполнении этот метод возвращает код `200 OK` ответа [и объект itemEmail](../resources/itememail.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9702e-131">If successful, this method returns a `200 OK` response code and an [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9702e-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="9702e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9702e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9702e-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="9702e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9702e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itememail"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{userId}/profile/emails/{id}
```
# <a name="c"></a>[<span data-ttu-id="9702e-135">C#</span><span class="sxs-lookup"><span data-stu-id="9702e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itememail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9702e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9702e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itememail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9702e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9702e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itememail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9702e-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9702e-138">Response</span></span>
<span data-ttu-id="9702e-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9702e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
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
  "address": "Innocenty.Popov@adventureworks.com",
  "displayName": "Business Email",
  "type": "work"
}
```
