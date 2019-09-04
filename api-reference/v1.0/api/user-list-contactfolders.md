---
title: Список объектов contactFolder
description: Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 98a01c64fffdfc395c7eef1ab707c10fa6423963
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727525"
---
# <a name="list-contactfolders"></a><span data-ttu-id="c924e-103">Список объектов contactFolder</span><span class="sxs-lookup"><span data-stu-id="c924e-103">List contactFolders</span></span>

<span data-ttu-id="c924e-104">Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="c924e-104">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="c924e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c924e-105">Permissions</span></span>
<span data-ttu-id="c924e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c924e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c924e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c924e-108">Permission type</span></span>      | <span data-ttu-id="c924e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c924e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c924e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c924e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c924e-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c924e-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c924e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c924e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c924e-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c924e-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c924e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c924e-114">Application</span></span> | <span data-ttu-id="c924e-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c924e-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c924e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c924e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c924e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c924e-117">Optional query parameters</span></span>
<span data-ttu-id="c924e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c924e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c924e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c924e-119">Request headers</span></span>
| <span data-ttu-id="c924e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c924e-120">Header</span></span>       | <span data-ttu-id="c924e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c924e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c924e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c924e-122">Authorization</span></span>  | <span data-ttu-id="c924e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c924e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c924e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c924e-125">Content-Type</span></span>   | <span data-ttu-id="c924e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c924e-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c924e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c924e-127">Request body</span></span>
<span data-ttu-id="c924e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c924e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c924e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c924e-129">Response</span></span>

<span data-ttu-id="c924e-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c924e-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c924e-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c924e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c924e-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c924e-132">Request</span></span>
<span data-ttu-id="c924e-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c924e-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c924e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c924e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c924e-135">C#</span><span class="sxs-lookup"><span data-stu-id="c924e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c924e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c924e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c924e-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c924e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c924e-138">Java</span><span class="sxs-lookup"><span data-stu-id="c924e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c924e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c924e-139">Response</span></span>
<span data-ttu-id="c924e-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c924e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
