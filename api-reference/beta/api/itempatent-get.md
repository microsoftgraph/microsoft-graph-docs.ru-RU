---
title: Получение itemPatent
description: Чтение свойств и связей объекта itemPatent.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a30f62fdb622ffb732c9dc807d87577665297dd0
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819927"
---
# <a name="get-itempatent"></a><span data-ttu-id="6fca1-103">Получение itemPatent</span><span class="sxs-lookup"><span data-stu-id="6fca1-103">Get itemPatent</span></span>

<span data-ttu-id="6fca1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fca1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fca1-105">Чтение свойств и связей объекта [itemPatent.](../resources/itempatent.md)</span><span class="sxs-lookup"><span data-stu-id="6fca1-105">Read the properties and relationships of an [itemPatent](../resources/itempatent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fca1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6fca1-106">Permissions</span></span>

<span data-ttu-id="6fca1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6fca1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fca1-109">Permission type</span></span>                        | <span data-ttu-id="6fca1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fca1-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="6fca1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fca1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fca1-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fca1-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6fca1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fca1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fca1-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fca1-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="6fca1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6fca1-115">Application</span></span>                            | <span data-ttu-id="6fca1-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fca1-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="6fca1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fca1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/patents/{id}
GET /users/{id | userPrincipalName}/profile/patents/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6fca1-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6fca1-118">Optional query parameters</span></span>

<span data-ttu-id="6fca1-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="6fca1-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="6fca1-120">Укажите список свойств, включаемых в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="6fca1-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="6fca1-121">Для оптимальной производительности выбирайте только необходимые свойства.</span><span class="sxs-lookup"><span data-stu-id="6fca1-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6fca1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fca1-122">Request headers</span></span>
|<span data-ttu-id="6fca1-123">Имя</span><span class="sxs-lookup"><span data-stu-id="6fca1-123">Name</span></span>|<span data-ttu-id="6fca1-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6fca1-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6fca1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6fca1-125">Authorization</span></span>|<span data-ttu-id="6fca1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fca1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fca1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6fca1-128">Request body</span></span>
<span data-ttu-id="6fca1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6fca1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fca1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fca1-130">Response</span></span>

<span data-ttu-id="6fca1-131">При успешном выполнении этот метод возвращает код `200 OK` отклика [и объект itemPatent](../resources/itempatent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6fca1-131">If successful, this method returns a `200 OK` response code and an [itemPatent](../resources/itempatent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fca1-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="6fca1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6fca1-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fca1-133">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="6fca1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fca1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_itempatent"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/profile/patents/{id}
```
# <a name="c"></a>[<span data-ttu-id="6fca1-135">C#</span><span class="sxs-lookup"><span data-stu-id="6fca1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-itempatent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fca1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fca1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-itempatent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fca1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fca1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-itempatent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6fca1-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fca1-138">Response</span></span>

<span data-ttu-id="6fca1-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6fca1-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPatent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "me",
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
  "description": "Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.",
  "displayName": "Inferring User Intent through browsing behaviors",
  "isPending": true,
  "issuedDate": "Date",
  "issuingAuthority": null,
  "number": "USPTO-3954432633",
  "webUrl": "https://patents.gov/3954432633"
}
```
