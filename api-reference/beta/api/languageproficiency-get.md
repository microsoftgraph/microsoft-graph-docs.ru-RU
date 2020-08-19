---
title: Получение ЛангуажепрофиЦиенци
description: Получение свойств и связей объекта ЛангуажепрофиЦиенци.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 60e262952e5b849b77665b092c59794988432e61
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811765"
---
# <a name="get-languageproficiency"></a><span data-ttu-id="2b366-103">Получение ЛангуажепрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="2b366-103">Get languageProficiency</span></span>

<span data-ttu-id="2b366-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b366-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b366-105">Получение свойств и связей объекта [лангуажепрофиЦиенци](../resources/languageproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b366-105">Retrieve the properties and relationships of a [languageProficiency](../resources/languageproficiency.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b366-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b366-106">Permissions</span></span>

<span data-ttu-id="2b366-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b366-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b366-109">Permission type</span></span>                        | <span data-ttu-id="2b366-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b366-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="2b366-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b366-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b366-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2b366-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2b366-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b366-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b366-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2b366-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="2b366-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b366-115">Application</span></span>                            | <span data-ttu-id="2b366-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2b366-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="2b366-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b366-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/languages/{id}
GET /users/{id | userPrincipalName}/profile/languages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b366-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b366-118">Optional query parameters</span></span>

<span data-ttu-id="2b366-119">Этот метод поддерживает `$select` параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="2b366-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="2b366-120">Укажите список свойств, которые необходимо включить в ответ, разделяя их запятыми.</span><span class="sxs-lookup"><span data-stu-id="2b366-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="2b366-121">Для обеспечения оптимальной производительности следует выбирать только подмножество нужных свойств.</span><span class="sxs-lookup"><span data-stu-id="2b366-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b366-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b366-122">Request headers</span></span>

| <span data-ttu-id="2b366-123">Имя</span><span class="sxs-lookup"><span data-stu-id="2b366-123">Name</span></span>           |<span data-ttu-id="2b366-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2b366-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="2b366-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b366-125">Authorization</span></span>  | <span data-ttu-id="2b366-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b366-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="2b366-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b366-128">Request body</span></span>

<span data-ttu-id="2b366-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b366-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b366-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b366-130">Response</span></span>

<span data-ttu-id="2b366-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [лангуажепрофиЦиенци](../resources/languageproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b366-131">If successful, this method returns a `200 OK` response code and the requested [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b366-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="2b366-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b366-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b366-133">Request</span></span>

<span data-ttu-id="2b366-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b366-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b366-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b366-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_languageproficiency"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/languages/{id}
```
# <a name="c"></a>[<span data-ttu-id="2b366-136">C#</span><span class="sxs-lookup"><span data-stu-id="2b366-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b366-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b366-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b366-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b366-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="2b366-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b366-139">Response</span></span>

<span data-ttu-id="2b366-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2b366-140">The following is an example of the response.</span></span>

> <span data-ttu-id="2b366-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b366-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.languageProficiency"
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
  "displayName": "Norwegian Bokmål",
  "tag": "nb-NO",
  "spoken": "nativeOrBilingual",
  "written": "nativeOrBilingual",
  "reading": "nativeOrBilingual"
}
```
