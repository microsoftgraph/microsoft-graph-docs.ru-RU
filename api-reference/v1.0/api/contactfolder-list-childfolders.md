---
title: Список childFolders
description: Получение коллекции дочерних папок для указанной папки с контактами.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e2a11db354ccf85674b9135c51613e924c20a64a
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404275"
---
# <a name="list-childfolders"></a><span data-ttu-id="d2bee-103">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="d2bee-103">List childFolders</span></span>

<span data-ttu-id="d2bee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2bee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2bee-105">Получение коллекции дочерних папок для указанной папки с контактами.</span><span class="sxs-lookup"><span data-stu-id="d2bee-105">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="d2bee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2bee-106">Permissions</span></span>
<span data-ttu-id="d2bee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2bee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2bee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2bee-109">Permission type</span></span>      | <span data-ttu-id="d2bee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2bee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2bee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2bee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2bee-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2bee-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d2bee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2bee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2bee-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2bee-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="d2bee-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2bee-115">Application</span></span> | <span data-ttu-id="d2bee-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2bee-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2bee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2bee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2bee-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2bee-118">Optional query parameters</span></span>
<span data-ttu-id="d2bee-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2bee-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d2bee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2bee-120">Request headers</span></span>
| <span data-ttu-id="d2bee-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d2bee-121">Name</span></span>       | <span data-ttu-id="d2bee-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d2bee-122">Type</span></span> | <span data-ttu-id="d2bee-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d2bee-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d2bee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2bee-124">Authorization</span></span>  | <span data-ttu-id="d2bee-125">string</span><span class="sxs-lookup"><span data-stu-id="d2bee-125">string</span></span>  | <span data-ttu-id="d2bee-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2bee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2bee-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2bee-128">Request body</span></span>
<span data-ttu-id="d2bee-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2bee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2bee-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2bee-130">Response</span></span>

<span data-ttu-id="d2bee-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2bee-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2bee-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d2bee-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2bee-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2bee-133">Request</span></span>
<span data-ttu-id="d2bee-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2bee-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2bee-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2bee-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contactfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
```
# <a name="c"></a>[<span data-ttu-id="d2bee-136">C#</span><span class="sxs-lookup"><span data-stu-id="d2bee-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contactfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2bee-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2bee-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contactfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2bee-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2bee-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contactfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2bee-139">Java</span><span class="sxs-lookup"><span data-stu-id="d2bee-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contactfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2bee-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2bee-140">Response</span></span>
<span data-ttu-id="d2bee-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2bee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->