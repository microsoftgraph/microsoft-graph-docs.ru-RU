---
title: Get languageProficiency
description: Извлечение свойств и связей объекта languageProficiency.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: dbeb53eab0e527c3eeb2335bd3607716fcd1bc15
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052189"
---
# <a name="get-languageproficiency"></a><span data-ttu-id="37a03-103">Get languageProficiency</span><span class="sxs-lookup"><span data-stu-id="37a03-103">Get languageProficiency</span></span>

<span data-ttu-id="37a03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37a03-105">Извлечение свойств и связей [объекта languageProficiency](../resources/languageproficiency.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="37a03-105">Retrieve the properties and relationships of a [languageProficiency](../resources/languageproficiency.md) object within a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37a03-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37a03-106">Permissions</span></span>

<span data-ttu-id="37a03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37a03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37a03-109">Permission type</span></span>                        | <span data-ttu-id="37a03-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37a03-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="37a03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37a03-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37a03-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a03-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="37a03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37a03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37a03-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a03-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="37a03-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="37a03-115">Application</span></span>                            | <span data-ttu-id="37a03-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a03-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="37a03-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37a03-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/languages/{id}
GET /users/{id | userPrincipalName}/profile/languages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37a03-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37a03-118">Optional query parameters</span></span>

<span data-ttu-id="37a03-119">Этот метод поддерживает параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="37a03-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="37a03-120">Укажите список свойств, которые необходимо включить в ответ, разделив их запятой.</span><span class="sxs-lookup"><span data-stu-id="37a03-120">Specify a list of properties to include in the response, separating them by commas.</span></span> <span data-ttu-id="37a03-121">Для оптимальной производительности выберите только подмножество необходимых свойств.</span><span class="sxs-lookup"><span data-stu-id="37a03-121">For optimal performance, only select the subset of properties needed.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37a03-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37a03-122">Request headers</span></span>

| <span data-ttu-id="37a03-123">Имя</span><span class="sxs-lookup"><span data-stu-id="37a03-123">Name</span></span>           |<span data-ttu-id="37a03-124">Описание</span><span class="sxs-lookup"><span data-stu-id="37a03-124">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="37a03-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37a03-125">Authorization</span></span>  | <span data-ttu-id="37a03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37a03-p103">Bearer {token}. Required.</span></span>   |

## <a name="request-body"></a><span data-ttu-id="37a03-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37a03-128">Request body</span></span>

<span data-ttu-id="37a03-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="37a03-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37a03-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a03-130">Response</span></span>

<span data-ttu-id="37a03-131">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [languageProficiency](../resources/languageproficiency.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="37a03-131">If successful, this method returns a `200 OK` response code and the requested [languageProficiency](../resources/languageproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37a03-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="37a03-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37a03-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="37a03-133">Request</span></span>

<span data-ttu-id="37a03-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37a03-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37a03-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a03-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_languageproficiency"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/languages/{id}
```
# <a name="c"></a>[<span data-ttu-id="37a03-136">C#</span><span class="sxs-lookup"><span data-stu-id="37a03-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-languageproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37a03-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a03-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-languageproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37a03-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37a03-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-languageproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37a03-139">Java</span><span class="sxs-lookup"><span data-stu-id="37a03-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-languageproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="37a03-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="37a03-140">Response</span></span>

<span data-ttu-id="37a03-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="37a03-141">The following is an example of the response.</span></span>

> <span data-ttu-id="37a03-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37a03-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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


