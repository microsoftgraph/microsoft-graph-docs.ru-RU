---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. Вы можете использовать короткий путь `.../me/MailFolders` для получения верхнего уровня '
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 15aab6ed4b351596cdc884970dbbe9dc0c8b7024
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38702463"
---
# <a name="list-childfolders"></a><span data-ttu-id="4b35d-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="4b35d-104">List childFolders</span></span>

<span data-ttu-id="4b35d-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/mailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="4b35d-p102">Get the folder collection under the specified folder. You can use the `.../me/mailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b35d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b35d-107">Permissions</span></span>
<span data-ttu-id="4b35d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b35d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b35d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b35d-110">Permission type</span></span>      | <span data-ttu-id="4b35d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b35d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b35d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b35d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4b35d-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b35d-113">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4b35d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b35d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b35d-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b35d-115">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="4b35d-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4b35d-116">Application</span></span> | <span data-ttu-id="4b35d-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b35d-117">Mail.ReadBasic.All, Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b35d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b35d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4b35d-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4b35d-119">Optional query parameters</span></span>
<span data-ttu-id="4b35d-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4b35d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4b35d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b35d-121">Request headers</span></span>
| <span data-ttu-id="4b35d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4b35d-122">Name</span></span>       | <span data-ttu-id="4b35d-123">Тип</span><span class="sxs-lookup"><span data-stu-id="4b35d-123">Type</span></span> | <span data-ttu-id="4b35d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4b35d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4b35d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b35d-125">Authorization</span></span>  | <span data-ttu-id="4b35d-126">string</span><span class="sxs-lookup"><span data-stu-id="4b35d-126">string</span></span>  | <span data-ttu-id="4b35d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b35d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b35d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b35d-129">Request body</span></span>
<span data-ttu-id="4b35d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b35d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b35d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b35d-131">Response</span></span>

<span data-ttu-id="4b35d-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b35d-132">If successful, this method returns a `200 OK` response code and collection of [mailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4b35d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4b35d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4b35d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b35d-134">Request</span></span>
<span data-ttu-id="4b35d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b35d-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4b35d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b35d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "mailfolder_get_childfolders"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}/childFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b35d-137">C#</span><span class="sxs-lookup"><span data-stu-id="4b35d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/mailfolder-get-childfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b35d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b35d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/mailfolder-get-childfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b35d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b35d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/mailfolder-get-childfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4b35d-140">Java</span><span class="sxs-lookup"><span data-stu-id="4b35d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/mailfolder-get-childfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4b35d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b35d-141">Response</span></span>
<span data-ttu-id="4b35d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b35d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
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
