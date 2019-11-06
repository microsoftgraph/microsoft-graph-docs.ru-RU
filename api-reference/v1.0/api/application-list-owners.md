---
title: Список владельцев
description: Получение списка владельцев (объектов directoryObject) для приложения.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f91a7926c5635a1f66622b6f3dd7e375d42c3f7d
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37999131"
---
# <a name="list-owners"></a><span data-ttu-id="49776-103">Список владельцев</span><span class="sxs-lookup"><span data-stu-id="49776-103">List owners</span></span>

<span data-ttu-id="49776-104">Получение списка владельцев для приложения, которое является [directoryObject](../resources/directoryobject.md) объектами.</span><span class="sxs-lookup"><span data-stu-id="49776-104">Retrieve a list of owners for an application that are [directoryObject](../resources/directoryobject.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="49776-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49776-105">Permissions</span></span>
<span data-ttu-id="49776-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49776-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49776-108">Permission type</span></span>      | <span data-ttu-id="49776-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49776-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49776-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49776-110">Delegated (work or school account)</span></span> | <span data-ttu-id="49776-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49776-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49776-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49776-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49776-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49776-113">Not supported.</span></span>    |
|<span data-ttu-id="49776-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49776-114">Application</span></span> | <span data-ttu-id="49776-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49776-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49776-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49776-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49776-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49776-117">Optional query parameters</span></span>
<span data-ttu-id="49776-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="49776-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49776-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49776-119">Request headers</span></span>
| <span data-ttu-id="49776-120">Имя</span><span class="sxs-lookup"><span data-stu-id="49776-120">Name</span></span>       | <span data-ttu-id="49776-121">Тип</span><span class="sxs-lookup"><span data-stu-id="49776-121">Type</span></span> | <span data-ttu-id="49776-122">Описание</span><span class="sxs-lookup"><span data-stu-id="49776-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="49776-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49776-123">Authorization</span></span>  | <span data-ttu-id="49776-124">string</span><span class="sxs-lookup"><span data-stu-id="49776-124">string</span></span>  | <span data-ttu-id="49776-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49776-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="49776-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49776-127">Request body</span></span>
<span data-ttu-id="49776-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49776-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49776-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="49776-129">Response</span></span>

<span data-ttu-id="49776-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="49776-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49776-131">Пример</span><span class="sxs-lookup"><span data-stu-id="49776-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49776-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="49776-132">Request</span></span>
<span data-ttu-id="49776-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49776-133">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="49776-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="49776-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/owners
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="49776-135">C#</span><span class="sxs-lookup"><span data-stu-id="49776-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="49776-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49776-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="49776-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49776-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="49776-138">Java</span><span class="sxs-lookup"><span data-stu-id="49776-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49776-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="49776-139">Response</span></span>
<span data-ttu-id="49776-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49776-140">Here is an example of the response.</span></span> 

><span data-ttu-id="49776-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49776-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
