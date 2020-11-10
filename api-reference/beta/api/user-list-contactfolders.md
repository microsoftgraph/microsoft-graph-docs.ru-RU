---
title: Список объектов contactFolder
description: Получение всех папок контактов в почтовом ящике вошедшего пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cb43b621fa43a32516a18a5bb6de04ea0ab8bea3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982225"
---
# <a name="list-contactfolders"></a><span data-ttu-id="35bd3-103">Список объектов contactFolder</span><span class="sxs-lookup"><span data-stu-id="35bd3-103">List contactFolders</span></span>

<span data-ttu-id="35bd3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35bd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35bd3-105">Получение всех папок контактов в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="35bd3-105">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="35bd3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35bd3-106">Permissions</span></span>
<span data-ttu-id="35bd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35bd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35bd3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35bd3-109">Permission type</span></span>      | <span data-ttu-id="35bd3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35bd3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35bd3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35bd3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35bd3-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35bd3-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="35bd3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35bd3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35bd3-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35bd3-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="35bd3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35bd3-115">Application</span></span> | <span data-ttu-id="35bd3-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="35bd3-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="35bd3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35bd3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35bd3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35bd3-118">Optional query parameters</span></span>
<span data-ttu-id="35bd3-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="35bd3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="35bd3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35bd3-120">Request headers</span></span>
| <span data-ttu-id="35bd3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35bd3-121">Header</span></span>       | <span data-ttu-id="35bd3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="35bd3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="35bd3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35bd3-123">Authorization</span></span>  | <span data-ttu-id="35bd3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35bd3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="35bd3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35bd3-126">Content-Type</span></span>   | <span data-ttu-id="35bd3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="35bd3-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="35bd3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35bd3-128">Request body</span></span>
<span data-ttu-id="35bd3-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35bd3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35bd3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="35bd3-130">Response</span></span>

<span data-ttu-id="35bd3-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35bd3-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35bd3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="35bd3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35bd3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="35bd3-133">Request</span></span>
<span data-ttu-id="35bd3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35bd3-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="35bd3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="35bd3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders
```
# <a name="c"></a>[<span data-ttu-id="35bd3-136">C#</span><span class="sxs-lookup"><span data-stu-id="35bd3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35bd3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35bd3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35bd3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35bd3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35bd3-139">Java</span><span class="sxs-lookup"><span data-stu-id="35bd3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contactfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="35bd3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="35bd3-140">Response</span></span>
<span data-ttu-id="35bd3-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="35bd3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "wellKnownName": "wellKnownName-value",
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
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
