---
title: Список объектов contactFolder
description: Получение всех папок контактов в почтовом ящике вошедшего пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f59362e627dc4b23be75f70b84e9824dd7f9ce16
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459514"
---
# <a name="list-contactfolders"></a><span data-ttu-id="55567-103">Список объектов contactFolder</span><span class="sxs-lookup"><span data-stu-id="55567-103">List contactFolders</span></span>

<span data-ttu-id="55567-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55567-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55567-105">Получение всех папок контактов в почтовом ящике вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="55567-105">Get all the contact folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="55567-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55567-106">Permissions</span></span>
<span data-ttu-id="55567-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55567-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55567-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55567-109">Permission type</span></span>      | <span data-ttu-id="55567-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55567-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55567-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55567-111">Delegated (work or school account)</span></span> | <span data-ttu-id="55567-112">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55567-112">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="55567-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55567-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55567-114">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55567-114">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="55567-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55567-115">Application</span></span> | <span data-ttu-id="55567-116">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55567-116">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="55567-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55567-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="55567-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="55567-118">Optional query parameters</span></span>
<span data-ttu-id="55567-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="55567-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="55567-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55567-120">Request headers</span></span>
| <span data-ttu-id="55567-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55567-121">Header</span></span>       | <span data-ttu-id="55567-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55567-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55567-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55567-123">Authorization</span></span>  | <span data-ttu-id="55567-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55567-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="55567-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55567-126">Content-Type</span></span>   | <span data-ttu-id="55567-127">application/json</span><span class="sxs-lookup"><span data-stu-id="55567-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55567-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55567-128">Request body</span></span>
<span data-ttu-id="55567-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55567-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55567-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="55567-130">Response</span></span>

<span data-ttu-id="55567-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55567-131">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="55567-132">Пример</span><span class="sxs-lookup"><span data-stu-id="55567-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55567-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="55567-133">Request</span></span>
<span data-ttu-id="55567-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55567-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55567-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="55567-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contactFolders
```
# <a name="c"></a>[<span data-ttu-id="55567-136">C#</span><span class="sxs-lookup"><span data-stu-id="55567-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contactfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55567-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55567-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contactfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55567-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55567-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contactfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="55567-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="55567-139">Response</span></span>
<span data-ttu-id="55567-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55567-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
