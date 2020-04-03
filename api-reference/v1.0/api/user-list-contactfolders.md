---
title: Список объектов contactFolder
description: Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5d1033f9e7034a98631403759b29cc9339f6bfb0
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108853"
---
# <a name="list-contactfolders"></a><span data-ttu-id="3de46-103">Список объектов contactFolder</span><span class="sxs-lookup"><span data-stu-id="3de46-103">List contactFolders</span></span>

<span data-ttu-id="3de46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3de46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3de46-105">Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="3de46-105">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="3de46-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3de46-106">Permissions</span></span>
<span data-ttu-id="3de46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3de46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de46-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3de46-109">Permission type</span></span>      | <span data-ttu-id="3de46-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3de46-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3de46-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3de46-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3de46-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3de46-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3de46-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3de46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3de46-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3de46-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3de46-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3de46-115">Application</span></span> | <span data-ttu-id="3de46-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3de46-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3de46-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3de46-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3de46-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3de46-118">Optional query parameters</span></span>
<span data-ttu-id="3de46-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3de46-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3de46-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3de46-120">Request headers</span></span>
| <span data-ttu-id="3de46-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3de46-121">Header</span></span>       | <span data-ttu-id="3de46-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3de46-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3de46-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3de46-123">Authorization</span></span>  | <span data-ttu-id="3de46-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3de46-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3de46-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3de46-126">Content-Type</span></span>   | <span data-ttu-id="3de46-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3de46-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3de46-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3de46-128">Request body</span></span>
<span data-ttu-id="3de46-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3de46-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3de46-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="3de46-130">Response</span></span>

<span data-ttu-id="3de46-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3de46-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3de46-132">Пример</span><span class="sxs-lookup"><span data-stu-id="3de46-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3de46-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3de46-133">Request</span></span>
<span data-ttu-id="3de46-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3de46-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3de46-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3de46-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
# <a name="c"></a>[<span data-ttu-id="3de46-136">C#</span><span class="sxs-lookup"><span data-stu-id="3de46-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3de46-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3de46-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3de46-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3de46-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3de46-139">Java</span><span class="sxs-lookup"><span data-stu-id="3de46-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3de46-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de46-140">Response</span></span>
<span data-ttu-id="3de46-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3de46-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
