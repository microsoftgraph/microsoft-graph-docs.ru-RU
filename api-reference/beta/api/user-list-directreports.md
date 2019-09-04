---
title: Список directReports
description: Получение непосредственных подчиненных пользователя.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff22d99f4982669ba8276a4699c22fdb57c407a7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721987"
---
# <a name="list-directreports"></a><span data-ttu-id="ebe52-103">Список directReports</span><span class="sxs-lookup"><span data-stu-id="ebe52-103">List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebe52-104">Получение непосредственных подчиненных пользователя.</span><span class="sxs-lookup"><span data-stu-id="ebe52-104">Get a user's direct reports.</span></span> <span data-ttu-id="ebe52-105">Возвращает пользователей и контакты, для которых данный пользователь назначен руководителем.</span><span class="sxs-lookup"><span data-stu-id="ebe52-105">Returns the users and contacts for whom this user is assigned as manager.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebe52-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebe52-106">Permissions</span></span>
<span data-ttu-id="ebe52-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebe52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebe52-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebe52-109">Permission type</span></span>      | <span data-ttu-id="ebe52-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebe52-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebe52-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebe52-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebe52-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ebe52-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ebe52-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebe52-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebe52-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="ebe52-114">Not supported</span></span> |
|<span data-ttu-id="ebe52-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebe52-115">Application</span></span> | <span data-ttu-id="ebe52-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebe52-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebe52-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebe52-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebe52-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ebe52-118">Optional query parameters</span></span>
<span data-ttu-id="ebe52-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ebe52-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ebe52-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebe52-120">Request headers</span></span>
| <span data-ttu-id="ebe52-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebe52-121">Header</span></span>       | <span data-ttu-id="ebe52-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ebe52-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="ebe52-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebe52-123">Authorization</span></span>  | <span data-ttu-id="ebe52-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebe52-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ebe52-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ebe52-126">Content-Type</span></span>   | <span data-ttu-id="ebe52-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ebe52-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebe52-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ebe52-128">Request body</span></span>
<span data-ttu-id="ebe52-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebe52-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebe52-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebe52-130">Response</span></span>

<span data-ttu-id="ebe52-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ebe52-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebe52-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ebe52-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebe52-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebe52-133">Request</span></span>
<span data-ttu-id="ebe52-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebe52-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ebe52-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebe52-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ebe52-136">C#</span><span class="sxs-lookup"><span data-stu-id="ebe52-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ebe52-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebe52-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ebe52-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ebe52-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ebe52-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebe52-139">Response</span></span>
<span data-ttu-id="ebe52-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ebe52-140">Here is an example of the response.</span></span> 

><span data-ttu-id="ebe52-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebe52-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
