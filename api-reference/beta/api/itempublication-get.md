---
title: Получение элемента itemPublication
description: Чтение свойств и связей объекта itemPublication.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a3a0751c925fd09756aa9b121741bd06eeea7de4
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820326"
---
# <a name="get-itempublication"></a><span data-ttu-id="0b816-103">Получение элемента itemPublication</span><span class="sxs-lookup"><span data-stu-id="0b816-103">Get itemPublication</span></span>

<span data-ttu-id="0b816-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b816-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="0b816-105">Чтение свойств и связей объекта [itemPublication](../resources/itempublication.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="0b816-105">Read the properties and relationships of an [itemPublication](../resources/itempublication.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b816-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b816-106">Permissions</span></span>

<span data-ttu-id="0b816-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b816-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b816-109">Permission type</span></span>                        | <span data-ttu-id="0b816-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b816-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="0b816-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b816-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b816-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b816-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0b816-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b816-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b816-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b816-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="0b816-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0b816-115">Application</span></span>                            | <span data-ttu-id="0b816-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b816-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="0b816-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b816-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/publications/{id}
GET /users/{id | userPrincipalName}/profile/publications/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b816-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b816-118">Optional query parameters</span></span>

<span data-ttu-id="0b816-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="0b816-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="0b816-120">Укажите список свойств, включаемых в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="0b816-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="0b816-121">Для оптимальной производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="0b816-121">For optimal performance, only select the subset of properties needed.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0b816-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b816-122">Request headers</span></span>
|<span data-ttu-id="0b816-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0b816-123">Name</span></span>|<span data-ttu-id="0b816-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0b816-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b816-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b816-125">Authorization</span></span>|<span data-ttu-id="0b816-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b816-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b816-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b816-128">Request body</span></span>
<span data-ttu-id="0b816-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b816-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b816-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b816-130">Response</span></span>

<span data-ttu-id="0b816-131">При успешном выполнении этот метод возвращает код `200 OK` ответа [и объект itemPublication](../resources/itempublication.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b816-131">If successful, this method returns a `200 OK` response code and an [itemPublication](../resources/itempublication.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b816-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b816-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b816-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b816-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="0b816-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b816-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itempublication"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/publications/{id}
```
# <a name="c"></a>[<span data-ttu-id="0b816-135">C#</span><span class="sxs-lookup"><span data-stu-id="0b816-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itempublication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b816-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b816-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itempublication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b816-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b816-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itempublication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0b816-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b816-138">Response</span></span>

<span data-ttu-id="0b816-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0b816-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPublication"
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
  "description": "One persons journey to the top of the branding management field.",
  "displayName": "Got Brands? The story of Innocenty Popov and his journey to the top.",
  "publishedDate": "Date",
  "publisher": "International Association of Branding Management Publishing",
  "thumbnailUrl": "https://iabm.io/sdhdfhsdhshsd.jpg",
  "webUrl": "https://www.iabm.io"
}
```
