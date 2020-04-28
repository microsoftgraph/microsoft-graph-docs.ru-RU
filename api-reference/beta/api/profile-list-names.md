---
title: Перечисление имен
description: Получение списка объектов personName из профиля пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 87688a8e8049370ebe6a0bd4929450f3de7a1301
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228662"
---
# <a name="list-names"></a><span data-ttu-id="c2ba2-103">Перечисление имен</span><span class="sxs-lookup"><span data-stu-id="c2ba2-103">List names</span></span>

<span data-ttu-id="c2ba2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2ba2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2ba2-105">Получение списка объектов [PersonName](../resources/personname.md) из [профиля](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2ba2-105">Retrieve a list of [personName](../resources/personname.md) objects from a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2ba2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ba2-106">Permissions</span></span>

<span data-ttu-id="c2ba2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2ba2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2ba2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ba2-109">Permission type</span></span>                        | <span data-ttu-id="c2ba2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2ba2-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="c2ba2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2ba2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2ba2-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c2ba2-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c2ba2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2ba2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2ba2-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c2ba2-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="c2ba2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2ba2-115">Application</span></span>                            | <span data-ttu-id="c2ba2-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c2ba2-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="c2ba2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2ba2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/profile/names
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c2ba2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2ba2-118">Optional query parameters</span></span>

<span data-ttu-id="c2ba2-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2ba2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c2ba2-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c2ba2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2ba2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2ba2-121">Request headers</span></span>

| <span data-ttu-id="c2ba2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c2ba2-122">Name</span></span>           |<span data-ttu-id="c2ba2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c2ba2-123">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="c2ba2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2ba2-124">Authorization</span></span>  | <span data-ttu-id="c2ba2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2ba2-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="c2ba2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2ba2-127">Content-Type</span></span>   | <span data-ttu-id="c2ba2-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2ba2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2ba2-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2ba2-130">Request body</span></span>

<span data-ttu-id="c2ba2-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2ba2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2ba2-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2ba2-132">Response</span></span>

<span data-ttu-id="c2ba2-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [PersonName](../resources/personname.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2ba2-133">If successful, this method returns a `200 OK` response code and a collection of [personName](../resources/personname.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2ba2-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="c2ba2-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2ba2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2ba2-135">Request</span></span>

<span data-ttu-id="c2ba2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2ba2-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2ba2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2ba2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_names"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/profile/names
```
# <a name="c"></a>[<span data-ttu-id="c2ba2-138">C#</span><span class="sxs-lookup"><span data-stu-id="c2ba2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-names-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2ba2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2ba2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-names-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2ba2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2ba2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-names-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c2ba2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2ba2-141">Response</span></span>

<span data-ttu-id="c2ba2-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2ba2-142">The following is an example of the response.</span></span>

> <span data-ttu-id="c2ba2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2ba2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personName",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "first": "first-value",
      "initials": "initials-value",
      "last": "last-value",
      "languageTag": "languageTag-value",
      "maiden": "maiden-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List names",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
